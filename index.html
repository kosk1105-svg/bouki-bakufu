[index.html](https://github.com/user-attachments/files/34877430/index.html)
<!DOCTYPE html>
<html lang="ja" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="apple-mobile-web-app-title" content="棒木幕府">
    <title>棒木幕府 (BOUKI BAKUFU) - 3人専用ゲーム評定＆投票ハブ</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;900&family=Noto+Sans+JP:wght@400;500;700;900&display=swap" rel="stylesheet">
    <!-- Tone.js for UI & Roulette Sound Effects -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/tone/14.8.49/Tone.js"></script>

    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['"Inter"', '"Noto Sans JP"', 'sans-serif'],
                    },
                    colors: {
                        gaming: {
                            bg: '#0b0f19',
                            card: '#131b2e',
                            border: '#23304f',
                            accent: '#6366f1',
                            neon: '#00f5d4',
                            pink: '#f72585',
                            amber: '#ffbe0b'
                        }
                    }
                }
            }
        }
    </script>

    <style>
        html, body {
            background-color: #0b0f19;
            color: #f1f5f9;
            font-family: 'Inter', 'Noto Sans JP', sans-serif;
            overflow-x: hidden;
            max-width: 100vw;
            width: 100%;
            -webkit-tap-highlight-color: transparent;
        }
        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 6px;
            height: 6px;
        }
        ::-webkit-scrollbar-track {
            background: #0b0f19;
        }
        ::-webkit-scrollbar-thumb {
            background: #23304f;
            border-radius: 9999px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #6366f1;
        }

        /* Glowing Effects */
        .glow-match {
            box-shadow: 0 0 18px rgba(0, 245, 212, 0.35), inset 0 0 12px rgba(0, 245, 212, 0.15);
            border-color: #00f5d4 !important;
        }
        .glow-chance {
            box-shadow: 0 0 14px rgba(255, 190, 11, 0.25);
            border-color: #ffbe0b !important;
        }
        .glow-unanimous {
            box-shadow: 0 0 20px rgba(247, 37, 133, 0.4);
            border-color: #f72585 !important;
        }

        @keyframes pulse-border {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.65; }
        }
        .animate-pulse-slow {
            animation: pulse-border 2.8s infinite ease-in-out;
        }

        .glass-panel {
            background: rgba(19, 27, 46, 0.85);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }
    </style>
</head>
<body class="min-h-screen flex flex-col pb-20 md:pb-6 selection:bg-indigo-500 selection:text-white">

    <!-- TOP NAVIGATION / MEMBER SWITCHER HEADER -->
    <header class="sticky top-0 z-30 glass-panel border-b border-gaming-border px-3 sm:px-6 py-3">
        <div class="max-w-7xl mx-auto flex flex-wrap items-center justify-between gap-3">
            <!-- Brand & Sync Status -->
            <div class="flex items-center gap-3">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-amber-500 via-indigo-600 to-purple-700 flex items-center justify-center shadow-lg shadow-amber-500/25 border border-amber-400/40">
                    <i class="fa-solid fa-torii-gate text-white text-lg"></i>
                </div>
                <div>
                    <div class="flex items-center flex-wrap gap-2">
                        <h1 class="font-black text-lg sm:text-xl tracking-wider bg-clip-text text-transparent bg-gradient-to-r from-amber-200 via-white to-indigo-300">
                            棒木幕府
                        </h1>
                        <span class="text-[10px] font-black px-2 py-0.5 rounded-md bg-amber-500/20 text-amber-300 border border-amber-400/30">
                            BOUKI BAKUFU
                        </span>
                        <span id="syncBadge" class="inline-flex items-center gap-1 text-[10px] font-bold px-2 py-0.5 rounded-full bg-emerald-500/20 text-emerald-300 border border-emerald-500/30">
                            <span class="w-1.5 h-1.5 rounded-full bg-emerald-400 animate-ping"></span>
                            LIVE同期
                        </span>
                        <button onclick="openDiscordSettingsModal()" id="discordHeaderBadge" class="inline-flex items-center gap-1 text-[10px] font-black px-2.5 py-0.5 rounded-full bg-slate-800 text-slate-400 border border-slate-700 hover:border-indigo-400 transition">
                            <i class="fa-brands fa-discord"></i>
                            <span>Discord未設定</span>
                        </button>
                    </div>
                    <p class="text-xs text-slate-400 hidden sm:block">3人専用ゲーム評定（予定合わせ）＆タイトル投票ハブ</p>
                </div>
            </div>

            <!-- Active Member Selector (3 Players) -->
            <div class="flex flex-wrap items-center gap-1.5 sm:gap-2 bg-slate-900/90 p-1.5 rounded-2xl border border-gaming-border max-w-full">
                <span class="text-[11px] text-slate-400 px-2 hidden lg:inline"><i class="fa-solid fa-user-check mr-1 text-amber-400"></i>操作中の家臣:</span>
                <div id="memberSwitcherContainer" class="flex items-center gap-1 sm:gap-1.5 flex-wrap">
                    <!-- Rendered dynamically via JS -->
                </div>
                <button onclick="openDiscordSettingsModal()" title="Discord自動通知（3人の予定が合った時だけ通知）の設定" class="px-2 sm:px-2.5 h-8 rounded-xl bg-[#5865F2]/25 hover:bg-[#5865F2]/40 border border-[#5865F2]/50 text-indigo-200 text-xs font-bold flex items-center gap-1.5 transition shrink-0">
                    <i class="fa-brands fa-discord text-[#5865F2]"></i>
                    <span class="hidden sm:inline">伝令設定</span>
                </button>
                <button onclick="openOnboardingModal(true)" title="初期登録・マイプロフィール設定" class="px-2 sm:px-2.5 h-8 rounded-xl bg-amber-500/20 hover:bg-amber-500/35 border border-amber-500/40 text-amber-200 text-xs font-bold flex items-center gap-1.5 transition shrink-0">
                    <i class="fa-solid fa-id-card"></i>
                    <span class="hidden sm:inline">プロフィール変更</span>
                </button>
            </div>
        </div>
    </header>

    <!-- QUICK STATUS BAR (3 MEMBERS' CURRENT VOICE/MEMO BUBBLES + 1-TAP SIGNAL) -->
    <section class="bg-slate-900/60 border-b border-gaming-border/70 px-2.5 sm:px-6 py-2.5 overflow-hidden">
        <div class="max-w-7xl mx-auto flex flex-col gap-2">
            <div class="flex flex-col md:flex-row items-stretch md:items-center justify-between gap-2.5">
                <div id="memberStatusPills" class="grid grid-cols-3 gap-1.5 sm:gap-2 flex-1 min-w-0">
                    <!-- 3 Member status pills rendered by JS -->
                </div>
                <div class="flex items-center gap-1 sm:gap-1.5 flex-wrap">
                    <span class="text-[10px] font-black text-amber-300 px-1"><i class="fa-solid fa-bolt mr-0.5"></i>今すぐ状況:</span>
                    <button onclick="setOneTapRealtimeSignal('🟢 今すぐ遊べる！')" class="px-2 py-1 rounded-lg bg-emerald-500/20 hover:bg-emerald-500/35 text-emerald-300 border border-emerald-500/30 text-[10px] sm:text-[11px] font-bold transition">
                        🟢 今すぐOK
                    </button>
                    <button onclick="setOneTapRealtimeSignal('♨️ 風呂・飯（後で合流）')" class="px-2 py-1 rounded-lg bg-amber-500/20 hover:bg-amber-500/35 text-amber-300 border border-amber-500/30 text-[10px] sm:text-[11px] font-bold transition">
                        ♨️ 風呂・飯
                    </button>
                    <button onclick="setOneTapRealtimeSignal('📺 作業・画面共有OK')" class="px-2 py-1 rounded-lg bg-sky-500/20 hover:bg-sky-500/35 text-sky-300 border border-sky-500/30 text-[10px] sm:text-[11px] font-bold transition">
                        📺 通話OK
                    </button>
                    <button onclick="setOneTapRealtimeSignal('💤 今日は寝落ち・休息')" class="px-2 py-1 rounded-lg bg-slate-800 hover:bg-slate-700 text-slate-300 border border-slate-700 text-[10px] sm:text-[11px] font-bold transition">
                        💤 休息
                    </button>
                    <button onclick="toggleSound()" id="soundToggleBtn" class="px-2 py-1 rounded-lg bg-slate-800 hover:bg-slate-700 text-slate-400 border border-slate-700 text-xs transition" title="効果音ON/OFF">
                        <i class="fa-solid fa-volume-xmark"></i>
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- MAIN CONTENT CONTAINER -->
    <main class="max-w-7xl w-full mx-auto px-2 sm:px-6 py-4 sm:py-5 flex-1 flex flex-col gap-5 overflow-hidden">

        <!-- DESKTOP NAVIGATION TABS -->
        <div class="hidden md:flex items-center justify-between bg-gaming-card p-1.5 rounded-2xl border border-gaming-border">
            <div class="flex items-center gap-2">
                <button onclick="switchTab('calendar')" id="tabBtn-calendar" class="tab-btn px-5 py-2.5 rounded-xl font-bold text-sm flex items-center gap-2 transition bg-indigo-600 text-white shadow-lg shadow-indigo-600/30">
                    <i class="fa-regular fa-calendar-check"></i>
                    <span>評定カレンダー</span>
                    <span id="matchCountBadge" class="ml-1 px-2 py-0.5 text-xs rounded-full bg-emerald-400 text-slate-950 font-black">0</span>
                </button>
                <button onclick="switchTab('games')" id="tabBtn-games" class="tab-btn px-5 py-2.5 rounded-xl font-bold text-sm flex items-center gap-2 transition text-slate-300 hover:bg-slate-800">
                    <i class="fa-solid fa-fire-flame-curved text-pink-400"></i>
                    <span>ゲーム検索＆やりたい投票</span>
                    <span id="gameCountBadge" class="ml-1 px-2 py-0.5 text-xs rounded-full bg-slate-700 text-slate-200 font-bold">0</span>
                </button>
                <button onclick="switchTab('arcade')" id="tabBtn-arcade" class="tab-btn px-5 py-2.5 rounded-xl font-bold text-sm flex items-center gap-2 transition text-slate-300 hover:bg-slate-800">
                    <i class="fa-solid fa-gamepad text-emerald-400"></i>
                    <span>幕府遊戯場 (ミニゲーム)</span>
                    <span class="ml-1 px-1.5 py-0.5 text-[10px] rounded-full bg-emerald-500/20 text-emerald-300 border border-emerald-500/40 font-black">4種</span>
                </button>
                <button onclick="switchTab('party')" id="tabBtn-party" class="tab-btn px-5 py-2.5 rounded-xl font-bold text-sm flex items-center gap-2 transition text-slate-300 hover:bg-slate-800">
                    <i class="fa-solid fa-scroll text-amber-400"></i>
                    <span>軍議・番付・年表</span>
                </button>
                <button onclick="switchTab('appguide')" id="tabBtn-appguide" class="tab-btn px-5 py-2.5 rounded-xl font-bold text-sm flex items-center gap-2 transition text-slate-300 hover:bg-slate-800">
                    <i class="fa-brands fa-discord text-[#5865F2]"></i>
                    <span>Discord伝令・アプリ化</span>
                </button>
            </div>
            <div class="pr-3 text-xs text-slate-400 flex items-center gap-2">
                <span>3人揃う日: <strong id="headerMatchSummary" class="text-emerald-400">0日</strong></span>
                <span>|</span>
                <span>満場一致ゲーム: <strong id="headerUnanimousSummary" class="text-pink-400">0本</strong></span>
            </div>
        </div>

        <!-- ==========================================
             TAB 1: 3-MEMBER INTERACTIVE CALENDAR
             ========================================== -->
        <section id="view-calendar" class="space-y-5">
            <!-- Next Match Hero Banner & Quick Batch Input -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-4">
                <!-- Match Highlight Banner -->
                <div class="lg:col-span-2 rounded-2xl bg-gradient-to-r from-indigo-950/90 via-slate-900 to-emerald-950/80 border border-emerald-500/40 p-4 sm:p-5 flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4 relative overflow-hidden">
                    <div class="space-y-1 z-10">
                        <div class="inline-flex items-center gap-1.5 text-xs font-black uppercase tracking-wider text-emerald-300 bg-emerald-500/20 px-2.5 py-0.5 rounded-full border border-emerald-400/30">
                            <i class="fa-solid fa-bolt"></i> PARTY MATCH RADAR
                        </div>
                        <h2 id="nextMatchHeadline" class="text-lg sm:text-xl font-black text-white pt-1">
                            カレンダーの日付をタップして3人の予定を入れよう！
                        </h2>
                        <p id="nextMatchSubtext" class="text-xs sm:text-sm text-slate-300">
                            3人全員が「◯」または「△」の日はネオン枠で自動ハイライトされます。
                        </p>
                    </div>
                    <div class="flex items-center flex-wrap gap-2 self-end sm:self-center z-10">
                        <button onclick="quickFillAvailableForActiveMember()" class="px-3.5 py-2 rounded-xl bg-emerald-500 hover:bg-emerald-400 text-slate-950 font-black text-xs shadow-lg shadow-emerald-500/25 flex items-center gap-1.5 transition">
                            <i class="fa-solid fa-wand-magic-sparkles"></i>
                            <span>今週末(金土日)に「◯」を入力/解除</span>
                        </button>
                        <button onclick="clearCurrentMonthForActiveMember()" title="表示中の月の自分の予定をリセット" class="px-2.5 py-2 rounded-xl bg-slate-800/90 hover:bg-rose-950/80 text-slate-300 hover:text-rose-300 border border-slate-700 font-bold text-xs flex items-center gap-1 transition">
                            <i class="fa-solid fa-eraser"></i>
                            <span>今月クリア</span>
                        </button>
                    </div>
                </div>

                <!-- Legend & Quick Guide Card -->
                <div class="rounded-2xl bg-gaming-card border border-gaming-border p-4 flex flex-col justify-between gap-3">
                    <div class="flex items-center justify-between">
                        <span class="text-xs font-bold text-slate-300"><i class="fa-solid fa-palette text-indigo-400 mr-1"></i>カレンダーの色とマッチ判定</span>
                        <span id="activeMemberIndicatorText" class="text-xs font-bold text-indigo-300 bg-indigo-500/20 px-2 py-0.5 rounded-lg"></span>
                    </div>
                    <div class="grid grid-cols-2 gap-2 text-xs">
                        <div class="bg-emerald-500/25 p-2.5 rounded-xl border-2 border-emerald-400 flex items-center gap-2.5">
                            <span class="w-4 h-4 rounded-md bg-emerald-400 shrink-0 shadow shadow-emerald-400/50"></span>
                            <div>
                                <div class="text-emerald-300 font-black text-xs">緑色に発光</div>
                                <div class="text-[10px] text-emerald-100/80">3人全員「◯」</div>
                            </div>
                        </div>
                        <div class="bg-amber-500/25 p-2.5 rounded-xl border-2 border-amber-400 flex items-center gap-2.5">
                            <span class="w-4 h-4 rounded-md bg-amber-400 shrink-0 shadow shadow-amber-400/50"></span>
                            <div>
                                <div class="text-amber-300 font-black text-xs">金色に発光</div>
                                <div class="text-[10px] text-amber-100/80">3人「◯・△」</div>
                            </div>
                        </div>
                    </div>
                    <div class="text-[11px] text-slate-400 flex items-center justify-around pt-1 border-t border-slate-800">
                        <span><strong class="text-emerald-400">◯</strong> いつでもOK</span>
                        <span><strong class="text-amber-400">△</strong> 条件・時間付</span>
                        <span><strong class="text-rose-400">×</strong> 参加不可</span>
                    </div>
                </div>
            </div>

            <!-- Calendar Controls -->
            <div class="bg-gaming-card rounded-2xl border border-gaming-border p-2.5 sm:p-5 overflow-hidden">
                <div class="flex flex-wrap items-center justify-between gap-2.5 mb-3 sm:mb-4">
                    <div class="flex items-center gap-1.5 sm:gap-2">
                        <button onclick="changeMonth(-1)" class="w-8 h-8 sm:w-9 sm:h-9 rounded-xl bg-slate-800 hover:bg-slate-700 text-slate-200 flex items-center justify-center transition">
                            <i class="fa-solid fa-chevron-left"></i>
                        </button>
                        <h3 id="calendarMonthTitle" class="text-base sm:text-xl font-black px-1.5 sm:px-2 tracking-wide">2025年 5月</h3>
                        <button onclick="changeMonth(1)" class="w-8 h-8 sm:w-9 sm:h-9 rounded-xl bg-slate-800 hover:bg-slate-700 text-slate-200 flex items-center justify-center transition">
                            <i class="fa-solid fa-chevron-right"></i>
                        </button>
                        <button onclick="goToTodayMonth()" class="ml-0.5 px-2.5 py-1.5 rounded-xl bg-slate-800 hover:bg-slate-700 text-xs font-bold text-slate-300 transition">
                            今月
                        </button>
                    </div>

                    <!-- One-tap Quick Stamp Mode -->
                    <div class="flex items-center gap-1 bg-slate-900 p-1 rounded-xl border border-slate-800 max-w-full overflow-x-auto">
                        <span class="text-[10px] sm:text-[11px] text-slate-400 px-1 shrink-0"><i class="fa-solid fa-hand-pointer mr-0.5 text-amber-400"></i>タップ:</span>
                        <button onclick="setQuickStampMode('modal')" id="stampMode-modal" class="px-2 py-1 rounded-lg text-[11px] sm:text-xs font-bold bg-indigo-600 text-white transition shrink-0">
                            詳細
                        </button>
                        <button onclick="setQuickStampMode('o')" id="stampMode-o" class="px-2 py-1 rounded-lg text-[11px] sm:text-xs font-bold text-emerald-400 hover:bg-slate-800 transition shrink-0">
                            連続◯
                        </button>
                        <button onclick="setQuickStampMode('m')" id="stampMode-m" class="px-2 py-1 rounded-lg text-[11px] sm:text-xs font-bold text-amber-400 hover:bg-slate-800 transition shrink-0">
                            連続△
                        </button>
                        <button onclick="setQuickStampMode('x')" id="stampMode-x" class="px-2 py-1 rounded-lg text-[11px] sm:text-xs font-bold text-rose-400 hover:bg-slate-800 transition shrink-0">
                            連続×
                        </button>
                    </div>
                </div>

                <!-- Day of week header -->
                <div class="grid grid-cols-7 gap-1 sm:gap-2 mb-1.5 text-center text-[11px] sm:text-xs font-bold">
                    <div class="text-rose-400 py-1">日</div>
                    <div class="text-slate-400 py-1">月</div>
                    <div class="text-slate-400 py-1">火</div>
                    <div class="text-slate-400 py-1">水</div>
                    <div class="text-slate-400 py-1">木</div>
                    <div class="text-slate-400 py-1">金</div>
                    <div class="text-sky-400 py-1">土</div>
                </div>

                <!-- Calendar Days Grid -->
                <div id="calendarGrid" class="grid grid-cols-7 gap-1 sm:gap-2 w-full">
                    <!-- Populated via JS -->
                </div>
            </div>

            <!-- Matched Days Summary List -->
            <div class="bg-gaming-card rounded-2xl border border-gaming-border p-4 sm:p-5">
                <div class="flex items-center justify-between mb-3">
                    <h4 class="font-black text-base flex items-center gap-2">
                        <i class="fa-solid fa-crown text-amber-400"></i>
                        <span>3人が集まれる候補日リスト</span>
                    </h4>
                    <span class="text-xs text-slate-400">日付をクリックでプレイするゲームを設定</span>
                </div>
                <div id="matchedDaysList" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-3">
                    <!-- Populated via JS -->
                </div>
            </div>
        </section>

        <!-- ==========================================
             TAB 2: INTERNET GAME SEARCH & VOTING BOARD
             ========================================== -->
        <section id="view-games" class="space-y-6 hidden">
            <!-- Internet Game Search & Catalog Box -->
            <div class="bg-gradient-to-br from-indigo-950/90 via-gaming-card to-slate-900 rounded-2xl border border-indigo-500/40 p-4 sm:p-6 shadow-xl space-y-5">
                <div class="flex flex-col md:flex-row md:items-center justify-between gap-4">
                    <div>
                        <span class="inline-flex items-center gap-1 text-[11px] font-black uppercase tracking-wider text-indigo-300 bg-indigo-500/20 px-2.5 py-0.5 rounded-full border border-indigo-400/30">
                            <i class="fa-solid fa-globe"></i> ONLINE GAME ICON & ACTIVITY CATALOG
                        </span>
                        <h2 class="text-lg sm:text-xl font-black text-white mt-1">
                            ネットからゲームアイコンを参照してリスト登録 ＆ その他の選択肢
                        </h2>
                        <p class="text-xs text-slate-300">
                            遊ぶゲームがいつでも変わってOK！ネット検索・人気ジャンル別カタログ・「その他（雑談や当日決め）」からワンタップで投票リストに追加できます。
                        </p>
                    </div>
                    <button onclick="openCustomGameModal()" class="self-start md:self-center px-3.5 py-2.5 rounded-xl bg-pink-600/20 hover:bg-pink-600/40 text-pink-200 border border-pink-500/40 text-xs font-black flex items-center gap-1.5 transition shrink-0">
                        <i class="fa-solid fa-pen-ruler"></i>
                        <span>自由入力・その他を自作追加</span>
                    </button>
                </div>

                <!-- Search Input Bar -->
                <div class="flex flex-col sm:flex-row gap-2">
                    <div class="relative flex-1">
                        <i class="fa-solid fa-magnifying-glass absolute left-4 top-1/2 -translate-y-1/2 text-slate-400"></i>
                        <input
                            type="text"
                            id="gameSearchInput"
                            placeholder="ゲーム名を入力してネットからアイコン検索 (例: モンハン, Apex, マリパ, スト6, 原神...)"
                            onkeydown="if(event.key === 'Enter') searchGamesFromInternet()"
                            class="w-full pl-11 pr-4 py-3 rounded-xl bg-slate-950/90 border border-gaming-border focus:border-indigo-400 focus:outline-none text-sm text-white placeholder-slate-500"
                        >
                    </div>
                    <div class="flex items-center gap-2">
                        <select id="searchPlatformSelect" class="px-3 py-3 rounded-xl bg-slate-950/90 border border-gaming-border text-xs font-bold text-slate-200 focus:outline-none">
                            <option value="Crossplay">🌐 クロスプレイ / 全機種</option>
                            <option value="Switch">🎮 Switch</option>
                            <option value="PC">💻 PC (Steam等)</option>
                            <option value="PS5">🕹️ PS5 / PS4</option>
                            <option value="Mobile">📱 スマホアプリ</option>
                            <option value="その他">🎲 その他・自由枠</option>
                        </select>
                        <button onclick="searchGamesFromInternet()" id="searchGameBtn" class="px-5 py-3 rounded-xl bg-indigo-600 hover:bg-indigo-500 text-white font-black text-sm shadow-lg shadow-indigo-600/30 flex items-center gap-2 transition shrink-0">
                            <i class="fa-solid fa-cloud-arrow-down"></i>
                            <span>ネット検索</span>
                        </button>
                    </div>
                </div>

                <!-- Browsable Online Catalog Tabs + Flexible "Other" Options -->
                <div class="bg-slate-950/80 rounded-2xl border border-slate-800 p-3.5 space-y-3">
                    <div class="flex flex-wrap items-center justify-between gap-2 border-b border-slate-800/80 pb-2.5">
                        <div class="flex items-center gap-1.5 flex-wrap">
                            <span class="text-xs font-black text-indigo-300 mr-1"><i class="fa-solid fa-layer-group mr-1"></i>カタログから選ぶ:</span>
                            <button onclick="loadCatalogCategory('fps_action')" id="catTab-fps_action" class="cat-tab-btn px-3 py-1.5 rounded-xl text-xs font-black bg-indigo-600 text-white transition">
                                🔥 定番マルチ・FPS
                            </button>
                            <button onclick="loadCatalogCategory('party_switch')" id="catTab-party_switch" class="cat-tab-btn px-3 py-1.5 rounded-xl text-xs font-bold bg-slate-900 text-slate-300 hover:bg-slate-800 transition">
                                🎉 パーティ・Switch・ボドゲ
                            </button>
                            <button onclick="loadCatalogCategory('coop_survival')" id="catTab-coop_survival" class="cat-tab-btn px-3 py-1.5 rounded-xl text-xs font-bold bg-slate-900 text-slate-300 hover:bg-slate-800 transition">
                                🌲 サバイバル・協力・RPG
                            </button>
                            <button onclick="loadCatalogCategory('mobile_cross')" id="catTab-mobile_cross" class="cat-tab-btn px-3 py-1.5 rounded-xl text-xs font-bold bg-slate-900 text-slate-300 hover:bg-slate-800 transition">
                                📱 スマホ・クロスプレイ
                            </button>
                            <button onclick="loadCatalogCategory('other_activities')" id="catTab-other_activities" class="cat-tab-btn px-3 py-1.5 rounded-xl text-xs font-bold bg-amber-500/20 text-amber-300 border border-amber-500/30 hover:bg-amber-500/30 transition">
                                🎲 その他・自由な選択肢
                            </button>
                        </div>
                        <span id="catalogSyncStatus" class="text-[11px] text-slate-400">ネットからアイコン自動取得対応</span>
                    </div>

                    <!-- Scrollable Visual Catalog List -->
                    <div id="catalogItemsGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-2.5 max-h-72 overflow-y-auto p-1">
                        <!-- Populated dynamically via JS with live-fetched icons -->
                    </div>
                </div>

                <!-- Live Search Results Drawer (Shown when user searches custom query) -->
                <div id="searchResultsContainer" class="pt-2 border-t border-indigo-500/30 hidden">
                    <div class="flex items-center justify-between mb-2.5">
                        <span id="searchStatusText" class="text-xs font-black text-emerald-300">ネット検索結果リスト</span>
                        <button onclick="closeSearchResults()" class="px-2.5 py-1 rounded-lg bg-slate-800 text-xs text-slate-300 hover:text-white">
                            <i class="fa-solid fa-xmark mr-1"></i>検索結果を閉じる
                        </button>
                    </div>
                    <div id="searchResultsGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-3 max-h-80 overflow-y-auto p-1">
                        <!-- Search results injected via JS -->
                    </div>
                </div>
            </div>

            <!-- Voting Filter & Lifecycle Status Header -->
            <div class="flex flex-wrap items-center justify-between gap-3">
                <div class="flex items-center gap-1.5 flex-wrap bg-gaming-card p-1.5 rounded-2xl border border-gaming-border text-xs">
                    <button onclick="setGameFilter('all')" id="filterBtn-all" class="px-3 py-1.5 rounded-lg font-black bg-indigo-600 text-white transition">
                        🔥 現役・投票中すべて
                    </button>
                    <button onclick="setGameFilter('unanimous')" id="filterBtn-unanimous" class="px-3 py-1.5 rounded-lg font-bold text-slate-300 hover:bg-slate-800 transition">
                        👑 3/3 満場一致
                    </button>
                    <button onclick="setGameFilter('playing')" id="filterBtn-playing" class="px-3 py-1.5 rounded-lg font-bold text-slate-300 hover:bg-slate-800 transition">
                        🎮 いま遊んでる
                    </button>
                    <button onclick="setGameFilter('other')" id="filterBtn-other" class="px-3 py-1.5 rounded-lg font-bold text-slate-300 hover:bg-slate-800 transition">
                        🎲 その他・自由枠
                    </button>
                    <button onclick="setGameFilter('cleared')" id="filterBtn-cleared" class="px-3 py-1.5 rounded-lg font-bold text-slate-300 hover:bg-slate-800 transition">
                        🏆 殿堂入り・休止中
                    </button>
                </div>
                <span class="text-xs text-slate-400">3人全員が投票すると「🔥3/3 満場一致！」になります</span>
            </div>

            <!-- Games Voting Cards Grid -->
            <div id="gamesVotingGrid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                <!-- Populated dynamically via JS -->
            </div>
        </section>

        <!-- ==========================================
             TAB 2.5: BOUKI BAKUFU ARCADE (4 MINI-GAMES & 3-PLAYER LEADERBOARD)
             ========================================== -->
        <section id="view-arcade" class="space-y-6 hidden">
            <!-- Arcade Header & 3-Player Live Leaderboard -->
            <div class="bg-gradient-to-br from-emerald-950/90 via-gaming-card to-indigo-950/90 rounded-2xl border border-emerald-500/40 p-4 sm:p-6 shadow-xl space-y-5">
                <div class="flex flex-col md:flex-row md:items-center justify-between gap-4">
                    <div>
                        <span class="inline-flex items-center gap-1.5 text-[11px] font-black uppercase tracking-wider text-emerald-300 bg-emerald-500/20 px-2.5 py-0.5 rounded-full border border-emerald-400/30">
                            <i class="fa-solid fa-trophy"></i> BAKUFU ARCADE & MINI-GAMES
                        </span>
                        <h2 class="text-lg sm:text-xl font-black text-white mt-1">
                            🎮 棒木幕府「御前試合・遊戯場」（4大ミニゲーム＆3人番付）
                        </h2>
                        <p class="text-xs text-slate-300">
                            集合前の暇つぶしや、部屋ホスト・罰ゲーム決めに！記録は3人全員の画面にリアルタイム同期されます。
                        </p>
                    </div>
                    <!-- Mini-game Selector Pills -->
                    <div class="flex flex-wrap items-center gap-1.5 bg-slate-950/90 p-1.5 rounded-2xl border border-slate-800">
                        <button onclick="selectMiniGame('iai')" id="mgTab-iai" class="px-3 py-2 rounded-xl text-xs font-black bg-emerald-500 text-slate-950 transition flex items-center gap-1.5">
                            <span>⚡ 居合斬り</span>
                        </button>
                        <button onclick="selectMiniGame('mash')" id="mgTab-mash" class="px-3 py-2 rounded-xl text-xs font-bold text-slate-300 hover:bg-slate-800 transition flex items-center gap-1.5">
                            <span>🥁 太鼓連打</span>
                        </button>
                        <button onclick="selectMiniGame('memory')" id="mgTab-memory" class="px-3 py-2 rounded-xl text-xs font-bold text-slate-300 hover:bg-slate-800 transition flex items-center gap-1.5">
                            <span>🃏 絵札合わせ</span>
                        </button>
                        <button onclick="selectMiniGame('bomb')" id="mgTab-bomb" class="px-3 py-2 rounded-xl text-xs font-bold text-slate-300 hover:bg-slate-800 transition flex items-center gap-1.5">
                            <span>💣 爆弾回し</span>
                        </button>
                    </div>
                </div>

                <!-- 3-Player Synchronized High Score Leaderboard -->
                <div id="arcadeLeaderboardGrid" class="grid grid-cols-1 md:grid-cols-3 gap-3">
                    <!-- Rendered dynamically via JS -->
                </div>
            </div>

            <!-- MINI-GAME 1: IAI SLASH (REFLEX SPEED DUEL) -->
            <div id="mgPanel-iai" class="bg-gaming-card rounded-2xl border border-gaming-border p-5 sm:p-6 space-y-5">
                <div class="flex flex-wrap items-center justify-between gap-2">
                    <div>
                        <span class="text-[10px] font-black uppercase text-amber-300 bg-amber-500/20 px-2 py-0.5 rounded-full">GAME 01 • REFLEX DUEL</span>
                        <h3 class="text-lg font-black text-white mt-0.5">⚡ 刹那の居合斬り（反射神経対決）</h3>
                        <p class="text-xs text-slate-400">「構え...」の後、画面が光って<strong>「斬れ！！」</strong>と出た瞬間にタップ！最速タイム(ms)が記録されます。</p>
                    </div>
                    <div class="text-xs font-bold text-emerald-400 bg-slate-950 px-3 py-1.5 rounded-xl border border-slate-800">
                        200ms以下で「剣豪」、150ms以下で「将軍級」！
                    </div>
                </div>

                <div
                    id="iaiArenaBox"
                    onclick="handleIaiArenaTap()"
                    class="w-full min-h-[220px] sm:min-h-[260px] rounded-2xl border-2 border-slate-700 bg-slate-950 flex flex-col items-center justify-center p-6 text-center cursor-pointer select-none transition-all duration-150 shadow-inner"
                >
                    <div id="iaiIconDisplay" class="text-5xl sm:text-6xl mb-3">⚔️</div>
                    <div id="iaiMainText" class="text-xl sm:text-2xl font-black text-white">ここをタップして「居合の構え」を開始</div>
                    <div id="iaiSubText" class="text-xs sm:text-sm text-slate-400 mt-2">合図が出る前に押すと「お手付き（フライング）」になります</div>
                </div>
            </div>

            <!-- MINI-GAME 2: 10-SECOND TAIKO MASH -->
            <div id="mgPanel-mash" class="bg-gaming-card rounded-2xl border border-gaming-border p-5 sm:p-6 space-y-5 hidden">
                <div class="flex flex-wrap items-center justify-between gap-2">
                    <div>
                        <span class="text-[10px] font-black uppercase text-pink-400 bg-pink-500/20 px-2 py-0.5 rounded-full">GAME 02 • 10s SPEED TAP</span>
                        <h3 class="text-lg font-black text-white mt-0.5">🥁 陣太鼓・10秒間鬼連打チャレンジ</h3>
                        <p class="text-xs text-slate-400">制限時間10秒で何回連打できるか勝負！自己ベストを更新すると自動で3人番付に刻まれます。</p>
                    </div>
                    <button onclick="resetMashGame()" class="px-3.5 py-1.5 rounded-xl bg-slate-800 hover:bg-slate-700 text-xs font-bold text-slate-200">
                        <i class="fa-solid fa-rotate-right mr-1"></i>リセット
                    </button>
                </div>

                <div class="grid grid-cols-2 gap-3 text-center">
                    <div class="bg-slate-950 p-3.5 rounded-2xl border border-slate-800">
                        <div class="text-xs text-slate-400 font-bold">残り時間</div>
                        <div id="mashTimerDisplay" class="text-2xl sm:text-3xl font-black text-amber-400 mt-0.5">10.00秒</div>
                    </div>
                    <div class="bg-slate-950 p-3.5 rounded-2xl border border-slate-800">
                        <div class="text-xs text-slate-400 font-bold">連打スコア</div>
                        <div id="mashCountDisplay" class="text-2xl sm:text-3xl font-black text-pink-400 mt-0.5">0 回</div>
                    </div>
                </div>

                <button
                    type="button"
                    id="mashTapButton"
                    onclick="handleMashButtonTap()"
                    class="w-full py-12 rounded-2xl bg-gradient-to-r from-pink-600 via-rose-600 to-amber-500 active:scale-[0.98] text-white font-black text-xl sm:text-2xl shadow-xl shadow-pink-600/25 flex flex-col items-center justify-center gap-2 select-none transition"
                >
                    <span class="text-4xl">🥁</span>
                    <span id="mashBtnLabel">ここを連打でスタート！！</span>
                </button>
            </div>

            <!-- MINI-GAME 3: SHOGUNATE MEMORY FLIP (神経衰弱) -->
            <div id="mgPanel-memory" class="bg-gaming-card rounded-2xl border border-gaming-border p-5 sm:p-6 space-y-5 hidden">
                <div class="flex flex-wrap items-center justify-between gap-2">
                    <div>
                        <span class="text-[10px] font-black uppercase text-indigo-300 bg-indigo-500/20 px-2 py-0.5 rounded-full">GAME 03 • MEMORY MATCH</span>
                        <h3 class="text-lg font-black text-white mt-0.5">🃏 幕府絵札合わせ（神経衰弱・最速手数勝負）</h3>
                        <p class="text-xs text-slate-400">全6ペア（12枚）の絵札を何手で揃えられるか競います！手数が少ないほど上位になります。</p>
                    </div>
                    <div class="flex items-center gap-3">
                        <span class="text-xs font-bold text-slate-300 bg-slate-950 px-3 py-1.5 rounded-xl border border-slate-800">
                            現在の手数: <strong id="memoryMovesDisplay" class="text-emerald-400 text-sm">0</strong> 手
                        </span>
                        <button onclick="initMemoryGame()" class="px-3.5 py-1.5 rounded-xl bg-indigo-600 hover:bg-indigo-500 text-xs font-black text-white">
                            <i class="fa-solid fa-shuffle mr-1"></i>シャッフル再開
                        </button>
                    </div>
                </div>

                <div id="memoryCardsGrid" class="grid grid-cols-4 sm:grid-cols-6 gap-2.5">
                    <!-- Populated via JS -->
                </div>
            </div>

            <!-- MINI-GAME 4: BAKUDAN ROULETTE (BOMB DEFUSAL FOR 3 PLAYERS) -->
            <div id="mgPanel-bomb" class="bg-gaming-card rounded-2xl border border-gaming-border p-5 sm:p-6 space-y-5 hidden">
                <div class="flex flex-wrap items-center justify-between gap-2">
                    <div>
                        <span class="text-[10px] font-black uppercase text-rose-300 bg-rose-500/20 px-2 py-0.5 rounded-full">GAME 04 • PARTY SURVIVAL</span>
                        <h3 class="text-lg font-black text-white mt-0.5">💣 幕府爆弾回し（3人サバイバル危機一発）</h3>
                        <p class="text-xs text-slate-400">12個の導火線のうち、<strong>1つだけ大爆発するハズレ</strong>が潜んでいます！順番に選んで爆発させた人が今日の部屋立て・罰ゲーム！</p>
                    </div>
                    <button onclick="initBombGame()" class="px-4 py-2 rounded-xl bg-rose-600 hover:bg-rose-500 text-xs font-black text-white">
                        <i class="fa-solid fa-bomb mr-1"></i>新しい爆弾をセット
                    </button>
                </div>

                <div id="bombTurnBanner" class="bg-slate-950 border border-amber-500/40 rounded-xl p-3 text-center text-sm font-black text-amber-300">
                    順番に好きな番号をタップして導火線を切ってください！
                </div>

                <div id="bombWiresGrid" class="grid grid-cols-3 sm:grid-cols-4 gap-3">
                    <!-- Populated via JS -->
                </div>
            </div>
        </section>

        <!-- ==========================================
             TAB 3: BAKUFU WAR ROOM (ROULETTE, ROLES, SHOGUNATE RANKING, CHALLENGE OMIKUJI, MEMORIES, TREASURY)
             ========================================== -->
        <section id="view-party" class="space-y-6 hidden">
            <!-- NEW: 棒木幕府 家臣番付・戦績カウンター & 縛りプレイおみくじ -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
                <!-- 3人の戦績・キャリー・やらかし番付 -->
                <div class="lg:col-span-2 bg-gradient-to-br from-amber-950/40 via-gaming-card to-slate-950 rounded-2xl border border-amber-500/40 p-5 space-y-4">
                    <div class="flex flex-wrap items-center justify-between gap-2">
                        <div>
                            <span class="text-[10px] font-black uppercase text-amber-300 bg-amber-500/20 px-2 py-0.5 rounded-full">SHOGUNATE RANKING</span>
                            <h3 class="text-base sm:text-lg font-black text-white mt-0.5">👑 棒木幕府「家臣番付・戦績カウンター」</h3>
                            <p class="text-xs text-slate-400">普段のゲームでの「勝利・神キャリー・やらかし(トロール)」を記録して幕府内の役職を競おう！</p>
                        </div>
                    </div>
                    <div id="memberBattleStatsGrid" class="grid grid-cols-1 sm:grid-cols-3 gap-3">
                        <!-- Populated via JS -->
                    </div>
                </div>

                <!-- 縛りプレイ・罰ゲームおみくじ -->
                <div class="bg-gaming-card rounded-2xl border border-pink-500/30 p-5 flex flex-col justify-between gap-4">
                    <div>
                        <span class="text-[10px] font-black uppercase text-pink-300 bg-pink-500/20 px-2 py-0.5 rounded-full">CHALLENGE OMIKUJI</span>
                        <h3 class="text-base sm:text-lg font-black text-white mt-0.5">⛩️ 幕府の御触書（縛りプレイ＆お題くじ）</h3>
                        <p class="text-xs text-slate-400">いつものゲームに刺激を入れるランダムお題ガチャ！</p>
                    </div>

                    <div class="bg-slate-950 rounded-2xl border border-pink-500/30 p-4 text-center space-y-1.5 min-h-[104px] flex flex-col items-center justify-center">
                        <div id="omikujiBadge" class="text-[10px] font-black px-2.5 py-0.5 rounded-full bg-pink-500/20 text-pink-300">お題ボタンを押して抽選</div>
                        <div id="omikujiResultText" class="text-sm font-black text-white leading-relaxed">今日のお題・縛りルールは何が出るかな？</div>
                    </div>

                    <button onclick="drawChallengeOmikuji()" class="w-full py-3 rounded-xl bg-gradient-to-r from-pink-600 to-amber-500 hover:opacity-95 text-white font-black text-xs sm:text-sm shadow-lg shadow-pink-600/20 flex items-center justify-center gap-2 transition">
                        <i class="fa-solid fa-scroll"></i>
                        <span>御触書（お題くじ）を引く！</span>
                    </button>
                </div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- 1. Game Decision Roulette -->
                <div class="bg-gaming-card rounded-2xl border border-gaming-border p-5 flex flex-col justify-between gap-4">
                    <div class="flex items-center justify-between">
                        <div>
                            <span class="text-[10px] font-black uppercase text-pink-400 bg-pink-500/15 px-2 py-0.5 rounded-full">DECISION ROULETTE</span>
                            <h3 class="text-base sm:text-lg font-black text-white mt-0.5">🎰 今夜やるゲーム決定ルーレット</h3>
                            <p class="text-xs text-slate-400">迷った時は棒木幕府のルーレットにお任せ！</p>
                        </div>
                        <label class="flex items-center gap-1.5 text-xs text-slate-300 cursor-pointer bg-slate-900 px-2.5 py-1.5 rounded-xl border border-slate-800">
                            <input type="checkbox" id="rouletteOnlyHighVotes" checked class="rounded text-indigo-500 focus:ring-0">
                            <span>2票以上を優先</span>
                        </label>
                    </div>

                    <div class="bg-slate-950 rounded-2xl border border-indigo-500/30 p-4 flex items-center gap-4">
                        <img id="rouletteGameIcon" src="https://placehold.co/160x160/1e1b4b/a5b4fc?text=SPIN!" class="w-16 h-16 rounded-2xl object-cover border border-slate-700 shrink-0">
                        <div class="min-w-0 flex-1">
                            <div id="rouletteGameTitle" class="text-sm sm:text-base font-black text-white truncate">ボタンを押してルーレット回転！</div>
                            <div id="rouletteGameSub" class="text-xs text-slate-400 mt-0.5">投票ボードのタイトルからランダム抽選します</div>
                        </div>
                    </div>

                    <button onclick="spinGameRoulette()" id="spinRouletteBtn" class="w-full py-3 rounded-xl bg-gradient-to-r from-indigo-600 via-purple-600 to-pink-600 hover:opacity-95 text-white font-black text-xs sm:text-sm shadow-lg shadow-indigo-600/30 flex items-center justify-center gap-2 transition">
                        <i class="fa-solid fa-dice"></i>
                        <span>ルーレットを回す！</span>
                    </button>
                </div>

                <!-- 2. 3-Player Role / Host Shuffler -->
                <div class="bg-gaming-card rounded-2xl border border-gaming-border p-5 flex flex-col justify-between gap-4">
                    <div>
                        <span class="text-[10px] font-black uppercase text-amber-300 bg-amber-500/20 px-2 py-0.5 rounded-full">3-PLAYER SHUFFLE</span>
                        <h3 class="text-base sm:text-lg font-black text-white mt-0.5">🎲 3人の役割・部屋ホスト決めシャッフル</h3>
                        <p class="text-xs text-slate-400">3人のロール分担や、1対2のハンデ戦・部屋立て係をワンタップで抽選！</p>
                    </div>

                    <div id="roleShuffleResults" class="grid grid-cols-3 gap-2.5">
                        <!-- Rendered via JS -->
                    </div>

                    <div class="grid grid-cols-3 gap-2">
                        <button onclick="shuffleThreeRoles('rpg')" class="py-2.5 rounded-xl bg-slate-800 hover:bg-slate-700 text-xs font-bold text-slate-200 transition">
                            ⚔️ 前衛/タンク/支援
                        </button>
                        <button onclick="shuffleThreeRoles('host')" class="py-2.5 rounded-xl bg-slate-800 hover:bg-slate-700 text-xs font-bold text-slate-200 transition">
                            👑 部屋ホスト決め
                        </button>
                        <button onclick="shuffleThreeRoles('1v2')" class="py-2.5 rounded-xl bg-slate-800 hover:bg-slate-700 text-xs font-bold text-slate-200 transition">
                            😈 1対2 チーム分け
                        </button>
                    </div>
                </div>
            </div>

            <!-- 3. Party Memo / Discord & Server Code Quick Board -->
            <div class="bg-gaming-card rounded-2xl border border-gaming-border p-5 space-y-4">
                <div class="flex flex-wrap items-center justify-between gap-2">
                    <div>
                        <h3 class="text-base sm:text-lg font-black flex items-center gap-2">
                            <i class="fa-solid fa-clipboard-list text-emerald-400"></i>
                            <span>棒木幕府 軍議室＆共有メモ（部屋パス・目標・作戦）</span>
                        </h3>
                        <p class="text-xs text-slate-400">マルチプレイのサーバーパスワードや、次回の目標などを自由に書き込めます。</p>
                    </div>
                    <button onclick="saveSharedPartyNotes()" class="px-4 py-2 rounded-xl bg-emerald-500 hover:bg-emerald-400 text-slate-950 font-black text-xs flex items-center gap-1.5 transition">
                        <i class="fa-solid fa-floppy-disk"></i>
                        <span>メモを同期保存</span>
                    </button>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                    <div class="md:col-span-2">
                        <textarea
                            id="sharedPartyMemoInput"
                            rows="4"
                            placeholder="例: マイクラ統合版レルムコード: XXXX-YYYY / 次のモンハンは上位クエスト進めるぞ！ / 22時になったらDiscord集合！"
                            class="w-full p-3.5 rounded-xl bg-slate-950 border border-gaming-border focus:border-emerald-400 focus:outline-none text-sm text-slate-100"
                        ></textarea>
                    </div>
                    <div class="bg-slate-950 rounded-xl border border-gaming-border p-4 flex flex-col justify-between">
                        <div>
                            <div class="text-xs font-bold text-slate-400 mb-1">棒木幕府 累計評定（集会）カウント</div>
                            <div class="flex items-baseline gap-2">
                                <span id="sessionCounterValue" class="text-3xl font-black text-emerald-400">0</span>
                                <span class="text-xs text-slate-400">回 開催達成！</span>
                            </div>
                        </div>
                        <div class="flex items-center gap-2 mt-3">
                            <button onclick="incrementSessionCounter(1)" class="flex-1 py-2 rounded-xl bg-indigo-600 hover:bg-indigo-500 text-white font-bold text-xs transition">
                                🎉 今日も遊んだ！ (+1)
                            </button>
                            <button onclick="copySummaryForLineOrDiscord()" class="px-3 py-2 rounded-xl bg-slate-800 hover:bg-slate-700 text-slate-200 font-bold text-xs transition" title="予定サマリーをLINE/Discord用にコピー">
                                <i class="fa-regular fa-copy"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 4. 棒木幕府 戦果・神回年表 & 御用金（割り勘・立て替え帳） -->
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- 戦果・神回年表 (Hall of Memories) -->
                <div class="bg-gaming-card rounded-2xl border border-amber-500/30 p-5 space-y-4">
                    <div class="flex items-center justify-between">
                        <div>
                            <span class="text-[10px] font-black uppercase text-amber-300 bg-amber-500/20 px-2 py-0.5 rounded-full">HALL OF SHOGUNATE</span>
                            <h3 class="text-base sm:text-lg font-black text-white mt-0.5">📜 棒木幕府「戦果・神回年表」</h3>
                            <p class="text-xs text-slate-400">クリアしたゲームの記録や、腹筋崩壊した珍事件・MVPを残せます。</p>
                        </div>
                    </div>
                    <div class="flex flex-col sm:flex-row gap-2">
                        <input type="text" id="newMemoryTextInput" placeholder="例: オーバークック2全ステージ星3クリア！ / ケンが溶岩ダイブ事件" class="flex-1 px-3 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-white">
                        <select id="newMemoryMvpSelect" class="px-2.5 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-amber-300 font-bold">
                            <!-- Populated via JS -->
                        </select>
                        <button onclick="addBakufuMemory()" class="px-4 py-2 rounded-xl bg-amber-500 hover:bg-amber-400 text-slate-950 font-black text-xs shrink-0 transition">
                            年表に刻む
                        </button>
                    </div>
                    <div id="bakufuMemoriesList" class="space-y-2 max-h-56 overflow-y-auto pr-1">
                        <!-- Rendered via JS -->
                    </div>
                </div>

                <!-- 御用金・立て替え帳 (Split Expense Ledger) -->
                <div class="bg-gaming-card rounded-2xl border border-emerald-500/30 p-5 space-y-4">
                    <div>
                        <span class="text-[10px] font-black uppercase text-emerald-300 bg-emerald-500/20 px-2 py-0.5 rounded-full">SHOGUNATE TREASURY</span>
                        <h3 class="text-base sm:text-lg font-black text-white mt-0.5">💰 幕府の御用金（サーバー代・まとめ買い立て替え帳）</h3>
                        <p class="text-xs text-slate-400">マルチサーバー代やDLC・オフ会などのちょっとした貸し借りメモ。</p>
                    </div>
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-2">
                        <input type="text" id="newExpenseTitleInput" placeholder="項目 (例: マイクラRealms代)" class="sm:col-span-2 px-3 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-white">
                        <input type="number" id="newExpenseAmountInput" placeholder="金額 (円)" class="px-3 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-white">
                    </div>
                    <div class="flex items-center justify-between gap-2">
                        <span class="text-[11px] text-slate-400">立て替えた人: 現在操作中のメンバーで記録されます</span>
                        <button onclick="addBakufuExpense()" class="px-4 py-2 rounded-xl bg-emerald-500 hover:bg-emerald-400 text-slate-950 font-black text-xs shrink-0 transition">
                            ＋ 御用金に記録
                        </button>
                    </div>
                    <div id="bakufuExpensesList" class="space-y-2 max-h-48 overflow-y-auto pr-1">
                        <!-- Rendered via JS -->
                    </div>
                </div>
            </div>
        </section>

        <!-- ==========================================
             TAB 4: DISCORD WEBHOOK & FREE iOS APP / PWA GUIDE
             ========================================== -->
        <section id="view-appguide" class="space-y-6 hidden">
            <!-- Discord Auto-Notification Panel (3人の予定が合った時だけ自動通知) -->
            <div class="bg-gradient-to-br from-[#5865F2]/25 via-gaming-card to-slate-950 rounded-2xl border border-[#5865F2]/50 p-5 sm:p-6 space-y-4 shadow-xl">
                <div class="flex flex-wrap items-center justify-between gap-3">
                    <div>
                        <span class="inline-flex items-center gap-1.5 text-xs font-black text-indigo-200 bg-[#5865F2]/30 px-3 py-1 rounded-full border border-[#5865F2]/50">
                            <i class="fa-brands fa-discord"></i> 棒木幕府・Discord自動伝令システム
                        </span>
                        <h3 class="text-lg sm:text-xl font-black text-white mt-1.5">
                            🔔 3人の予定が合った時だけDiscordへ自動通知！
                        </h3>
                        <p class="text-xs text-slate-300 mt-0.5">
                            1人・2人が入力した段階や「×」の日は通知せず、<strong>3人全員が「◯」または「△」で揃った瞬間だけ</strong>普段のDiscordチャンネルへ自動で集合伝令を飛ばします。
                        </p>
                    </div>
                    <button onclick="openDiscordSettingsModal()" class="px-5 py-3 rounded-xl bg-[#5865F2] hover:bg-[#4752C4] text-white font-black text-xs sm:text-sm shadow-lg shadow-[#5865F2]/30 flex items-center gap-2 transition">
                        <i class="fa-solid fa-gear"></i>
                        <span>Discord Webhookを設定する</span>
                    </button>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-3 gap-3 text-xs">
                    <div class="bg-slate-950/80 p-3.5 rounded-xl border border-slate-800 space-y-1">
                        <div class="font-black text-emerald-400"><i class="fa-solid fa-filter mr-1"></i>スパムゼロの厳密判定</div>
                        <p class="text-slate-400 text-[11px]">3人全員が「◯（全員◯）」または「◯＋△（3人集合可）」になった日のみ自動送信します。</p>
                    </div>
                    <div class="bg-slate-950/80 p-3.5 rounded-xl border border-slate-800 space-y-1">
                        <div class="font-black text-amber-400"><i class="fa-solid fa-gamepad mr-1"></i>遊ぶゲーム＆時間も通知</div>
                        <p class="text-slate-400 text-[11px]">その日に設定したゲームタイトル（アイコン付）や集合時間、3人の内訳をカード形式で綺麗に通知します。</p>
                    </div>
                    <div class="bg-slate-950/80 p-3.5 rounded-xl border border-slate-800 space-y-1">
                        <div class="font-black text-sky-400"><i class="fa-solid fa-cloud-arrow-up mr-1"></i>1人が設定すれば3人全員に適用</div>
                        <p class="text-slate-400 text-[11px]">Webhook URLはクラウド同期されるため、代表者1人が設定するだけで誰が3人目の「◯」を押しても通知が飛びます。</p>
                    </div>
                </div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Immediate Free iPhone Home Screen App Guide -->
                <div class="bg-gaming-card rounded-2xl border border-emerald-500/40 p-5 space-y-4">
                    <div class="inline-flex items-center gap-1.5 text-xs font-black text-emerald-300 bg-emerald-500/20 px-2.5 py-1 rounded-full">
                        <i class="fa-solid fa-mobile-screen-button"></i> 完全無料・今すぐiPhoneアプリ化 (PWA)
                    </div>
                    <h3 class="text-lg font-black text-white">3人のiPhoneのホーム画面にアイコンを追加する方法</h3>
                    <p class="text-xs text-slate-300 leading-relaxed">
                        Appleの年間登録料（約15,000円）を払わなくても、このサイトを<strong>iPhoneの「ホーム画面に追加」</strong>するだけで、アドレスバーが消えてフルスクリーンのネイティブアプリとして動きます！
                    </p>
                    <ol class="space-y-2.5 text-xs text-slate-200 bg-slate-950 p-4 rounded-xl border border-slate-800">
                        <li class="flex items-start gap-2.5">
                            <span class="w-5 h-5 rounded-full bg-indigo-600 text-white font-black flex items-center justify-center shrink-0">1</span>
                            <span>URLをLINEやDiscordで<strong>友達2人に送る</strong></span>
                        </li>
                        <li class="flex items-start gap-2.5">
                            <span class="w-5 h-5 rounded-full bg-indigo-600 text-white font-black flex items-center justify-center shrink-0">2</span>
                            <span>Safariの下部にある<strong>「共有ボタン（四角から上矢印）」</strong>をタップ</span>
                        </li>
                        <li class="flex items-start gap-2.5">
                            <span class="w-5 h-5 rounded-full bg-indigo-600 text-white font-black flex items-center justify-center shrink-0">3</span>
                            <span><strong>「ホーム画面に追加」</strong>をタップすると、専用アイコンでいつでもワンタップ起動！</span>
                        </li>
                    </ol>
                    <button onclick="copySummaryForLineOrDiscord()" class="w-full py-3 rounded-xl bg-emerald-500 hover:bg-emerald-400 text-slate-950 font-black text-xs flex items-center justify-center gap-2 transition">
                        <i class="fa-solid fa-share-nodes"></i>
                        <span>LINE / Discord共有用テキストをコピー</span>
                    </button>
                </div>

                <!-- Step-by-Step Hosting & Cloud Sync Guide -->
                <div class="bg-gaming-card rounded-2xl border border-amber-500/40 p-5 space-y-4">
                    <div class="inline-flex items-center gap-1.5 text-xs font-black text-amber-300 bg-amber-500/20 px-2.5 py-1 rounded-full">
                        <i class="fa-solid fa-rocket"></i> どこでどうやって動かす？（無料公開＆3人同期ガイド）
                    </div>
                    <h3 class="text-lg font-black text-white">最短3分でネット公開して3人で共有する手順</h3>
                    <div class="space-y-2.5 text-xs text-slate-200 bg-slate-950 p-4 rounded-xl border border-slate-800">
                        <div class="space-y-1">
                            <div class="font-black text-amber-400">方法A：今この画面のプレビューでそのまま試す</div>
                            <p class="text-slate-400 text-[11px]">画面右上の「Preview（プレビュー）」ボタンを押すだけで、今すぐこの場ですべての機能が動きます！</p>
                        </div>
                        <div class="space-y-1 pt-2 border-t border-slate-800">
                            <div class="font-black text-emerald-400">方法B：無料で専用URLを作って友達2人に送る（おすすめ！）</div>
                            <p class="text-slate-400 text-[11px]">
                                1. このコードを <strong><code>index.html</code></strong> という名前で保存します。<br>
                                2. 無料サイト公開サービス <strong>Netlify Drop (app.netlify.com/drop)</strong> または <strong>GitHub Pages / Vercel</strong> にドラッグ＆ドロップするだけで、世界に1つの専用URL（<code>https://bouki-bakufu.netlify.app</code> など）が無料で発行されます！
                            </p>
                        </div>
                        <div class="space-y-1 pt-2 border-t border-slate-800">
                            <div class="font-black text-indigo-300">方法C：外部サイトで3人リアルタイム同期を使う設定</div>
                            <p class="text-slate-400 text-[11px]">
                                外部サーバーで3人のデータをリアルタイム同期するには、無料の <strong>Firebase Console</strong> でプロジェクトを作成し、下のボタンから <code>firebaseConfig</code> を1回貼り付けるだけでOKです。
                            </p>
                        </div>
                    </div>
                    <button onclick="openCustomFirebaseModal()" class="w-full py-2.5 rounded-xl bg-indigo-600/30 hover:bg-indigo-600/50 border border-indigo-400/50 text-indigo-200 font-black text-xs flex items-center justify-center gap-2 transition">
                        <i class="fa-solid fa-database"></i>
                        <span>外部公開用のFirebase同期キーを設定・確認する</span>
                    </button>
                </div>
            </div>
        </section>

    </main>

    <!-- MOBILE BOTTOM NAVIGATION BAR -->
    <nav class="md:hidden fixed bottom-0 left-0 right-0 z-30 glass-panel border-t border-gaming-border px-2 py-1.5">
        <div class="grid grid-cols-5 gap-1 max-w-md mx-auto">
            <button onclick="switchTab('calendar')" id="mobTab-calendar" class="flex flex-col items-center justify-center py-1.5 rounded-xl text-indigo-400 bg-indigo-500/15 font-bold">
                <i class="fa-regular fa-calendar-check text-base"></i>
                <span class="text-[10px] mt-0.5">評定予定</span>
            </button>
            <button onclick="switchTab('games')" id="mobTab-games" class="flex flex-col items-center justify-center py-1.5 rounded-xl text-slate-400 font-bold">
                <i class="fa-solid fa-fire-flame-curved text-base"></i>
                <span class="text-[10px] mt-0.5">ゲーム投票</span>
            </button>
            <button onclick="switchTab('arcade')" id="mobTab-arcade" class="flex flex-col items-center justify-center py-1.5 rounded-xl text-slate-400 font-bold">
                <i class="fa-solid fa-gamepad text-base"></i>
                <span class="text-[10px] mt-0.5">遊戯場</span>
            </button>
            <button onclick="switchTab('party')" id="mobTab-party" class="flex flex-col items-center justify-center py-1.5 rounded-xl text-slate-400 font-bold">
                <i class="fa-solid fa-scroll text-base"></i>
                <span class="text-[10px] mt-0.5">軍議・番付</span>
            </button>
            <button onclick="switchTab('appguide')" id="mobTab-appguide" class="flex flex-col items-center justify-center py-1.5 rounded-xl text-slate-400 font-bold">
                <i class="fa-brands fa-discord text-base"></i>
                <span class="text-[10px] mt-0.5">伝令・設定</span>
            </button>
        </div>
    </nav>

    <!-- ==========================================
         MODAL 1: DAY SCHEDULE EDITOR (3 MEMBERS + TARGET GAME)
         ========================================== -->
    <div id="dayModal" class="fixed inset-0 z-50 bg-slate-950/80 backdrop-blur-sm hidden items-center justify-center p-4">
        <div class="bg-gaming-card border border-gaming-border rounded-2xl max-w-lg w-full p-5 space-y-4 shadow-2xl animate-fade-in">
            <div class="flex items-center justify-between border-b border-slate-800 pb-3">
                <div>
                    <span id="modalDateMatchBadge" class="text-[10px] font-black px-2 py-0.5 rounded-full bg-slate-800 text-slate-300">SCHEDULE</span>
                    <h3 id="modalDateTitle" class="text-lg font-black text-white mt-0.5">5月10日 (土) の予定</h3>
                </div>
                <button onclick="closeDayModal()" class="w-8 h-8 rounded-xl bg-slate-800 hover:bg-slate-700 text-slate-300 flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>

            <!-- 3 Members' Availability Rows -->
            <div id="modalMembersScheduleList" class="space-y-3">
                <!-- Populated dynamically via JS for all 3 members -->
            </div>

            <!-- Day's Target Game, "Other" Choices & Quick Online Search -->
            <div class="bg-slate-900/90 p-3.5 rounded-xl border border-slate-800 space-y-3">
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                    <div>
                        <div class="flex items-center justify-between mb-1">
                            <label class="block text-xs font-bold text-slate-300">
                                <i class="fa-solid fa-gamepad text-pink-400 mr-1"></i>この日に遊ぶゲーム・予定内容
                            </label>
                            <button type="button" onclick="toggleModalInlineGameAdder()" class="text-[11px] font-bold text-indigo-400 hover:text-indigo-300">
                                <i class="fa-solid fa-plus-circle mr-0.5"></i>新規ゲーム追加
                            </button>
                        </div>
                        <select id="modalDayGameSelect" onchange="handleModalGameSelectChange(this.value)" class="w-full px-3 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-white focus:outline-none">
                            <option value="">未定（投票リスト・その他から選択）</option>
                        </select>
                    </div>
                    <div>
                        <label class="block text-xs font-bold text-slate-300 mb-1">
                            <i class="fa-regular fa-clock text-emerald-400 mr-1"></i>集合時間の目安・一言
                        </label>
                        <input type="text" id="modalDayTimeInput" placeholder="例: 21:00〜 / 22:30頃Discord" class="w-full px-3 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-white focus:outline-none">
                    </div>
                </div>

                <!-- Quick "Other / Flexible" 1-Tap Chips inside Calendar Modal -->
                <div class="flex items-center gap-1.5 flex-wrap pt-1 border-t border-slate-800/80">
                    <span class="text-[10px] text-slate-400"><i class="fa-solid fa-wand-magic-sparkles text-amber-400 mr-1"></i>その他の選択肢をセット:</span>
                    <button type="button" onclick="selectOrAddOtherOptionInModal('opt_decide_later', '🎲 当日ルーレット・ノリで決める', 'その他')" class="px-2 py-1 rounded-lg bg-slate-950 hover:bg-indigo-950 text-[11px] text-amber-300 border border-amber-500/30 transition">
                        🎲 当日決める
                    </button>
                    <button type="button" onclick="selectOrAddOtherOptionInModal('opt_vc_chat', '💬 雑談・作業通話・画面共有', 'その他')" class="px-2 py-1 rounded-lg bg-slate-950 hover:bg-indigo-950 text-[11px] text-sky-300 border border-sky-500/30 transition">
                        💬 雑談・画面共有
                    </button>
                    <button type="button" onclick="selectOrAddOtherOptionInModal('opt_game_hunt', '🛒 新作ゲーム探し・セール巡り', 'その他')" class="px-2 py-1 rounded-lg bg-slate-950 hover:bg-indigo-950 text-[11px] text-emerald-300 border border-emerald-500/30 transition">
                        🛒 新作探し
                    </button>
                    <button type="button" onclick="selectOrAddOtherOptionInModal('opt_watch_party', '🎬 ウォッチパーティ・動画鑑賞', 'その他')" class="px-2 py-1 rounded-lg bg-slate-950 hover:bg-indigo-950 text-[11px] text-pink-300 border border-pink-500/30 transition">
                        🎬 動画・配信鑑賞
                    </button>
                </div>

                <!-- Inline Mini Online Game Finder inside Day Modal -->
                <div id="modalInlineGameAdder" class="hidden pt-2 border-t border-slate-800 space-y-2">
                    <div class="text-[11px] font-bold text-indigo-300">ネットからアイコン検索してそのままこの日の予定に登録：</div>
                    <div class="flex gap-1.5">
                        <input type="text" id="modalInlineSearchInput" placeholder="ゲーム名を入力 (例: スプラ, スト6, マイクラ)..." onkeydown="if(event.key==='Enter') searchInlineForDayModal()" class="flex-1 px-2.5 py-1.5 rounded-lg bg-slate-950 border border-slate-700 text-xs text-white">
                        <button type="button" onclick="searchInlineForDayModal()" class="px-3 py-1.5 rounded-lg bg-indigo-600 hover:bg-indigo-500 text-white text-xs font-bold shrink-0">
                            検索
                        </button>
                    </div>
                    <div id="modalInlineSearchResults" class="grid grid-cols-1 sm:grid-cols-2 gap-1.5 max-h-36 overflow-y-auto"></div>
                </div>
            </div>

            <!-- Discord Match Re-Notify Row (Visible ONLY when all 3 members match on this day) -->
            <div id="modalDiscordMatchedNotice" class="hidden bg-[#5865F2]/15 border border-[#5865F2]/40 rounded-xl p-3 flex flex-wrap items-center justify-between gap-2">
                <div class="text-xs text-indigo-200 flex items-center gap-2">
                    <i class="fa-brands fa-discord text-[#5865F2] text-base"></i>
                    <span id="modalDiscordMatchedStatusText">3人の予定が合っています！保存時にDiscordへ自動通知されます。</span>
                </div>
                <button type="button" onclick="manualSendDiscordForEditingDay()" class="px-3 py-1.5 rounded-lg bg-[#5865F2] hover:bg-[#4752C4] text-white text-[11px] font-black flex items-center gap-1 transition">
                    <i class="fa-solid fa-paper-plane"></i>
                    <span>📣 今すぐDiscordへ再通知</span>
                </button>
            </div>

            <div class="flex items-center justify-end gap-2 pt-2">
                <button onclick="closeDayModal()" class="px-4 py-2 rounded-xl bg-slate-800 hover:bg-slate-700 text-xs font-bold text-slate-300">
                    キャンセル
                </button>
                <button onclick="saveDayModalChanges()" class="px-5 py-2 rounded-xl bg-indigo-600 hover:bg-indigo-500 text-xs font-black text-white shadow-lg shadow-indigo-600/30">
                    保存して同期
                </button>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MODAL 2: INITIAL ONBOARDING & PROFILE REGISTRATION MODAL
         ========================================== -->
    <div id="onboardingModal" class="fixed inset-0 z-50 bg-slate-950/85 backdrop-blur-md hidden items-center justify-center p-4 overflow-y-auto">
        <div class="bg-gaming-card border-2 border-amber-500/50 rounded-3xl max-w-xl w-full p-5 sm:p-6 space-y-5 shadow-2xl my-auto">
            <div class="flex items-start justify-between gap-3 border-b border-slate-800 pb-3.5">
                <div class="flex items-center gap-3">
                    <div class="w-11 h-11 rounded-2xl bg-gradient-to-br from-amber-500 to-indigo-600 flex items-center justify-center text-white text-xl shadow-lg">
                        <i class="fa-solid fa-torii-gate"></i>
                    </div>
                    <div>
                        <span class="text-[10px] font-black uppercase tracking-wider text-amber-300 bg-amber-500/20 px-2 py-0.5 rounded-full">
                            WELCOME TO BOUKI BAKUFU
                        </span>
                        <h3 class="text-base sm:text-lg font-black text-white mt-0.5">棒木幕府・家臣（メンバー）初期登録</h3>
                        <p class="text-xs text-slate-400">自分の枠を選んで、アイコンと名前を登録してください</p>
                    </div>
                </div>
                <button onclick="closeOnboardingModal()" class="w-8 h-8 rounded-xl bg-slate-800 hover:bg-slate-700 text-slate-300 flex items-center justify-center shrink-0">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>

            <!-- STEP 1: Choose Slot -->
            <div class="space-y-2">
                <label class="block text-xs font-black text-amber-300">STEP 1. あなたのプレイヤー枠を選択</label>
                <div id="onboardingSlotGrid" class="grid grid-cols-3 gap-2.5">
                    <!-- Rendered dynamically via JS -->
                </div>
            </div>

            <!-- STEP 2: Name & Status -->
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                <div>
                    <label class="block text-xs font-bold text-slate-300 mb-1">STEP 2. あなたの名前（ニックネーム）</label>
                    <input
                        type="text"
                        id="onboardingNameInput"
                        oninput="updateOnboardingPreview()"
                        placeholder="例: タロウ / 将軍"
                        class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-700 focus:border-amber-400 focus:outline-none text-xs sm:text-sm text-white font-bold"
                    >
                </div>
                <div>
                    <label class="block text-xs font-bold text-slate-300 mb-1">一言ステータス（任意）</label>
                    <input
                        type="text"
                        id="onboardingStatusInput"
                        placeholder="例: 21時以降なら毎日OK！"
                        class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-700 focus:border-amber-400 focus:outline-none text-xs sm:text-sm text-white"
                    >
                </div>
            </div>

            <!-- STEP 3: Avatar Picker & Image Upload -->
            <div class="space-y-2.5">
                <div class="flex flex-wrap items-center justify-between gap-2">
                    <label class="text-xs font-bold text-slate-300">STEP 3. メンバーアイコンを選択</label>
                    <label class="px-3 py-1.5 rounded-xl bg-indigo-600/30 hover:bg-indigo-600/50 border border-indigo-400/50 text-indigo-200 text-[11px] font-black cursor-pointer flex items-center gap-1.5 transition">
                        <i class="fa-solid fa-image"></i>
                        <span>スマホ・PCから画像を選択</span>
                        <input type="file" accept="image/*" onchange="handleAvatarFileUpload(event)" class="hidden">
                    </label>
                </div>

                <!-- Live Preview + Emoji Grid -->
                <div class="flex flex-col sm:flex-row items-center gap-3 bg-slate-950/90 p-3 rounded-2xl border border-slate-800">
                    <div class="flex flex-col items-center justify-center px-3 py-2 bg-slate-900 rounded-xl border border-slate-800 shrink-0 min-w-[100px]">
                        <div id="onboardingAvatarPreviewBox" class="w-14 h-14 rounded-full flex items-center justify-center text-3xl">🐉</div>
                        <span id="onboardingNamePreviewText" class="text-[11px] font-black text-amber-300 mt-1 truncate max-w-[90px]">自分</span>
                    </div>
                    <div id="onboardingEmojiPalette" class="grid grid-cols-8 gap-1.5 flex-1 w-full max-h-36 overflow-y-auto p-1">
                        <!-- Populated via JS -->
                    </div>
                </div>
            </div>

            <div class="flex items-center justify-between gap-3 pt-2 border-t border-slate-800">
                <button type="button" onclick="openMemberSettingsModal(); closeOnboardingModal();" class="text-xs text-slate-400 hover:text-slate-200 underline">
                    3人分まとめて名前を編集する
                </button>
                <button type="button" onclick="completeOnboardingRegistration()" class="px-6 py-3 rounded-xl bg-gradient-to-r from-amber-500 to-indigo-600 hover:opacity-95 text-white font-black text-xs sm:text-sm shadow-lg shadow-amber-500/20 flex items-center gap-2 transition">
                    <i class="fa-solid fa-check"></i>
                    <span>このプロフィールで始める！</span>
                </button>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MODAL 3: 3-MEMBER BULK PROFILE SETTINGS
         ========================================== -->
    <div id="memberSettingsModal" class="fixed inset-0 z-50 bg-slate-950/80 backdrop-blur-sm hidden items-center justify-center p-4">
        <div class="bg-gaming-card border border-gaming-border rounded-2xl max-w-md w-full p-5 space-y-4 shadow-2xl">
            <div class="flex items-center justify-between border-b border-slate-800 pb-3">
                <h3 class="text-base font-black text-white">3人のメンバー名・アイコン一括設定</h3>
                <button onclick="closeMemberSettingsModal()" class="w-8 h-8 rounded-xl bg-slate-800 text-slate-300 flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div id="memberEditInputs" class="space-y-2.5"></div>
            <div class="flex justify-end gap-2 pt-2">
                <button onclick="closeMemberSettingsModal()" class="px-4 py-2 rounded-xl bg-slate-800 text-xs font-bold text-slate-300">閉じる</button>
                <button onclick="saveMemberProfiles()" class="px-5 py-2 rounded-xl bg-indigo-600 text-xs font-black text-white">保存する</button>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MODAL 4: QUICK STATUS MESSAGE UPDATE
         ========================================== -->
    <div id="statusUpdateModal" class="fixed inset-0 z-50 bg-slate-950/80 backdrop-blur-sm hidden items-center justify-center p-4">
        <div class="bg-gaming-card border border-gaming-border rounded-2xl max-w-md w-full p-5 space-y-4 shadow-2xl">
            <div class="flex items-center justify-between border-b border-slate-800 pb-3">
                <h3 id="statusModalMemberLabel" class="text-base font-black text-white">一言ステータスの更新</h3>
                <button onclick="closeStatusUpdateModal()" class="w-8 h-8 rounded-xl bg-slate-800 text-slate-300 flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <input type="text" id="statusMessageInput" placeholder="例: 今夜21時からいける！" class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-700 text-xs sm:text-sm text-white">
            <div class="flex flex-wrap gap-1.5">
                <button type="button" onclick="setQuickStatusText('🟢 今すぐ遊べる！')" class="px-2.5 py-1 rounded-lg bg-slate-900 text-xs text-emerald-300 border border-slate-800">🟢 今すぐ遊べる！</button>
                <button type="button" onclick="setQuickStatusText('🔥 21時以降ならOK！')" class="px-2.5 py-1 rounded-lg bg-slate-900 text-xs text-amber-300 border border-slate-800">🔥 21時以降ならOK！</button>
                <button type="button" onclick="setQuickStatusText('♨️ 風呂・飯いってくる')" class="px-2.5 py-1 rounded-lg bg-slate-900 text-xs text-sky-300 border border-slate-800">♨️ 風呂・飯いってくる</button>
            </div>
            <div class="flex justify-end gap-2 pt-2">
                <button onclick="closeStatusUpdateModal()" class="px-4 py-2 rounded-xl bg-slate-800 text-xs font-bold text-slate-300">キャンセル</button>
                <button onclick="saveStatusMessage()" class="px-5 py-2 rounded-xl bg-indigo-600 text-xs font-black text-white">更新する</button>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MODAL 5: CUSTOM GAME / OTHER ACTIVITY ADD MODAL
         ========================================== -->
    <div id="customGameModal" class="fixed inset-0 z-50 bg-slate-950/80 backdrop-blur-sm hidden items-center justify-center p-4">
        <div class="bg-gaming-card border border-gaming-border rounded-2xl max-w-md w-full p-5 space-y-4 shadow-2xl">
            <div class="flex items-center justify-between border-b border-slate-800 pb-3">
                <h3 class="text-base font-black text-white">自由入力・その他の選択肢を追加</h3>
                <button onclick="closeCustomGameModal()" class="w-8 h-8 rounded-xl bg-slate-800 text-slate-300 flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div class="space-y-3">
                <div>
                    <label class="block text-xs font-bold text-slate-300 mb-1">ゲーム名 または 予定タイトル</label>
                    <div class="flex gap-1.5">
                        <input type="text" id="customGameTitleInput" placeholder="例: スト6 / 雑談ボイチャ / 新作探し" class="flex-1 px-3 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-white">
                        <button type="button" onclick="fetchIconForCustomModal()" class="px-3 py-2 rounded-xl bg-indigo-600/30 border border-indigo-400/40 text-indigo-200 text-xs font-bold shrink-0">
                            アイコン検索
                        </button>
                    </div>
                </div>
                <div id="customModalIconCandidates" class="hidden space-y-1">
                    <div class="text-[11px] text-slate-400">タップしてアイコンをセット:</div>
                    <div id="customModalIconGrid" class="flex items-center gap-2 overflow-x-auto py-1"></div>
                </div>
                <div class="grid grid-cols-2 gap-2">
                    <div>
                        <label class="block text-xs font-bold text-slate-300 mb-1">機種・カテゴリ</label>
                        <select id="customGamePlatformInput" class="w-full px-3 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-white">
                            <option value="Crossplay">🌐 クロスプレイ</option>
                            <option value="Switch">🎮 Switch</option>
                            <option value="PC">💻 PC (Steam)</option>
                            <option value="PS5">🕹️ PS5 / PS4</option>
                            <option value="Mobile">📱 スマホ</option>
                            <option value="その他">🎲 その他・自由枠</option>
                        </select>
                    </div>
                    <div>
                        <label class="block text-xs font-bold text-slate-300 mb-1">現在の状態</label>
                        <select id="customGameStatusInput" class="w-full px-3 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-white">
                            <option value="want">🌱 やりたい候補</option>
                            <option value="playing">🎮 いま遊んでる</option>
                            <option value="cleared">🏆 殿堂入り・休止</option>
                        </select>
                    </div>
                </div>
                <div>
                    <label class="block text-xs font-bold text-slate-300 mb-1">アイコン画像URL（空欄でも自動生成されます）</label>
                    <input type="text" id="customGameImageInput" placeholder="https://..." class="w-full px-3 py-2 rounded-xl bg-slate-950 border border-slate-700 text-xs text-white">
                </div>
            </div>
            <div class="flex justify-end gap-2 pt-2">
                <button onclick="closeCustomGameModal()" class="px-4 py-2 rounded-xl bg-slate-800 text-xs font-bold text-slate-300">キャンセル</button>
                <button onclick="addCustomGameToBoard()" class="px-5 py-2 rounded-xl bg-indigo-600 text-xs font-black text-white">リストに追加</button>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MODAL 6: DISCORD WEBHOOK SETTINGS MODAL (3人一致時のみ自動通知)
         ========================================== -->
    <div id="discordSettingsModal" class="fixed inset-0 z-50 bg-slate-950/85 backdrop-blur-md hidden items-center justify-center p-4 overflow-y-auto">
        <div class="bg-gaming-card border-2 border-[#5865F2]/60 rounded-3xl max-w-lg w-full p-5 sm:p-6 space-y-5 shadow-2xl my-auto">
            <div class="flex items-start justify-between gap-3 border-b border-slate-800 pb-3.5">
                <div class="flex items-center gap-3">
                    <div class="w-11 h-11 rounded-2xl bg-[#5865F2] flex items-center justify-center text-white text-xl shadow-lg shadow-[#5865F2]/40 shrink-0">
                        <i class="fa-brands fa-discord"></i>
                    </div>
                    <div>
                        <span class="text-[10px] font-black uppercase tracking-wider text-indigo-300 bg-[#5865F2]/25 px-2 py-0.5 rounded-full">
                            3-PLAYER MATCH AUTO WEBHOOK
                        </span>
                        <h3 class="text-base sm:text-lg font-black text-white mt-0.5">棒木幕府・Discord自動伝令設定</h3>
                        <p class="text-xs text-slate-400">3人全員の予定が合った（◯または△で揃った）ときだけ通知します</p>
                    </div>
                </div>
                <button onclick="closeDiscordSettingsModal()" class="w-8 h-8 rounded-xl bg-slate-800 hover:bg-slate-700 text-slate-300 flex items-center justify-center shrink-0">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>

            <div class="space-y-4">
                <!-- Enable Toggle -->
                <label class="flex items-center justify-between p-3.5 rounded-2xl bg-slate-950 border border-slate-800 cursor-pointer">
                    <div>
                        <div class="text-xs sm:text-sm font-black text-white">3人の予定一致時のDiscord自動通知</div>
                        <div class="text-[11px] text-slate-400">ONにすると、3人目の予定（◯/△）が揃った瞬間に自動で伝令を送ります</div>
                    </div>
                    <input type="checkbox" id="discordAutoNotifyToggle" checked class="w-5 h-5 rounded bg-slate-900 border-slate-700 text-[#5865F2] focus:ring-0">
                </label>

                <!-- Webhook URL Input -->
                <div>
                    <label class="block text-xs font-bold text-slate-300 mb-1.5">
                        <i class="fa-solid fa-link text-[#5865F2] mr-1"></i>Discord Webhook URL
                    </label>
                    <input
                        type="url"
                        id="discordWebhookUrlInput"
                        placeholder="https://discord.com/api/webhooks/..."
                        class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-700 focus:border-[#5865F2] focus:outline-none text-xs sm:text-sm text-white"
                    >
                    <p class="text-[11px] text-slate-400 mt-1.5">
                        Discordの「チャンネルの編集 ⚙️」➔「連携サービス」➔「ウェブフック」からURLをコピーして貼り付けてください。
                    </p>
                </div>
            </div>

            <div class="flex flex-wrap items-center justify-between gap-2 pt-2 border-t border-slate-800">
                <button type="button" id="testDiscordWebhookBtn" onclick="sendTestDiscordWebhook()" class="px-3.5 py-2 rounded-xl bg-slate-800 hover:bg-slate-700 text-indigo-300 text-xs font-bold flex items-center gap-1.5 transition">
                    <i class="fa-solid fa-paper-plane"></i>
                    <span>テスト伝令を送る</span>
                </button>
                <div class="flex items-center gap-2">
                    <button type="button" onclick="closeDiscordSettingsModal()" class="px-4 py-2 rounded-xl bg-slate-800 text-xs font-bold text-slate-300">キャンセル</button>
                    <button type="button" onclick="saveDiscordWebhookSettings()" class="px-5 py-2.5 rounded-xl bg-[#5865F2] hover:bg-[#4752C4] text-xs font-black text-white shadow-lg shadow-[#5865F2]/30">設定を保存して同期</button>
                </div>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MODAL 7: EXTERNAL HOSTING FIREBASE CONFIG HELPER MODAL
         ========================================== -->
    <div id="customFirebaseModal" class="fixed inset-0 z-50 bg-slate-950/85 backdrop-blur-md hidden items-center justify-center p-4 overflow-y-auto">
        <div class="bg-gaming-card border-2 border-indigo-500/60 rounded-3xl max-w-lg w-full p-5 sm:p-6 space-y-4 shadow-2xl my-auto">
            <div class="flex items-start justify-between gap-3 border-b border-slate-800 pb-3">
                <div>
                    <span class="text-[10px] font-black uppercase text-indigo-300 bg-indigo-500/20 px-2 py-0.5 rounded-full">EXTERNAL HOSTING SETUP</span>
                    <h3 class="text-base sm:text-lg font-black text-white mt-0.5">外部サイト公開時の3人リアルタイム同期ガイド</h3>
                </div>
                <button onclick="closeCustomFirebaseModal()" class="w-8 h-8 rounded-xl bg-slate-800 text-slate-300 flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div class="space-y-3 text-xs text-slate-300 leading-relaxed">
                <p>
                    このプレビュー画面内ではすでに<strong>自動でクラウド同期が稼働</strong>していますが、自分で <strong>GitHub Pages / Netlify / Vercel</strong> などに <code>index.html</code> をアップロードして使う場合は、無料のFirebaseプロジェクトを1つ繋ぐだけで3人同期が動きます。
                </p>
                <ol class="list-decimal list-inside space-y-1.5 bg-slate-950 p-3.5 rounded-xl border border-slate-800 text-[11px]">
                    <li><a href="https://console.firebase.google.com/" target="_blank" class="text-indigo-400 underline">Firebase Console</a>（無料）で新規プロジェクトを作成</li>
                    <li>「Authentication」➔「Sign-in method」で<strong>「匿名（Anonymous）」</strong>を有効化</li>
                    <li>「Firestore Database」を作成し、プロジェクト設定から <code>firebaseConfig</code>（JSON）をコピーして下の欄に貼り付ければ完了です！</li>
                </ol>
                <div>
                    <label class="block text-xs font-bold text-slate-300 mb-1">Firebase Config JSON（任意・外部公開時のみ）</label>
                    <textarea id="customFirebaseConfigInput" rows="4" placeholder='{"apiKey": "...", "authDomain": "...", "projectId": "..."}' class="w-full p-3 rounded-xl bg-slate-950 border border-slate-700 font-mono text-[11px] text-white"></textarea>
                </div>
            </div>
            <div class="flex justify-end gap-2 pt-2">
                <button onclick="closeCustomFirebaseModal()" class="px-4 py-2 rounded-xl bg-slate-800 text-xs font-bold text-slate-300">閉じる</button>
                <button onclick="applyCustomFirebaseConfig()" class="px-5 py-2 rounded-xl bg-indigo-600 hover:bg-indigo-500 text-xs font-black text-white">この設定で再接続</button>
            </div>
        </div>
    </div>

    <!-- TOAST NOTIFICATION -->
    <div id="toastBox" class="fixed bottom-20 md:bottom-6 right-4 z-50 px-4 py-3 rounded-2xl bg-slate-900/95 border border-indigo-500/50 text-white text-xs font-bold shadow-2xl flex items-center gap-2.5 transform translate-y-20 opacity-0 transition-all duration-300 pointer-events-none">
        <i class="fa-solid fa-circle-check text-emerald-400 text-base"></i>
        <span id="toastMessage">保存しました</span>
    </div>

    <!-- ==========================================
         APPLICATION & FIREBASE REALTIME LOGIC
         ========================================== -->
    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, signInWithCustomToken, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore, doc, setDoc, onSnapshot } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        // ------------------------------------------
        // 1. STATE, LOCALSTORAGE HYDRATION & ANTI-OVERWRITE PROTECTION
        // ------------------------------------------
        const STORAGE_KEY_STATE = 'bouki_bakufu_state_v1';
        const STORAGE_KEY_MEMBERS = 'bouki_bakufu_members_v1';
        const STORAGE_KEY_MY_SLOT = 'bouki_bakufu_my_slot';
        const STORAGE_KEY_ONBOARDED = 'bouki_bakufu_onboarded';
        const STORAGE_KEY_CUSTOM_FB = 'bouki_bakufu_firebase_config_v1';

        const DEFAULT_PLACEHOLDER_NAMES = new Set([
            '自分 (P1)', 'フレンドA (P2)', 'フレンドB (P3)',
            '自分', 'フレンドA', 'フレンドB',
            'PLAYER 1', 'PLAYER 2', 'PLAYER 3',
            '将軍', '家老', '奉行', '名前未入力'
        ]);

        function isDefaultMemberName(name) {
            if (!name || typeof name !== 'string') return true;
            return DEFAULT_PLACEHOLDER_NAMES.has(name.trim());
        }

        function slotCodeToMemberId(slotCode) {
            if (slotCode === 'p1' || slotCode === 'm1') return 'm1';
            if (slotCode === 'p2' || slotCode === 'm2') return 'm2';
            if (slotCode === 'p3' || slotCode === 'm3') return 'm3';
            return 'm1';
        }

        function memberIdToSlotCode(memberId) {
            if (memberId === 'm1' || memberId === 'p1') return 'p1';
            if (memberId === 'm2' || memberId === 'p2') return 'p2';
            if (memberId === 'm3' || memberId === 'p3') return 'p3';
            return 'p1';
        }

        // Smartly merge two 3-member arrays so default placeholders NEVER overwrite custom-registered names
        function mergeMembersSmartly(localMembers, incomingMembers) {
            const baseIds = ['m1', 'm2', 'm3'];
            const defaultMeta = [
                { id: 'm1', name: '自分 (P1)', avatar: '🐉', color: 'indigo', status: '今週末ガッツリ遊べる！🔥', updatedAt: 0 },
                { id: 'm2', name: 'フレンドA (P2)', avatar: '🦊', color: 'emerald', status: '21時以降なら毎日いける！', updatedAt: 0 },
                { id: 'm3', name: 'フレンドB (P3)', avatar: '⚡', color: 'pink', status: '新作ゲームやりたい🙌', updatedAt: 0 }
            ];

            return baseIds.map((id, idx) => {
                const fallback = defaultMeta[idx];
                const loc = (Array.isArray(localMembers) ? localMembers.find(m => m && m.id === id) : null) || fallback;
                const inc = (Array.isArray(incomingMembers) ? incomingMembers.find(m => m && m.id === id) : null) || null;

                if (!inc) return { ...fallback, ...loc };

                const locCustom = !isDefaultMemberName(loc.name);
                const incCustom = !isDefaultMemberName(inc.name);

                // Rule 1: Never let a default placeholder overwrite a custom registered name
                if (locCustom && !incCustom) {
                    return { ...fallback, ...inc, name: loc.name, avatar: loc.avatar || inc.avatar, status: loc.status || inc.status, updatedAt: loc.updatedAt || Date.now() };
                }
                if (!locCustom && incCustom) {
                    return { ...fallback, ...loc, ...inc, updatedAt: inc.updatedAt || Date.now() };
                }

                // Rule 2: If both are custom (or both default), newest updatedAt timestamp wins
                const locTime = Number(loc.updatedAt || 0);
                const incTime = Number(inc.updatedAt || 0);
                if (locTime > incTime) {
                    return { ...fallback, ...inc, ...loc };
                }
                return { ...fallback, ...loc, ...inc };
            });
        }

        const today = new Date();
        const currentYear = today.getFullYear();
        const currentMonth = today.getMonth();

        function formatDateKey(year, month, day) {
            return `${year}-${String(month + 1).padStart(2, '0')}-${String(day).padStart(2, '0')}`;
        }

        // Seed upcoming weekend dates so the 3 friends immediately see how a match looks
        const sampleDay1 = formatDateKey(currentYear, currentMonth, Math.min(today.getDate() + 1, 28));
        const sampleDay2 = formatDateKey(currentYear, currentMonth, Math.min(today.getDate() + 2, 28));

        let appState = {
            members: [
                { id: 'm1', name: '自分 (P1)', avatar: '🐉', color: 'indigo', status: '今週末ガッツリ遊べる！🔥', updatedAt: 0 },
                { id: 'm2', name: 'フレンドA (P2)', avatar: '🦊', color: 'emerald', status: '21時以降なら毎日いける！', updatedAt: 0 },
                { id: 'm3', name: 'フレンドB (P3)', avatar: '⚡', color: 'pink', status: '新作ゲームやりたい🙌', updatedAt: 0 }
            ],
            schedules: {
                [sampleDay1]: {
                    m1: 'o', m2: 'o', m3: 'o',
                    time: '21:00〜',
                    gameId: 'g1'
                },
                [sampleDay2]: {
                    m1: 'o', m2: 'm', m3: 'o',
                    time: '22:00〜',
                    gameId: 'g2'
                }
            },
            games: [
                {
                    id: 'g1',
                    title: 'モンスターハンターワイルズ / ライズ',
                    platform: 'Crossplay',
                    imageUrl: 'https://placehold.co/200x200/1e1b4b/38bdf8?text=MONSTER+HUNTER',
                    votes: ['m1', 'm2', 'm3'],
                    suggestedBy: 'm1',
                    status: 'playing'
                },
                {
                    id: 'g2',
                    title: 'Minecraft (マインクラフト)',
                    platform: 'Crossplay',
                    imageUrl: 'https://placehold.co/200x200/064e3b/34d399?text=MINECRAFT',
                    votes: ['m1', 'm3'],
                    suggestedBy: 'm2',
                    status: 'playing'
                },
                {
                    id: 'g3',
                    title: 'Overcooked! 2 (オーバークック2)',
                    platform: 'Switch',
                    imageUrl: 'https://placehold.co/200x200/7f1d1d/f87171?text=OVERCOOKED+2',
                    votes: ['m1', 'm2', 'm3'],
                    suggestedBy: 'm3',
                    status: 'want'
                },
                {
                    id: 'opt_decide_later',
                    title: '🎲 当日ルーレット・ノリで決める（その他）',
                    platform: 'その他',
                    imageUrl: 'https://placehold.co/200x200/3b0764/f472b6?text=DECIDE+ON+SPOT',
                    votes: ['m1', 'm2', 'm3'],
                    suggestedBy: 'm1',
                    status: 'want'
                }
            ],
            partyMemo: '【棒木幕府 軍議メモ】\n・ボイチャはいつも通りDiscord集合！\n・3人の予定が合うと自動でDiscordに伝令が飛ぶぞ！',
            sessionCount: 12,
            discordConfig: {
                webhookUrl: '',
                enabled: true
            },
            memories: [
                { id: 'mem1', date: '2026/11', text: '棒木幕府 結成＆評定サイト開闢！', mvpId: 'm1' }
            ],
            expenses: [],
            arcadeScores: {
                m1: { iaiBestMs: null, mashBestCount: 0, memoryBestMoves: null },
                m2: { iaiBestMs: null, mashBestCount: 0, memoryBestMoves: null },
                m3: { iaiBestMs: null, mashBestCount: 0, memoryBestMoves: null }
            },
            battleStats: {
                m1: { wins: 3, carries: 2, trolls: 1 },
                m2: { wins: 2, carries: 3, trolls: 1 },
                m3: { wins: 2, carries: 2, trolls: 2 }
            }
        };

        // Local UI State
        let activeMemberId = 'm1';
        let currentUserSlot = 'p1'; // 'p1' | 'p2' | 'p3'
        let hasCompletedInitialSetup = false;
        let isHydratedFromLocal = false;
        let onboardingSelectedSlotId = 'm1';
        let onboardingTempAvatar = '🐉';
        let viewYear = currentYear;
        let viewMonth = currentMonth;
        let quickStampMode = 'modal'; // 'modal' | 'o' | 'm' | 'x'
        let currentGameFilter = 'all';
        let currentCatalogCategory = 'fps_action';
        let editingDateKey = null;
        let soundEnabled = false;

        // SYNCHRONOUS STARTUP HYDRATION: Read localStorage & URL Params BEFORE any render or save!
        function hydrateStateSynchronouslyOnStartup() {
            try {
                const rawState = localStorage.getItem(STORAGE_KEY_STATE);
                const rawMembers = localStorage.getItem(STORAGE_KEY_MEMBERS);
                const savedSlot = localStorage.getItem(STORAGE_KEY_MY_SLOT);
                const savedOnboarded = localStorage.getItem(STORAGE_KEY_ONBOARDED);

                if (rawState) {
                    const parsedState = JSON.parse(rawState);
                    if (parsedState && typeof parsedState === 'object') {
                        const mergedMembers = mergeMembersSmartly(appState.members, parsedState.members);
                        appState = {
                            ...appState,
                            ...parsedState,
                            members: mergedMembers,
                            schedules: { ...appState.schedules, ...(parsedState.schedules || {}) },
                            discordConfig: { ...appState.discordConfig, ...(parsedState.discordConfig || {}) },
                            arcadeScores: { ...appState.arcadeScores, ...(parsedState.arcadeScores || {}) },
                            battleStats: { ...appState.battleStats, ...(parsedState.battleStats || {}) }
                        };
                    }
                }

                // Redundant member profile backup always merges over state
                if (rawMembers) {
                    const parsedMembers = JSON.parse(rawMembers);
                    if (Array.isArray(parsedMembers)) {
                        appState.members = mergeMembersSmartly(appState.members, parsedMembers);
                    }
                }

                // Check URL query parameters (?p1=名前1&i1=🐉&p2=名前2&i2=🦊&p3=名前3&i3=⚡&slot=p1)
                const params = new URLSearchParams(window.location.search);
                let urlUpdatedAnyMember = false;
                [1, 2, 3].forEach(num => {
                    const pName = params.get(`p${num}`);
                    const pIcon = params.get(`i${num}`);
                    const targetMember = appState.members[num - 1];
                    if (targetMember && pName && pName.trim()) {
                        targetMember.name = pName.trim();
                        if (pIcon && pIcon.trim()) {
                            targetMember.avatar = pIcon.trim();
                        }
                        targetMember.updatedAt = Date.now();
                        urlUpdatedAnyMember = true;
                    }
                });

                const urlSlot = params.get('slot');
                if (urlSlot) {
                    activeMemberId = slotCodeToMemberId(urlSlot);
                    currentUserSlot = memberIdToSlotCode(activeMemberId);
                    localStorage.setItem(STORAGE_KEY_MY_SLOT, currentUserSlot);
                } else if (savedSlot) {
                    activeMemberId = slotCodeToMemberId(savedSlot);
                    currentUserSlot = memberIdToSlotCode(activeMemberId);
                }

                const myMemberObj = appState.members.find(m => m.id === activeMemberId) || appState.members[0];
                const anyCustomMemberRegistered = appState.members.some(m => !isDefaultMemberName(m.name));

                if (savedOnboarded === 'true' || !isDefaultMemberName(myMemberObj.name) || anyCustomMemberRegistered) {
                    hasCompletedInitialSetup = true;
                }

                isHydratedFromLocal = true;

                if (urlUpdatedAnyMember) {
                    saveStateToLocalStorage();
                }
            } catch (err) {
                console.warn("LocalStorage hydration warning:", err);
                isHydratedFromLocal = true;
            }
        }

        function saveStateToLocalStorage() {
            if (!isHydratedFromLocal) return; // Guard: never overwrite localStorage before initial hydration
            try {
                localStorage.setItem(STORAGE_KEY_STATE, JSON.stringify(appState));
                localStorage.setItem(STORAGE_KEY_MEMBERS, JSON.stringify(appState.members));
                localStorage.setItem(STORAGE_KEY_MY_SLOT, memberIdToSlotCode(activeMemberId));
                if (hasCompletedInitialSetup) {
                    localStorage.setItem(STORAGE_KEY_ONBOARDED, 'true');
                }
            } catch (err) {
                console.warn("LocalStorage save warning:", err);
            }
        }

        // Execute synchronous hydration immediately before anything else runs
        hydrateStateSynchronouslyOnStartup();

        // ------------------------------------------
        // 2. PRESETS, CATALOG DATA, AUDIO & HEADER RENDERERS
        // ------------------------------------------
        const appId = typeof __app_id !== 'undefined' ? __app_id : 'bouki-bakufu-hub';
        let auth = null;
        let db = null;
        let currentUser = null;
        const iconFetchCache = {};

        const PRESET_AVATARS = [
            '🐉', '🦊', '⚡', '🐯', '🦁', '🐺', '🦅', '🦈',
            '🥷', '👹', '👺', '👻', '🤖', '👽', '👾', '🧙‍♂️',
            '⚔️', '🛡️', '🏹', '🔥', '❄️', '💎', '👑', '🏯',
            '🎮', '🕹️', '🎲', '🎯', '🚀', '🐱', '🐶', '🐼'
        ];

        const CURATED_GAME_CATALOG = {
            fps_action: [
                { title: 'モンスターハンターワイルズ / ライズ', platform: 'Crossplay', searchKey: 'Monster Hunter', fallback: 'https://placehold.co/200x200/1e1b4b/38bdf8?text=MONSTER+HUNTER' },
                { title: 'Apex Legends', platform: 'Crossplay', searchKey: 'Apex Legends', fallback: 'https://placehold.co/200x200/7f1d1d/f87171?text=APEX' },
                { title: 'VALORANT', platform: 'PC', searchKey: 'VALORANT', fallback: 'https://placehold.co/200x200/881337/fb7185?text=VALORANT' },
                { title: 'スプラトゥーン3', platform: 'Switch', searchKey: 'Splatoon', fallback: 'https://placehold.co/200x200/3b0764/e879f9?text=SPLATOON+3' },
                { title: 'Overwatch 2', platform: 'Crossplay', searchKey: 'Overwatch', fallback: 'https://placehold.co/200x200/7c2d12/fb923c?text=OVERWATCH+2' },
                { title: 'ストリートファイター6', platform: 'Crossplay', searchKey: 'Street Fighter', fallback: 'https://placehold.co/200x200/312e81/818cf8?text=SF6' },
                { title: ' Fortnite (フォートナイト)', platform: 'Crossplay', searchKey: 'Fortnite', fallback: 'https://placehold.co/200x200/1e3a8a/60a5fa?text=FORTNITE' },
                { title: 'ELDEN RING NIGHTREIGN', platform: 'Crossplay', searchKey: 'ELDEN RING', fallback: 'https://placehold.co/200x200/422006/facc15?text=ELDEN+RING' }
            ],
            party_switch: [
                { title: 'マリオカート8 デラックス', platform: 'Switch', searchKey: 'Mario Kart', fallback: 'https://placehold.co/200x200/7f1d1d/fca5a5?text=MARIO+KART' },
                { title: 'スーパー マリオパーティ ジャンボリー', platform: 'Switch', searchKey: 'Super Mario Run', fallback: 'https://placehold.co/200x200/713f12/fde047?text=MARIO+PARTY' },
                { title: '大乱闘スマッシュブラザーズ SPECIAL', platform: 'Switch', searchKey: 'Smash', fallback: 'https://placehold.co/200x200/1e293b/f8fafc?text=SMASH+BROS' },
                { title: '桃太郎電鉄 ワールド / 昭和平成令和', platform: 'Switch', searchKey: '桃太郎電鉄', fallback: 'https://placehold.co/200x200/831843/f472b6?text=MOMOTETSU' },
                { title: 'Overcooked! 2 (オーバークック2)', platform: 'Switch', searchKey: 'Overcooked', fallback: 'https://placehold.co/200x200/7c2d12/fdba74?text=OVERCOOKED+2' },
                { title: '世界のアソビ大全51', platform: 'Switch', searchKey: 'テーブルゲーム', fallback: 'https://placehold.co/200x200/14532d/86efac?text=ASOBI+51' },
                { title: 'Ultimate Chicken Horse', platform: 'Crossplay', searchKey: 'Chicken Horse', fallback: 'https://placehold.co/200x200/78350f/fcd34d?text=CHICKEN+HORSE' },
                { title: 'ヒューマン フォール フラット', platform: 'Crossplay', searchKey: 'Human Fall Flat', fallback: 'https://placehold.co/200x200/1e3a8a/93c5fd?text=HUMAN+FALL+FLAT' }
            ],
            coop_survival: [
                { title: 'Minecraft (マインクラフト)', platform: 'Crossplay', searchKey: 'Minecraft', fallback: 'https://placehold.co/200x200/064e3b/34d399?text=MINECRAFT' },
                { title: 'Palworld (パルワールド)', platform: 'Crossplay', searchKey: 'Palworld', fallback: 'https://placehold.co/200x200/0c4a6e/38bdf8?text=PALWORLD' },
                { title: 'Lethal Company / R.E.P.O.', platform: 'PC', searchKey: 'Horror Coop', fallback: 'https://placehold.co/200x200/450a0a/f87171?text=HORROR+COOP' },
                { title: 'ARK: Survival Ascended', platform: 'Crossplay', searchKey: 'ARK Survival', fallback: 'https://placehold.co/200x200/134e4a/2dd4bf?text=ARK' },
                { title: '地球防衛軍6', platform: 'PS5', searchKey: 'Defense', fallback: 'https://placehold.co/200x200/1f2937/9ca3af?text=EDF+6' },
                { title: 'Core Keeper (コアキーパー)', platform: 'Crossplay', searchKey: 'Terraria', fallback: 'https://placehold.co/200x200/365314/a3e635?text=CORE+KEEPER' },
                { title: 'モンスターハンターNow / ワールド', platform: 'Crossplay', searchKey: 'Monster Hunter Now', fallback: 'https://placehold.co/200x200/312e81/a5b4fc?text=MH+WORLD' },
                { title: '原神 (Genshin Impact)', platform: 'Crossplay', searchKey: '原神', fallback: 'https://placehold.co/200x200/1e1b4b/c7d2fe?text=GENSHIN' }
            ],
            mobile_cross: [
                { title: 'Pokémon TCG Pocket (ポケポケ)', platform: 'Mobile', searchKey: 'ポケポケ', fallback: 'https://placehold.co/200x200/713f12/fde047?text=POKEPOKE' },
                { title: 'モンスターストライク (モンスト)', platform: 'Mobile', searchKey: 'モンスターストライク', fallback: 'https://placehold.co/200x200/7c2d12/fb923c?text=MONST' },
                { title: '荒野行動 / PUBG MOBILE', platform: 'Mobile', searchKey: 'PUBG MOBILE', fallback: 'https://placehold.co/200x200/422006/facc15?text=BATTLE+ROYALE' },
                { title: '麻雀一番街 / 雀魂 (じゃんたま)', platform: 'Crossplay', searchKey: '雀魂', fallback: 'https://placehold.co/200x200/064e3b/6ee7b7?text=MAHJONG' },
                { title: 'Among Us (アモングアス)', platform: 'Crossplay', searchKey: 'Among Us', fallback: 'https://placehold.co/200x200/7f1d1d/f87171?text=AMONG+US' },
                { title: 'ブロスタ (Brawl Stars)', platform: 'Mobile', searchKey: 'ブロスタ', fallback: 'https://placehold.co/200x200/3b0764/f472b6?text=BRAWL+STARS' },
                { title: 'IdentityV 第五人格', platform: 'Mobile', searchKey: '第五人格', fallback: 'https://placehold.co/200x200/1e293b/cbd5e1?text=IDENTITY+V' },
                { title: 'プロジェクトセカイ / リズムゲーム', platform: 'Mobile', searchKey: 'プロセカ', fallback: 'https://placehold.co/200x200/0f766e/5eead4?text=PROSEKA' }
            ],
            other_activities: [
                { title: '🎲 当日ルーレット・ノリで決める', platform: 'その他', searchKey: '', fallback: 'https://placehold.co/200x200/3b0764/f472b6?text=DECIDE+LATER' },
                { title: '💬 雑談・作業通話・画面共有', platform: 'その他', searchKey: '', fallback: 'https://placehold.co/200x200/0c4a6e/38bdf8?text=VOICE+CHAT' },
                { title: '🛒 新作ゲーム探し・Steamセール巡り', platform: 'その他', searchKey: '', fallback: 'https://placehold.co/200x200/064e3b/34d399?text=GAME+HUNT' },
                { title: '🎬 ウォッチパーティ・動画/配信鑑賞', platform: 'その他', searchKey: '', fallback: 'https://placehold.co/200x200/7f1d1d/fca5a5?text=WATCH+PARTY' },
                { title: '🍻 オンライン飲み会・近況報告会', platform: 'その他', searchKey: '', fallback: 'https://placehold.co/200x200/78350f/fcd34d?text=ONLINE+DRINK' },
                { title: '✏️ 自由入力で新しい選択肢を作る...', platform: 'その他', searchKey: 'CUSTOM_MODAL', fallback: 'https://placehold.co/200x200/312e81/a5b4fc?text=+CUSTOM+' }
            ]
        };

        function renderAvatarHtml(avatarStr, sizeClasses = 'w-6 h-6 text-base') {
            if (!avatarStr) return `<span class="${sizeClasses} inline-flex items-center justify-center">🐉</span>`;
            if (avatarStr.startsWith('data:image') || avatarStr.startsWith('http')) {
                return `<img src="${escapeHtml(avatarStr)}" alt="avatar" class="${sizeClasses} rounded-full object-cover inline-block shrink-0 border border-white/20">`;
            }
            return `<span class="${sizeClasses} inline-flex items-center justify-center leading-none select-none shrink-0">${escapeHtml(avatarStr)}</span>`;
        }

        function renderMemberHeader() {
            const switcher = document.getElementById('memberSwitcherContainer');
            if (switcher) {
                switcher.innerHTML = appState.members.map(m => {
                    const isActive = m.id === activeMemberId;
                    return `
                        <button
                            type="button"
                            onclick="switchActiveMember('${m.id}')"
                            class="px-2 sm:px-3 py-1 rounded-xl text-xs font-black flex items-center gap-1 sm:gap-1.5 transition max-w-[105px] sm:max-w-[140px] ${
                                isActive
                                    ? 'bg-indigo-600 text-white shadow-md shadow-indigo-500/30 ring-1 ring-indigo-300'
                                    : 'bg-slate-950/70 text-slate-400 hover:text-slate-200 hover:bg-slate-800'
                            }"
                        >
                            ${renderAvatarHtml(m.avatar, 'w-4 h-4 text-xs')}
                            <span class="truncate">${escapeHtml(m.name)}</span>
                        </button>
                    `;
                }).join('');
            }

            const pills = document.getElementById('memberStatusPills');
            if (pills) {
                pills.innerHTML = appState.members.map(m => {
                    const isActive = m.id === activeMemberId;
                    return `
                        <div
                            onclick="switchActiveMember('${m.id}'); openStatusUpdateModal();"
                            class="min-w-0 cursor-pointer px-2 sm:px-3 py-1.5 rounded-xl border transition flex items-center gap-1.5 sm:gap-2 ${
                                isActive
                                    ? 'bg-indigo-950/60 border-indigo-500/50 text-white'
                                    : 'bg-slate-950/70 border-slate-800/90 text-slate-300 hover:border-slate-700'
                            }"
                        >
                            ${renderAvatarHtml(m.avatar, 'w-5 h-5 sm:w-6 sm:h-6 text-sm sm:text-base')}
                            <div class="min-w-0 flex-1">
                                <div class="text-[10px] sm:text-xs font-black text-white truncate">${escapeHtml(m.name)}</div>
                                <div class="text-[9px] sm:text-[11px] text-emerald-300 truncate">${escapeHtml(m.status || 'ステータス未設定')}</div>
                            </div>
                        </div>
                    `;
                }).join('');
            }

            const activeIndicator = document.getElementById('activeMemberIndicatorText');
            if (activeIndicator) {
                const activeM = appState.members.find(m => m.id === activeMemberId) || appState.members[0];
                activeIndicator.textContent = `操作中: ${activeM.name}`;
            }
        }

        function renderAll() {
            renderMemberHeader();
            renderDiscordHeaderStatus();
            renderCalendar();
            renderMatchedDaysList();
            renderCatalogList(currentCatalogCategory);
            renderGamesVotingBoard();
            renderArcadeLeaderboard();
            renderMemberBattleStats();
            renderPartyTools();
            renderBakufuMemoriesAndExpenses();
            updateGlobalCounters();
        }

        window.toggleSound = async function() {
            soundEnabled = !soundEnabled;
            if (soundEnabled && typeof Tone !== 'undefined') {
                try { await Tone.start(); } catch (e) {}
            }
            const btn = document.getElementById('soundToggleBtn');
            if (btn) {
                btn.innerHTML = soundEnabled
                    ? '<i class="fa-solid fa-volume-high text-emerald-400"></i>'
                    : '<i class="fa-solid fa-volume-xmark"></i>';
            }
            showToast(soundEnabled ? '🔊 効果音をONにしました' : '🔇 効果音をOFFにしました');
        };

        function playUiSound(type = 'tap') {
            if (!soundEnabled || typeof Tone === 'undefined') return;
            try {
                const synth = new Tone.Synth().toDestination();
                synth.volume.value = -12;
                if (type === 'match') {
                    synth.triggerAttackRelease('C5', '16n');
                    setTimeout(() => synth.triggerAttackRelease('G5', '8n'), 90);
                } else if (type === 'vote') {
                    synth.triggerAttackRelease('E5', '16n');
                } else {
                    synth.triggerAttackRelease('A4', '32n');
                }
            } catch (e) {}
        }

        // ------------------------------------------
        // 3. FIREBASE INITIALIZATION & REALTIME SYNC
        // ------------------------------------------
        async function initRealtimeSync() {
            try {
                let rawConfig = (typeof __firebase_config !== 'undefined' && __firebase_config)
                    ? __firebase_config
                    : localStorage.getItem(STORAGE_KEY_CUSTOM_FB);

                if (!rawConfig) {
                    renderAll();
                    return;
                }
                const firebaseConfig = typeof rawConfig === 'string' ? JSON.parse(rawConfig) : rawConfig;
                const app = initializeApp(firebaseConfig);
                auth = getAuth(app);
                db = getFirestore(app);

                // RULE 3: Authenticate before any Firestore calls
                if (typeof __initial_auth_token !== 'undefined' && __initial_auth_token) {
                    await signInWithCustomToken(auth, __initial_auth_token);
                } else {
                    await signInAnonymously(auth);
                }

                onAuthStateChanged(auth, (user) => {
                    currentUser = user;
                    if (user) {
                        subscribeToPartyHub();
                    }
                });
            } catch (err) {
                console.warn("Running in standalone local persistence mode:", err);
                renderAll();
            }
        }

        function subscribeToPartyHub() {
            if (!currentUser || !db) return;
            // RULE 1: Strict public path so all 3 friends share the board
            const hubDocRef = doc(db, 'artifacts', appId, 'public', 'data', 'trioHubState', 'mainRoom');

            onSnapshot(hubDocRef, (snapshot) => {
                if (snapshot.exists()) {
                    const data = snapshot.data();
                    if (data.payload) {
                        try {
                            const parsed = JSON.parse(data.payload);

                            // Check if local has custom member names that remote still has as default placeholders
                            const localBackupMembers = (() => {
                                try {
                                    const raw = localStorage.getItem(STORAGE_KEY_MEMBERS);
                                    return raw ? JSON.parse(raw) : appState.members;
                                } catch (e) {
                                    return appState.members;
                                }
                            })();

                            const currentLocalMembers = mergeMembersSmartly(appState.members, localBackupMembers);
                            const remoteMembers = Array.isArray(parsed.members) ? parsed.members : [];
                            const smartMergedMembers = mergeMembersSmartly(currentLocalMembers, remoteMembers);

                            // Check whether local protected a custom name against a remote placeholder
                            const neededLocalProtection = smartMergedMembers.some((m, idx) => {
                                const rem = remoteMembers[idx];
                                return !isDefaultMemberName(m.name) && (!rem || isDefaultMemberName(rem.name) || (m.updatedAt || 0) > (rem.updatedAt || 0));
                            });

                            appState = {
                                ...appState,
                                ...parsed,
                                members: smartMergedMembers,
                                schedules: { ...(appState.schedules || {}), ...(parsed.schedules || {}) },
                                discordConfig: (parsed.discordConfig && parsed.discordConfig.webhookUrl)
                                    ? parsed.discordConfig
                                    : (appState.discordConfig || { webhookUrl: '', enabled: true })
                            };

                            saveStateToLocalStorage();
                            renderAll();

                            // If local had newer or custom member profiles that remote didn't have, sync them back up
                            if (neededLocalProtection) {
                                pushStateToCloud();
                            }
                        } catch (e) {
                            console.error("Failed to parse synced payload:", e);
                        }
                    }
                } else {
                    // Firestore doc doesn't exist yet -> initialize it with our already-hydrated local appState!
                    pushStateToCloud();
                }
            }, (error) => {
                console.warn("Firestore sync error:", error);
            });
        }

        async function pushStateToCloud() {
            saveStateToLocalStorage();
            renderAll();
            if (!currentUser || !db) return;
            try {
                const hubDocRef = doc(db, 'artifacts', appId, 'public', 'data', 'trioHubState', 'mainRoom');
                await setDoc(hubDocRef, {
                    payload: JSON.stringify(appState),
                    updatedAt: Date.now(),
                    updatedBy: currentUser.uid
                });
            } catch (e) {
                console.warn("Cloud save skipped:", e);
            }
        }

        window.switchActiveMember = function(memberId) {
            activeMemberId = slotCodeToMemberId(memberId);
            currentUserSlot = memberIdToSlotCode(activeMemberId);
            localStorage.setItem(STORAGE_KEY_MY_SLOT, currentUserSlot);
            saveStateToLocalStorage();
            playUiSound('tap');
            renderAll();
            const m = appState.members.find(x => x.id === activeMemberId);
            if (m) showToast(`操作メンバーを「${m.name}」に切り替えました`);
        };

        // ------------------------------------------
        // 4.2 DISCORD WEBHOOK AUTO-NOTIFICATION ENGINE (ONLY WHEN ALL 3 MATCH)
        // ------------------------------------------
        function renderDiscordHeaderStatus() {
            const badge = document.getElementById('discordHeaderBadge');
            if (!badge) return;
            const cfg = appState.discordConfig || { webhookUrl: '', enabled: true };
            const isReady = Boolean(cfg.webhookUrl && cfg.webhookUrl.startsWith('https://discord') && cfg.enabled);

            if (isReady) {
                badge.className = 'inline-flex items-center gap-1 text-[10px] font-black px-2.5 py-0.5 rounded-full bg-[#5865F2]/30 text-indigo-200 border border-[#5865F2] hover:bg-[#5865F2]/40 transition';
                badge.innerHTML = `<i class="fa-brands fa-discord text-[#5865F2]"></i><span>🔔 Discord伝令ON</span>`;
            } else {
                badge.className = 'inline-flex items-center gap-1 text-[10px] font-black px-2.5 py-0.5 rounded-full bg-slate-800 text-slate-400 border border-slate-700 hover:border-indigo-400 transition';
                badge.innerHTML = `<i class="fa-brands fa-discord"></i><span>🔕 Discord未設定</span>`;
            }
        }

        window.openDiscordSettingsModal = function() {
            const cfg = appState.discordConfig || { webhookUrl: '', enabled: true };
            document.getElementById('discordWebhookUrlInput').value = cfg.webhookUrl || '';
            document.getElementById('discordAutoNotifyToggle').checked = cfg.enabled !== false;
            const modal = document.getElementById('discordSettingsModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        };

        window.closeDiscordSettingsModal = function() {
            const modal = document.getElementById('discordSettingsModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        };

        window.saveDiscordWebhookSettings = function() {
            const url = document.getElementById('discordWebhookUrlInput').value.trim();
            const enabled = document.getElementById('discordAutoNotifyToggle').checked;
            appState.discordConfig = { webhookUrl: url, enabled: enabled };
            closeDiscordSettingsModal();
            playUiSound('match');
            pushStateToCloud();
            showToast(url ? '🔔 Discord自動伝令（3人一致時のみ通知）を設定しました！' : 'Discord設定を更新しました');
        };

        // Compute a unique signature for a 3-person matched day so we only notify on new match or meaningful change
        function computeMatchSignature(dateKey, dayRecord) {
            if (!dayRecord) return null;
            const matchType = evaluateDayMatch(dayRecord);
            if (matchType === 'none') return null; // Not all 3 matched
            const statuses = appState.members.map(m => `${m.id}:${dayRecord[m.id] || ''}`).join(',');
            return `${matchType}|${statuses}|${dayRecord.time || ''}|${dayRecord.gameId || ''}`;
        }

        // Check if a date newly matched all 3 players (or updated its game/time while matched) and trigger Discord Webhook
        async function checkAndTriggerDiscordMatchNotification(dateKey, forceManual = false) {
            const rec = appState.schedules[dateKey];
            if (!rec) return false;

            const matchType = evaluateDayMatch(rec);
            // STRICT RULE: Never notify unless all 3 members are 'o' (◯) or 'm' (△)
            if (matchType === 'none') {
                return false;
            }

            const cfg = appState.discordConfig || {};
            if (!cfg.webhookUrl || !cfg.webhookUrl.startsWith('https://discord')) {
                if (forceManual) {
                    showToast('先に「伝令設定」からDiscord Webhook URLを登録してください！');
                    openDiscordSettingsModal();
                }
                return false;
            }

            if (!forceManual && cfg.enabled === false) {
                return false;
            }

            const currentSignature = computeMatchSignature(dateKey, rec);
            if (!forceManual && rec.discordNotifiedSignature === currentSignature) {
                // Already notified for this exact 3-person match state
                return false;
            }

            const game = rec.gameId ? appState.games.find(g => g.id === rec.gameId) : null;
            const isPerfect = matchType === 'perfect';

            const memberLines = appState.members.map(m => {
                const st = rec[m.id] === 'o' ? '🟢 **◯ (いつでもOK)**' : '🟡 **△ (遅め・条件付)**';
                const emojiIcon = (m.avatar && !m.avatar.startsWith('data:') && !m.avatar.startsWith('http')) ? m.avatar : '🎮';
                return `${emojiIcon} **${m.name}** ： ${st}`;
            }).join('\n');

            const embedTitle = isPerfect
                ? `🏯【棒木幕府】🎉 3人全員「◯」で評定（集合）が確定しました！`
                : `🏯【棒木幕府】⚡ 3人全員集合可能（△含む）な日が揃いました！`;

            const embedColor = isPerfect ? 0x00f5d4 : 0xffbe0b;

            const payload = {
                username: "棒木幕府 伝令役",
                content: isPerfect
                    ? `📣 **いざ鎌倉！ ${formatJapaneseDate(dateKey)} は3人全員「◯」で予定が一致しました！**`
                    : `📣 **${formatJapaneseDate(dateKey)} は3人全員（◯・△）の予定が合いました！**`,
                embeds: [
                    {
                        title: embedTitle,
                        color: embedColor,
                        fields: [
                            {
                                name: "📅 開催日",
                                value: `**${dateKey} (${formatJapaneseDate(dateKey)})**`,
                                inline: true
                            },
                            {
                                name: "⏰ 集合時間・目安",
                                value: `**${rec.time || '時間未定（21:00頃〜）'}**`,
                                inline: true
                            },
                            {
                                name: "🎮 遊ぶゲーム・予定内容",
                                value: `**${game ? `${game.title} (${game.platform})` : '🎲 当日ルーレット・未定'}**`,
                                inline: false
                            },
                            {
                                name: "👥 家臣3名の出陣ステータス",
                                value: memberLines,
                                inline: false
                            }
                        ],
                        footer: {
                            text: "棒木幕府 (BOUKI BAKUFU) • 3人の予定が揃った時だけ自動通知"
                        },
                        timestamp: new Date().toISOString()
                    }
                ]
            };

            if (game && game.imageUrl && game.imageUrl.startsWith('http')) {
                payload.embeds[0].thumbnail = { url: game.imageUrl };
            }

            try {
                const response = await fetch(cfg.webhookUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });

                if (response.ok) {
                    rec.discordNotifiedSignature = currentSignature;
                    rec.discordNotifiedAt = Date.now();
                    pushStateToCloud();
                    showToast(`📣 3人の予定が一致したため、Discordへ伝令を飛ばしました！`);
                    return true;
                } else {
                    showToast('⚠️ Discordへの通知送信に失敗しました（Webhook URLを確認してください）');
                    return false;
                }
            } catch (err) {
                console.warn("Discord webhook error:", err);
                showToast('⚠️ Discord通知エラーが発生しました');
                return false;
            }
        }

        window.manualSendDiscordForEditingDay = async function() {
            if (!editingDateKey) return;
            if (!appState.schedules[editingDateKey]) appState.schedules[editingDateKey] = {};
            appState.schedules[editingDateKey].gameId = document.getElementById('modalDayGameSelect').value;
            appState.schedules[editingDateKey].time = document.getElementById('modalDayTimeInput').value.trim();
            await checkAndTriggerDiscordMatchNotification(editingDateKey, true);
        };

        window.sendTestDiscordWebhook = async function() {
            const url = document.getElementById('discordWebhookUrlInput').value.trim();
            if (!url || !url.startsWith('https://discord')) {
                showToast('有効なDiscord Webhook URLを入力してください');
                return;
            }
            const btn = document.getElementById('testDiscordWebhookBtn');
            btn.disabled = true;
            try {
                const res = await fetch(url, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({
                        username: "棒木幕府 伝令役",
                        embeds: [{
                            title: "🏯【棒木幕府】テスト伝令・通信成功！",
                            description: "これからカレンダーで**3人全員の予定が合った（◯または△で揃った）ときだけ**、このチャンネルへ自動で通知が届きます！",
                            color: 0x6366f1,
                            fields: [
                                { name: "👥 登録メンバー", value: appState.members.map(m => m.name).join(' / '), inline: false }
                            ]
                        }]
                    })
                });
                if (res.ok) {
                    playUiSound('match');
                    showToast('🎉 Discordへテスト伝令を送信しました！チャンネルを確認してください');
                } else {
                    showToast('⚠️ 送信できませんでした。Webhook URLを確認してください');
                }
            } catch (e) {
                showToast('⚠️ 通信エラーが発生しました');
            } finally {
                btn.disabled = false;
            }
        };

        window.setOneTapRealtimeSignal = function(signalText) {
            const m = appState.members.find(x => x.id === activeMemberId);
            if (!m) return;
            m.status = signalText;
            m.updatedAt = Date.now();
            playUiSound('match');
            pushStateToCloud();
            showToast(`${m.name} の状況を「${signalText}」に更新しました！`);
        };

        // ------------------------------------------
        // 4.5 INITIAL ONBOARDING & MEMBER REGISTRATION LOGIC
        // ------------------------------------------
        window.openOnboardingModal = function(manualOpen = false) {
            onboardingSelectedSlotId = activeMemberId || 'm1';
            const currentMember = appState.members.find(m => m.id === onboardingSelectedSlotId) || appState.members[0];
            onboardingTempAvatar = currentMember.avatar || '🐉';

            const nameEl = document.getElementById('onboardingNameInput');
            const statusEl = document.getElementById('onboardingStatusInput');
            if (nameEl) nameEl.value = isDefaultMemberName(currentMember.name) ? '' : (currentMember.name || '');
            if (statusEl) statusEl.value = currentMember.status || '';

            renderOnboardingSlots();
            renderOnboardingEmojiPalette();
            updateOnboardingPreview();

            const modal = document.getElementById('onboardingModal');
            if (modal) {
                modal.classList.remove('hidden');
                modal.classList.add('flex');
            }
        };

        window.closeOnboardingModal = function() {
            const modal = document.getElementById('onboardingModal');
            if (modal) {
                modal.classList.add('hidden');
                modal.classList.remove('flex');
            }
        };

        function renderOnboardingSlots() {
            const grid = document.getElementById('onboardingSlotGrid');
            if (!grid) return;
            grid.innerHTML = appState.members.map((m, idx) => {
                const isSelected = m.id === onboardingSelectedSlotId;
                return `
                    <button
                        type="button"
                        onclick="selectOnboardingSlot('${m.id}')"
                        class="p-3 rounded-2xl border text-center flex flex-col items-center gap-1.5 transition ${
                            isSelected
                                ? 'bg-amber-500/20 border-amber-400 ring-2 ring-amber-400/50 text-white shadow-lg'
                                : 'bg-slate-950/80 border-slate-800 text-slate-400 hover:bg-slate-900'
                        }"
                    >
                        <span class="text-[10px] font-black uppercase px-2 py-0.5 rounded-full ${isSelected ? 'bg-amber-400 text-slate-950' : 'bg-slate-800 text-slate-400'}">
                            PLAYER ${idx + 1}
                        </span>
                        <div class="my-0.5">${renderAvatarHtml(m.avatar, 'w-10 h-10 text-2xl')}</div>
                        <span class="text-xs font-black truncate max-w-full">${escapeHtml(m.name)}</span>
                    </button>
                `;
            }).join('');
        }

        window.selectOnboardingSlot = function(slotId) {
            onboardingSelectedSlotId = slotId;
            const m = appState.members.find(x => x.id === slotId);
            if (m) {
                onboardingTempAvatar = m.avatar || '🐉';
                const nameEl = document.getElementById('onboardingNameInput');
                const statusEl = document.getElementById('onboardingStatusInput');
                if (nameEl) nameEl.value = isDefaultMemberName(m.name) ? '' : (m.name || '');
                if (statusEl) statusEl.value = m.status || '';
            }
            playUiSound('tap');
            renderOnboardingSlots();
            renderOnboardingEmojiPalette();
            updateOnboardingPreview();
        };

        function renderOnboardingEmojiPalette() {
            const palette = document.getElementById('onboardingEmojiPalette');
            if (!palette) return;
            palette.innerHTML = PRESET_AVATARS.map(emoji => {
                const isSelected = onboardingTempAvatar === emoji;
                return `
                    <button
                        type="button"
                        onclick="selectOnboardingEmoji('${emoji}')"
                        class="h-9 rounded-xl text-lg flex items-center justify-center border transition ${
                            isSelected
                                ? 'bg-amber-500/30 border-amber-400 scale-105'
                                : 'bg-slate-900 border-slate-800 hover:bg-slate-800'
                        }"
                    >
                        ${emoji}
                    </button>
                `;
            }).join('');
        }

        window.selectOnboardingEmoji = function(emoji) {
            onboardingTempAvatar = emoji;
            playUiSound('tap');
            renderOnboardingEmojiPalette();
            updateOnboardingPreview();
        };

        window.updateOnboardingPreview = function() {
            const previewBox = document.getElementById('onboardingAvatarPreviewBox');
            const namePreview = document.getElementById('onboardingNamePreviewText');
            const nameInput = document.getElementById('onboardingNameInput');

            if (previewBox) {
                previewBox.innerHTML = renderAvatarHtml(onboardingTempAvatar, 'w-14 h-14 text-3xl');
            }
            if (namePreview && nameInput) {
                namePreview.textContent = nameInput.value.trim() || '名前未入力';
            }
        };

        window.handleAvatarFileUpload = function(event) {
            const file = event.target.files && event.target.files[0];
            if (!file) return;
            const reader = new FileReader();
            reader.onload = function(e) {
                const img = new Image();
                img.onload = function() {
                    const canvas = document.createElement('canvas');
                    const maxDim = 128;
                    canvas.width = maxDim;
                    canvas.height = maxDim;
                    const ctx = canvas.getContext('2d');
                    const minSide = Math.min(img.width, img.height);
                    const sx = (img.width - minSide) / 2;
                    const sy = (img.height - minSide) / 2;
                    ctx.drawImage(img, sx, sy, minSide, minSide, 0, 0, maxDim, maxDim);
                    onboardingTempAvatar = canvas.toDataURL('image/jpeg', 0.82);
                    playUiSound('match');
                    renderOnboardingEmojiPalette();
                    updateOnboardingPreview();
                    showToast('アイコン画像を読み込みました！');
                };
                img.src = e.target.result;
            };
            reader.readAsDataURL(file);
        };

        window.completeOnboardingRegistration = function() {
            const nameVal = document.getElementById('onboardingNameInput').value.trim();
            const statusVal = document.getElementById('onboardingStatusInput').value.trim();

            if (!nameVal) {
                showToast('プレイヤー名（ニックネーム）を入力してください！');
                return;
            }

            const member = appState.members.find(m => m.id === onboardingSelectedSlotId);
            if (member) {
                member.name = nameVal;
                member.avatar = onboardingTempAvatar || '🐉';
                if (statusVal) member.status = statusVal;
                member.updatedAt = Date.now();
            }

            activeMemberId = onboardingSelectedSlotId;
            currentUserSlot = memberIdToSlotCode(activeMemberId);
            hasCompletedInitialSetup = true;

            localStorage.setItem(STORAGE_KEY_MY_SLOT, currentUserSlot);
            localStorage.setItem(STORAGE_KEY_ONBOARDED, 'true');
            localStorage.setItem(STORAGE_KEY_MEMBERS, JSON.stringify(appState.members));
            saveStateToLocalStorage();

            closeOnboardingModal();
            playUiSound('match');
            pushStateToCloud();
            showToast(`🎉 「${nameVal}」としてプロフィールを保存しました！次回からも自動で維持されます`);
        };

        // Generate & Copy a shareable URL containing the 3 registered member names and icons
        window.copyMemberProfileShareUrl = function() {
            const baseUrl = window.location.origin + window.location.pathname;
            const params = new URLSearchParams();
            appState.members.forEach((m, idx) => {
                const num = idx + 1;
                if (m.name) params.set(`p${num}`, m.name);
                // Only embed emoji or short icon strings in URL query parameters (skip base64 images)
                if (m.avatar && !m.avatar.startsWith('data:') && m.avatar.length <= 16) {
                    params.set(`i${num}`, m.avatar);
                }
            });

            const shareUrl = `${baseUrl}?${params.toString()}`;
            const temp = document.createElement('textarea');
            temp.value = shareUrl;
            document.body.appendChild(temp);
            temp.select();
            document.execCommand('copy');
            document.body.removeChild(temp);

            playUiSound('match');
            showToast('📋 3人のメンバー名入り共有URLをコピーしました！友達が開くと名前が自動反映されます');
        };

        // ------------------------------------------
        // 5. CALENDAR LOGIC & 3-PLAYER MATCH ENGINE
        // ------------------------------------------
        function evaluateDayMatch(dayRecord) {
            if (!dayRecord) return 'none';
            const statuses = appState.members.map(m => dayRecord[m.id] || '');
            const allCircle = statuses.every(s => s === 'o');
            if (allCircle) return 'perfect'; // All 3 are ◯
            const allPlayable = statuses.every(s => s === 'o' || s === 'm');
            if (allPlayable) return 'chance'; // All 3 are ◯ or △
            return 'none';
        }

        function symbolBadge(val) {
            if (val === 'o') return '<span class="text-emerald-400 font-black">◯</span>';
            if (val === 'm') return '<span class="text-amber-400 font-black">△</span>';
            if (val === 'x') return '<span class="text-rose-400 font-black">×</span>';
            return '<span class="text-slate-600">-</span>';
        }

        function renderCalendar() {
            const titleEl = document.getElementById('calendarMonthTitle');
            titleEl.textContent = `${viewYear}年 ${viewMonth + 1}月`;

            const grid = document.getElementById('calendarGrid');
            const firstDayOfWeek = new Date(viewYear, viewMonth, 1).getDay();
            const daysInMonth = new Date(viewYear, viewMonth + 1, 0).getDate();

            let html = '';

            // Empty leading cells
            for (let i = 0; i < firstDayOfWeek; i++) {
                html += `<div class="min-h-[68px] sm:min-h-[96px] min-w-0 rounded-xl bg-slate-950/30 border border-slate-900/50"></div>`;
            }

            const todayKey = formatDateKey(today.getFullYear(), today.getMonth(), today.getDate());

            for (let day = 1; day <= daysInMonth; day++) {
                const dateKey = formatDateKey(viewYear, viewMonth, day);
                const rec = appState.schedules[dateKey] || {};
                const matchType = evaluateDayMatch(rec);
                const isToday = dateKey === todayKey;
                const dayOfWeek = new Date(viewYear, viewMonth, day).getDay();

                let dayColor = 'text-slate-200';
                if (dayOfWeek === 0) dayColor = 'text-rose-400';
                if (dayOfWeek === 6) dayColor = 'text-sky-400';

                // Pure color-based match highlighting without any text labels inside calendar cells
                let cardStyle = 'bg-slate-900/80 border border-gaming-border hover:border-indigo-500/60';
                let innerBoxStyle = 'bg-slate-950/85 border-slate-800/80';

                if (matchType === 'perfect') {
                    cardStyle = 'bg-gradient-to-br from-emerald-500/45 via-emerald-600/30 to-teal-500/45 border-2 border-emerald-300 glow-match';
                    innerBoxStyle = 'bg-emerald-950/80 border-emerald-400/50';
                    dayColor = 'text-emerald-200';
                } else if (matchType === 'chance') {
                    cardStyle = 'bg-gradient-to-br from-amber-500/40 via-amber-600/25 to-yellow-500/40 border-2 border-amber-300 glow-chance';
                    innerBoxStyle = 'bg-amber-950/80 border-amber-400/50';
                    dayColor = 'text-amber-200';
                }

                const assignedGame = rec.gameId ? appState.games.find(g => g.id === rec.gameId) : null;

                html += `
                    <div
                        onclick="handleCalendarDayClick('${dateKey}')"
                        class="min-h-[68px] sm:min-h-[96px] min-w-0 overflow-hidden p-1 sm:p-2 rounded-xl ${cardStyle} flex flex-col justify-between cursor-pointer transition select-none"
                    >
                        <div class="flex items-center justify-between gap-0.5 min-w-0">
                            <span class="text-[11px] sm:text-sm font-black leading-none ${dayColor} ${isToday ? 'bg-indigo-600 text-white px-1 sm:px-1.5 py-0.5 rounded' : ''}">
                                ${day}
                            </span>
                            ${assignedGame ? `
                                <img src="${escapeHtml(assignedGame.imageUrl)}" onerror="this.src='https://placehold.co/40x40/312e81/ffffff?text=G'" class="w-3.5 h-3.5 sm:w-4 sm:h-4 rounded object-cover shrink-0 border border-white/30">
                            ` : ''}
                        </div>

                        <!-- 3 Members Status Row (Icons & Symbols Only, Zero Text) -->
                        <div class="grid grid-cols-3 gap-0 sm:gap-0.5 ${innerBoxStyle} rounded-lg p-0.5 sm:p-1.5 border text-center min-w-0">
                            ${appState.members.map(m => `
                                <div class="flex flex-col items-center justify-center leading-none min-w-0 overflow-hidden">
                                    ${renderAvatarHtml(m.avatar, 'w-3 h-3 sm:w-4 sm:h-4 text-[9px] sm:text-xs')}
                                    <span class="text-[10px] sm:text-xs mt-0.5">${symbolBadge(rec[m.id])}</span>
                                </div>
                            `).join('')}
                        </div>
                    </div>
                `;
            }

            grid.innerHTML = html;
        }

        window.changeMonth = function(delta) {
            viewMonth += delta;
            if (viewMonth > 11) {
                viewMonth = 0;
                viewYear++;
            } else if (viewMonth < 0) {
                viewMonth = 11;
                viewYear--;
            }
            playUiSound('tap');
            renderCalendar();
        };

        window.goToTodayMonth = function() {
            viewYear = today.getFullYear();
            viewMonth = today.getMonth();
            playUiSound('tap');
            renderCalendar();
        };

        window.setQuickStampMode = function(mode) {
            quickStampMode = mode;
            ['modal', 'o', 'm', 'x'].forEach(k => {
                const btn = document.getElementById(`stampMode-${k}`);
                if (!btn) return;
                if (k === mode) {
                    btn.className = 'px-2.5 py-1 rounded-lg text-xs font-black bg-indigo-600 text-white transition';
                } else {
                    const colorMap = { modal: 'text-slate-300', o: 'text-emerald-400', m: 'text-amber-400', x: 'text-rose-400' };
                    btn.className = `px-2.5 py-1 rounded-lg text-xs font-bold ${colorMap[k]} hover:bg-slate-800 transition`;
                }
            });
            const m = appState.members.find(x => x.id === activeMemberId);
            if (mode !== 'modal' && m) {
                const label = mode === 'o' ? '◯' : mode === 'm' ? '△' : '×';
                showToast(`${m.avatar} ${m.name} の連続「${label}」スタンプモード中！日付をタップしてください`);
            }
        };

        window.handleCalendarDayClick = function(dateKey) {
            if (quickStampMode !== 'modal') {
                if (!appState.schedules[dateKey]) appState.schedules[dateKey] = {};
                const currentVal = appState.schedules[dateKey][activeMemberId];
                appState.schedules[dateKey][activeMemberId] = currentVal === quickStampMode ? '' : quickStampMode;

                const matchStatus = evaluateDayMatch(appState.schedules[dateKey]);
                playUiSound(matchStatus !== 'none' ? 'match' : 'tap');
                pushStateToCloud();

                // Automatically notify Discord ONLY if all 3 members now match!
                if (matchStatus !== 'none') {
                    checkAndTriggerDiscordMatchNotification(dateKey, false);
                }
                return;
            }
            openDayModal(dateKey);
        };

        window.quickFillAvailableForActiveMember = function() {
            const base = new Date(today.getFullYear(), today.getMonth(), today.getDate());
            const dow = base.getDay(); // 0:Sun, 1:Mon, ... 5:Fri, 6:Sat

            // Determine the Friday of the current/upcoming weekend
            let daysUntilFriday = 5 - dow;
            if (dow === 6) {
                daysUntilFriday = -1; // Saturday -> include yesterday(Fri), today(Sat), tomorrow(Sun)
            } else if (dow === 0) {
                daysUntilFriday = 5;  // Sunday night -> target the upcoming Fri/Sat/Sun
            }

            const weekendKeys = [];
            for (let i = 0; i < 3; i++) {
                const targetDate = new Date(base);
                targetDate.setDate(base.getDate() + daysUntilFriday + i);
                // Only include dates that haven't passed yet
                if (targetDate >= base) {
                    weekendKeys.push(formatDateKey(targetDate.getFullYear(), targetDate.getMonth(), targetDate.getDate()));
                }
            }

            // Switch calendar view to the month of the target weekend
            if (weekendKeys.length > 0) {
                const parts = weekendKeys[0].split('-');
                viewYear = parseInt(parts[0], 10);
                viewMonth = parseInt(parts[1], 10) - 1;
            }

            // Toggle behavior: if all target days already have 'o', clear them; otherwise set 'o'
            const allAlreadyCircle = weekendKeys.every(k => appState.schedules[k] && appState.schedules[k][activeMemberId] === 'o');
            const m = appState.members.find(x => x.id === activeMemberId);

            weekendKeys.forEach(k => {
                if (!appState.schedules[k]) appState.schedules[k] = {};
                appState.schedules[k][activeMemberId] = allAlreadyCircle ? '' : 'o';

                if (!allAlreadyCircle && evaluateDayMatch(appState.schedules[k]) !== 'none') {
                    checkAndTriggerDiscordMatchNotification(k, false);
                }
            });

            playUiSound(allAlreadyCircle ? 'tap' : 'match');
            pushStateToCloud();

            const dateLabels = weekendKeys.map(k => formatJapaneseDate(k)).join('・');
            if (allAlreadyCircle) {
                showToast(`${m.name} の今週末（${dateLabels}）の「◯」を解除しました`);
            } else {
                showToast(`${m.name} の今週末（${dateLabels}）だけに「◯」を入力しました！`);
            }
        };

        window.clearCurrentMonthForActiveMember = function() {
            const daysInMonth = new Date(viewYear, viewMonth + 1, 0).getDate();
            let cleared = 0;
            for (let d = 1; d <= daysInMonth; d++) {
                const key = formatDateKey(viewYear, viewMonth, d);
                if (appState.schedules[key] && appState.schedules[key][activeMemberId]) {
                    appState.schedules[key][activeMemberId] = '';
                    cleared++;
                }
            }
            playUiSound('tap');
            pushStateToCloud();
            const m = appState.members.find(x => x.id === activeMemberId);
            showToast(`${m.name} の ${viewMonth + 1}月分の予定（${cleared}日分）をクリアしました`);
        };

        function renderMatchedDaysList() {
            const container = document.getElementById('matchedDaysList');
            const allKeys = Object.keys(appState.schedules).sort();
            const matched = allKeys.filter(k => evaluateDayMatch(appState.schedules[k]) !== 'none');

            // Update Hero Banner
            const headline = document.getElementById('nextMatchHeadline');
            const subtext = document.getElementById('nextMatchSubtext');

            if (matched.length > 0) {
                const nextKey = matched[0];
                const rec = appState.schedules[nextKey];
                const game = rec.gameId ? appState.games.find(g => g.id === rec.gameId) : null;
                headline.innerHTML = `🔥 次回の3人集合可能日は <span class="text-emerald-400 underline decoration-emerald-400/50">${formatJapaneseDate(nextKey)}</span> (${rec.time || '時間自由'})！`;
                subtext.textContent = game
                    ? `予定タイトル: 「${game.title}」 / 他にも計 ${matched.length} 日がマッチしています！`
                    : `現在 ${matched.length} 日間、3人全員の予定が合っています！遊ぶゲームを割り当てましょう。`;
            } else {
                headline.textContent = 'カレンダーの日付をタップして3人の予定を入れよう！';
                subtext.textContent = '3人全員が「◯」または「△」の日はネオン枠で自動ハイライトされます。';
            }

            if (matched.length === 0) {
                container.innerHTML = `
                    <div class="col-span-full text-center py-6 text-xs text-slate-400 bg-slate-950/50 rounded-xl border border-slate-800">
                        まだ3人全員が揃う日がありません。上のカレンダーをクリックして「◯」や「△」を入力してみましょう！
                    </div>
                `;
                return;
            }

            container.innerHTML = matched.map(dateKey => {
                const rec = appState.schedules[dateKey];
                const matchType = evaluateDayMatch(rec);
                const game = rec.gameId ? appState.games.find(g => g.id === rec.gameId) : null;

                return `
                    <div onclick="openDayModal('${dateKey}')" class="cursor-pointer p-3.5 rounded-xl bg-slate-900/90 border ${matchType === 'perfect' ? 'border-emerald-500/60' : 'border-amber-500/50'} hover:bg-slate-800/80 transition flex items-center justify-between gap-3">
                        <div class="space-y-1 min-w-0">
                            <div class="flex items-center gap-2">
                                <span class="text-sm font-black text-white">${formatJapaneseDate(dateKey)}</span>
                                <span class="text-[10px] font-black px-2 py-0.5 rounded-full ${matchType === 'perfect' ? 'bg-emerald-400 text-slate-950' : 'bg-amber-400 text-slate-950'}">
                                    ${matchType === 'perfect' ? '全員◯ マッチ!' : '3人集合可(△含)'}
                                </span>
                            </div>
                            <div class="text-xs text-slate-300 truncate">
                                <i class="fa-regular fa-clock text-indigo-400 mr-1"></i>${escapeHtml(rec.time || '開始時間: 未設定')}
                            </div>
                            <div class="text-xs font-bold text-indigo-300 truncate">
                                <i class="fa-solid fa-gamepad mr-1"></i>${game ? escapeHtml(game.title) : 'タップして遊ぶゲームを選択'}
                            </div>
                        </div>
                        <i class="fa-solid fa-pen-to-square text-slate-400 shrink-0"></i>
                    </div>
                `;
            }).join('');
        }

        // ------------------------------------------
        // 6. DAY MODAL OPERATIONS
        // ------------------------------------------
        window.openDayModal = function(dateKey) {
            editingDateKey = dateKey;
            const rec = appState.schedules[dateKey] || {};
            document.getElementById('modalDateTitle').textContent = `${formatJapaneseDate(dateKey)} の予定調整`;

            const matchType = evaluateDayMatch(rec);
            const badge = document.getElementById('modalDateMatchBadge');
            if (matchType === 'perfect') {
                badge.className = 'text-[10px] font-black px-2.5 py-0.5 rounded-full bg-emerald-400 text-slate-950';
                badge.textContent = '🎉 3人全員「◯」FULL PARTY MATCH!';
            } else if (matchType === 'chance') {
                badge.className = 'text-[10px] font-black px-2.5 py-0.5 rounded-full bg-amber-400 text-slate-950';
                badge.textContent = '⚡ 3人集合可能 (時間調整)';
            } else {
                badge.className = 'text-[10px] font-black px-2.5 py-0.5 rounded-full bg-slate-800 text-slate-300';
                badge.textContent = '3人の予定ステータス';
            }

            // Populate 3 members toggles
            const listEl = document.getElementById('modalMembersScheduleList');
            listEl.innerHTML = appState.members.map(m => {
                const val = rec[m.id] || '';
                return `
                    <div class="flex items-center justify-between bg-slate-900 p-2.5 rounded-xl border border-slate-800">
                        <div class="flex items-center gap-2">
                            ${renderAvatarHtml(m.avatar, 'w-6 h-6 text-lg')}
                            <span class="text-xs sm:text-sm font-bold text-white">${escapeHtml(m.name)}</span>
                        </div>
                        <div class="flex items-center gap-1.5" data-member-group="${m.id}">
                            <button type="button" onclick="setModalMemberStatus('${m.id}', 'o')" id="modalBtn-${m.id}-o" class="w-10 py-1.5 rounded-lg text-xs font-black border transition ${val === 'o' ? 'bg-emerald-500 text-slate-950 border-emerald-400' : 'bg-slate-950 text-slate-400 border-slate-800'}">◯</button>
                            <button type="button" onclick="setModalMemberStatus('${m.id}', 'm')" id="modalBtn-${m.id}-m" class="w-10 py-1.5 rounded-lg text-xs font-black border transition ${val === 'm' ? 'bg-amber-400 text-slate-950 border-amber-300' : 'bg-slate-950 text-slate-400 border-slate-800'}">△</button>
                            <button type="button" onclick="setModalMemberStatus('${m.id}', 'x')" id="modalBtn-${m.id}-x" class="w-10 py-1.5 rounded-lg text-xs font-black border transition ${val === 'x' ? 'bg-rose-500 text-white border-rose-400' : 'bg-slate-950 text-slate-400 border-slate-800'}">×</button>
                        </div>
                    </div>
                `;
            }).join('');

            // Populate Game Dropdown with Active Games, Archived Games, and "Other" option
            populateDayModalGameDropdown(rec.gameId);

            document.getElementById('modalDayTimeInput').value = rec.time || '';
            document.getElementById('modalInlineGameAdder').classList.add('hidden');

            // Show or hide the Discord Match Notice bar inside Day Modal depending on whether all 3 match
            const discordRow = document.getElementById('modalDiscordMatchedNotice');
            if (discordRow) {
                if (matchType !== 'none') {
                    discordRow.classList.remove('hidden');
                } else {
                    discordRow.classList.add('hidden');
                }
            }

            const modal = document.getElementById('dayModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        };

        function populateDayModalGameDropdown(selectedGameId) {
            const gameSelect = document.getElementById('modalDayGameSelect');
            if (!gameSelect) return;

            const activeGames = appState.games.filter(g => g.status !== 'cleared' && g.platform !== 'その他');
            const otherOptions = appState.games.filter(g => g.platform === 'その他');
            const archivedGames = appState.games.filter(g => g.status === 'cleared' && g.platform !== 'その他');

            let html = `<option value="">未定（投票リスト・その他から選択）</option>`;

            if (activeGames.length > 0) {
                html += `<optgroup label="🔥 投票ボードのゲーム">`;
                activeGames.forEach(g => {
                    html += `<option value="${g.id}" ${selectedGameId === g.id ? 'selected' : ''}>${escapeHtml(g.title)} (🔥${g.votes?.length || 0}/3)</option>`;
                });
                html += `</optgroup>`;
            }

            if (otherOptions.length > 0) {
                html += `<optgroup label="🎲 その他の選択肢・自由枠">`;
                otherOptions.forEach(g => {
                    html += `<option value="${g.id}" ${selectedGameId === g.id ? 'selected' : ''}>${escapeHtml(g.title)}</option>`;
                });
                html += `</optgroup>`;
            }

            if (archivedGames.length > 0) {
                html += `<optgroup label="🏆 殿堂入り・以前遊んだゲーム">`;
                archivedGames.forEach(g => {
                    html += `<option value="${g.id}" ${selectedGameId === g.id ? 'selected' : ''}>${escapeHtml(g.title)}</option>`;
                });
                html += `</optgroup>`;
            }

            html += `<option value="__ADD_NEW__">＋ 新しいゲームや予定を検索して追加...</option>`;
            gameSelect.innerHTML = html;
        }

        window.handleModalGameSelectChange = function(val) {
            if (val === '__ADD_NEW__') {
                document.getElementById('modalDayGameSelect').value = '';
                const adder = document.getElementById('modalInlineGameAdder');
                adder.classList.remove('hidden');
                document.getElementById('modalInlineSearchInput').focus();
            }
        };

        window.toggleModalInlineGameAdder = function() {
            const adder = document.getElementById('modalInlineGameAdder');
            adder.classList.toggle('hidden');
            if (!adder.classList.contains('hidden')) {
                document.getElementById('modalInlineSearchInput').focus();
            }
        };

        window.selectOrAddOtherOptionInModal = function(optionId, title, platform) {
            let existing = appState.games.find(g => g.id === optionId || g.title === title);
            if (!existing) {
                existing = {
                    id: optionId,
                    title: title,
                    platform: platform || 'その他',
                    imageUrl: `https://placehold.co/200x200/3b0764/f472b6?text=${encodeURIComponent(title.slice(0, 8))}`,
                    votes: [activeMemberId],
                    suggestedBy: activeMemberId,
                    status: 'want'
                };
                appState.games.unshift(existing);
            }
            populateDayModalGameDropdown(existing.id);
            playUiSound('tap');
            showToast(`「${title}」を選択しました！`);
        };

        window.searchInlineForDayModal = async function() {
            const input = document.getElementById('modalInlineSearchInput');
            const term = input.value.trim();
            if (!term) return;
            const resBox = document.getElementById('modalInlineSearchResults');
            resBox.innerHTML = `<div class="col-span-full text-xs text-indigo-300 py-2"><i class="fa-solid fa-spinner fa-spin mr-1"></i>ネットから「${escapeHtml(term)}」のアイコンを検索中...</div>`;

            const results = await fetchGameIconsFromWeb(term, 4);
            results.push({
                title: term,
                imageUrl: `https://placehold.co/200x200/312e81/a5b4fc?text=${encodeURIComponent(term.slice(0, 8))}`,
                source: '自由入力'
            });

            window._modalInlineCandidates = results;
            resBox.innerHTML = results.map((r, i) => `
                <button type="button" onclick="pickInlineGameForDayModal(${i})" class="p-2 rounded-lg bg-slate-950 hover:bg-indigo-950 border border-slate-800 flex items-center gap-2 text-left transition">
                    <img src="${escapeHtml(r.imageUrl)}" onerror="this.src='https://placehold.co/80x80/1e1b4b/a5b4fc?text=G'" class="w-8 h-8 rounded-lg object-cover shrink-0">
                    <div class="min-w-0 flex-1">
                        <div class="text-xs font-bold text-white truncate">${escapeHtml(r.title)}</div>
                        <div class="text-[10px] text-indigo-400">タップしてこの日にセット</div>
                    </div>
                </button>
            `).join('');
        };

        window.pickInlineGameForDayModal = function(idx) {
            const item = (window._modalInlineCandidates || [])[idx];
            if (!item) return;
            const newGame = {
                id: 'g_' + Date.now(),
                title: item.title,
                platform: 'Crossplay',
                imageUrl: item.imageUrl,
                votes: [activeMemberId],
                suggestedBy: activeMemberId,
                status: 'playing'
            };
            appState.games.unshift(newGame);
            populateDayModalGameDropdown(newGame.id);
            document.getElementById('modalInlineGameAdder').classList.add('hidden');
            playUiSound('vote');
            showToast(`「${newGame.title}」をリストに追加して選択しました！`);
        };

        window.setModalMemberStatus = function(memberId, status) {
            if (!editingDateKey) return;
            if (!appState.schedules[editingDateKey]) appState.schedules[editingDateKey] = {};
            const current = appState.schedules[editingDateKey][memberId];
            appState.schedules[editingDateKey][memberId] = current === status ? '' : status;
            playUiSound('tap');
            openDayModal(editingDateKey); // Re-render modal buttons
        };

        window.saveDayModalChanges = function() {
            if (!editingDateKey) return;
            const targetKey = editingDateKey;
            if (!appState.schedules[targetKey]) appState.schedules[targetKey] = {};
            appState.schedules[targetKey].gameId = document.getElementById('modalDayGameSelect').value;
            appState.schedules[targetKey].time = document.getElementById('modalDayTimeInput').value.trim();

            const matchType = evaluateDayMatch(appState.schedules[targetKey]);
            playUiSound(matchType !== 'none' ? 'match' : 'tap');
            closeDayModal();
            pushStateToCloud();
            showToast(`${formatJapaneseDate(targetKey)} の予定を更新しました！`);

            // Trigger Discord auto-notification ONLY when all 3 members' schedules match
            if (matchType !== 'none') {
                checkAndTriggerDiscordMatchNotification(targetKey, false);
            }
        };

        window.closeDayModal = function() {
            const modal = document.getElementById('dayModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
            editingDateKey = null;
        };

        // ------------------------------------------
        // 7. INTERNET GAME SEARCH & CURATED ONLINE CATALOG (iTunes JP + CheapShark Steam API)
        // ------------------------------------------
        async function fetchGameIconsFromWeb(term, limit = 6) {
            const combined = [];
            try {
                const itunesUrl = `https://itunes.apple.com/search?term=${encodeURIComponent(term)}&entity=software&country=jp&limit=${limit}`;
                const cheapSharkUrl = `https://www.cheapshark.com/api/1.0/games?title=${encodeURIComponent(term)}&limit=${limit}`;

                const [itunesData, steamData] = await Promise.all([
                    fetch(itunesUrl).then(r => r.json()).catch(() => ({ results: [] })),
                    fetch(cheapSharkUrl).then(r => r.json()).catch(() => [])
                ]);

                if (itunesData && Array.isArray(itunesData.results)) {
                    itunesData.results.forEach(item => {
                        combined.push({
                            title: item.trackName,
                            imageUrl: item.artworkUrl512 || item.artworkUrl100,
                            source: 'App Store JP'
                        });
                    });
                }

                if (Array.isArray(steamData)) {
                    steamData.forEach(item => {
                        combined.push({
                            title: item.external,
                            imageUrl: item.thumb,
                            source: 'Steam / PC'
                        });
                    });
                }
            } catch (e) {
                console.warn("Icon fetch warning:", e);
            }
            return combined;
        }

        window.loadCatalogCategory = function(categoryKey) {
            currentCatalogCategory = categoryKey;
            ['fps_action', 'party_switch', 'coop_survival', 'mobile_cross', 'other_activities'].forEach(k => {
                const btn = document.getElementById(`catTab-${k}`);
                if (!btn) return;
                if (k === categoryKey) {
                    btn.className = 'cat-tab-btn px-3 py-1.5 rounded-xl text-xs font-black bg-indigo-600 text-white shadow-md shadow-indigo-600/30 transition';
                } else if (k === 'other_activities') {
                    btn.className = 'cat-tab-btn px-3 py-1.5 rounded-xl text-xs font-bold bg-amber-500/20 text-amber-300 border border-amber-500/30 hover:bg-amber-500/30 transition';
                } else {
                    btn.className = 'cat-tab-btn px-3 py-1.5 rounded-xl text-xs font-bold bg-slate-900 text-slate-300 hover:bg-slate-800 transition';
                }
            });
            playUiSound('tap');
            renderCatalogList(categoryKey);
        };

        async function renderCatalogList(categoryKey) {
            const grid = document.getElementById('catalogItemsGrid');
            if (!grid) return;
            const items = CURATED_GAME_CATALOG[categoryKey] || [];

            grid.innerHTML = items.map((item, idx) => {
                const cachedIcon = item.searchKey ? iconFetchCache[item.searchKey] : null;
                const displayIcon = cachedIcon || item.fallback;
                const alreadyInBoard = appState.games.some(g => g.title.toLowerCase() === item.title.toLowerCase());

                return `
                    <div class="bg-slate-900/90 border ${alreadyInBoard ? 'border-emerald-500/50' : 'border-slate-800 hover:border-indigo-500/60'} rounded-xl p-2.5 flex items-center gap-3 transition">
                        <img
                            id="catalogIcon-${categoryKey}-${idx}"
                            src="${escapeHtml(displayIcon)}"
                            onerror="this.src='${escapeHtml(item.fallback)}'"
                            class="w-12 h-12 rounded-xl object-cover shrink-0 border border-slate-700 bg-slate-950"
                        >
                        <div class="min-w-0 flex-1">
                            <div class="flex items-center gap-1">
                                <span class="text-[10px] font-bold px-1.5 py-0.2 rounded bg-slate-800 text-indigo-300">${escapeHtml(item.platform)}</span>
                                ${alreadyInBoard ? '<span class="text-[10px] font-black text-emerald-400">登録済</span>' : ''}
                            </div>
                            <div class="text-xs font-black text-white truncate mt-0.5" title="${escapeHtml(item.title)}">${escapeHtml(item.title)}</div>
                            <button
                                onclick="addCatalogItemToBoard('${categoryKey}', ${idx})"
                                class="mt-1 px-2.5 py-1 rounded-lg ${alreadyInBoard ? 'bg-emerald-600/30 text-emerald-200 border border-emerald-500/40' : 'bg-indigo-600 hover:bg-indigo-500 text-white'} font-bold text-[11px] inline-flex items-center gap-1 transition"
                            >
                                <i class="fa-solid ${alreadyInBoard ? 'fa-fire' : 'fa-plus'}"></i>
                                <span>${item.searchKey === 'CUSTOM_MODAL' ? '自由入力を開く' : alreadyInBoard ? '自分も投票🔥' : 'リストに登録'}</span>
                            </button>
                        </div>
                    </div>
                `;
            }).join('');

            // Automatically fetch real app icons from iTunes JP in the background for items not yet cached
            items.forEach(async (item, idx) => {
                if (!item.searchKey || item.searchKey === 'CUSTOM_MODAL' || iconFetchCache[item.searchKey]) return;
                try {
                    const url = `https://itunes.apple.com/search?term=${encodeURIComponent(item.searchKey)}&entity=software&country=jp&limit=1`;
                    const res = await fetch(url).then(r => r.json());
                    if (res && res.results && res.results[0]) {
                        const realIcon = res.results[0].artworkUrl512 || res.results[0].artworkUrl100;
                        if (realIcon) {
                            iconFetchCache[item.searchKey] = realIcon;
                            const imgEl = document.getElementById(`catalogIcon-${categoryKey}-${idx}`);
                            if (imgEl) imgEl.src = realIcon;
                        }
                    }
                } catch (e) {
                    // Keep fallback icon on network restriction
                }
            });
        }

        window.addCatalogItemToBoard = function(categoryKey, idx) {
            const items = CURATED_GAME_CATALOG[categoryKey] || [];
            const item = items[idx];
            if (!item) return;

            if (item.searchKey === 'CUSTOM_MODAL') {
                openCustomGameModal();
                return;
            }

            const existing = appState.games.find(g => g.title.toLowerCase() === item.title.toLowerCase());
            if (existing) {
                if (!Array.isArray(existing.votes)) existing.votes = [];
                if (!existing.votes.includes(activeMemberId)) {
                    existing.votes.push(activeMemberId);
                }
                if (existing.status === 'cleared') existing.status = 'playing'; // Revive if archived
                playUiSound('vote');
                pushStateToCloud();
                showToast(`「${existing.title}」にやりたい投票🔥を追加しました！`);
                return;
            }

            const iconUrl = (item.searchKey && iconFetchCache[item.searchKey]) ? iconFetchCache[item.searchKey] : item.fallback;
            const newGame = {
                id: 'g_' + Date.now(),
                title: item.title,
                platform: item.platform || 'Crossplay',
                imageUrl: iconUrl,
                votes: [activeMemberId],
                suggestedBy: activeMemberId,
                status: 'want'
            };

            appState.games.unshift(newGame);
            playUiSound('vote');
            pushStateToCloud();
            showToast(`「${item.title}」を投票ボードに追加しました！🔥`);
        };

        window.quickSearchTerm = function(term) {
            document.getElementById('gameSearchInput').value = term;
            searchGamesFromInternet();
        };

        window.searchGamesFromInternet = async function() {
            const queryInput = document.getElementById('gameSearchInput');
            const term = queryInput.value.trim();
            if (!term) {
                showToast('検索したいゲーム名を入力してください');
                return;
            }

            const resultsContainer = document.getElementById('searchResultsContainer');
            const resultsGrid = document.getElementById('searchResultsGrid');
            const statusText = document.getElementById('searchStatusText');
            const searchBtn = document.getElementById('searchGameBtn');

            resultsContainer.classList.remove('hidden');
            statusText.innerHTML = `<i class="fa-solid fa-spinner fa-spin mr-1"></i>「${escapeHtml(term)}」のアイコンとタイトルをネットから取得中...`;
            resultsGrid.innerHTML = '';
            searchBtn.disabled = true;

            let combinedResults = [];
            try {
                combinedResults = await fetchGameIconsFromWeb(term, 8);
            } finally {
                searchBtn.disabled = false;
            }

            // Always include a direct quick-add card with the exact search query at the end
            combinedResults.push({
                title: term,
                imageUrl: `https://placehold.co/200x200/312e81/a5b4fc?text=${encodeURIComponent(term.slice(0, 10))}`,
                source: 'そのままタイトル登録'
            });

            statusText.textContent = `「${term}」のネット検索リスト (${combinedResults.length}件) - タップで投票ボードに登録`;

            resultsGrid.innerHTML = combinedResults.map((item, idx) => `
                <div class="bg-slate-950 border border-slate-800 hover:border-indigo-500 rounded-xl p-2.5 flex items-center gap-3 transition">
                    <img
                        src="${escapeHtml(item.imageUrl)}"
                        onerror="this.src='https://placehold.co/120x120/1e1b4b/a5b4fc?text=GAME'"
                        class="w-14 h-14 rounded-xl object-cover shrink-0 border border-slate-700"
                    >
                    <div class="min-w-0 flex-1">
                        <div class="text-[10px] font-bold text-indigo-400">${escapeHtml(item.source)}</div>
                        <div class="text-xs font-black text-white truncate" title="${escapeHtml(item.title)}">${escapeHtml(item.title)}</div>
                        <button
                            onclick="addFetchedGame(${idx})"
                            class="mt-1.5 px-2.5 py-1 rounded-lg bg-indigo-600 hover:bg-indigo-500 text-white font-bold text-[11px] inline-flex items-center gap-1 transition"
                        >
                            <i class="fa-solid fa-plus"></i> リストに登録
                        </button>
                    </div>
                </div>
            `).join('');

            window._latestFetchedGames = combinedResults;
        };

        window.addFetchedGame = function(index) {
            const list = window._latestFetchedGames || [];
            const item = list[index];
            if (!item) return;

            const platform = document.getElementById('searchPlatformSelect').value || 'Crossplay';
            const newGame = {
                id: 'g_' + Date.now(),
                title: item.title,
                platform: platform,
                imageUrl: item.imageUrl,
                votes: [activeMemberId],
                suggestedBy: activeMemberId,
                status: 'want'
            };

            appState.games.unshift(newGame);
            playUiSound('vote');
            pushStateToCloud();
            showToast(`「${item.title}」を投票ボードに追加しました！🔥`);
        };

        window.closeSearchResults = function() {
            document.getElementById('searchResultsContainer').classList.add('hidden');
        };

        // ------------------------------------------
        // 8. GAME VOTING BOARD & LIFECYCLE FILTERS
        // ------------------------------------------
        window.setGameFilter = function(filter) {
            currentGameFilter = filter;
            ['all', 'unanimous', 'playing', 'other', 'cleared'].forEach(f => {
                const btn = document.getElementById(`filterBtn-${f}`);
                if (!btn) return;
                if (f === filter) {
                    btn.className = 'px-3 py-1.5 rounded-lg font-black bg-indigo-600 text-white transition';
                } else {
                    btn.className = 'px-3 py-1.5 rounded-lg font-bold text-slate-300 hover:bg-slate-800 transition';
                }
            });
            renderGamesVotingBoard();
        };

        function renderGamesVotingBoard() {
            const grid = document.getElementById('gamesVotingGrid');
            let games = [...appState.games];

            // Sort by vote count descending
            games.sort((a, b) => (b.votes?.length || 0) - (a.votes?.length || 0));

            if (currentGameFilter === 'all') {
                // Active games (exclude archived/cleared so changing games stays clean)
                games = games.filter(g => g.status !== 'cleared');
            } else if (currentGameFilter === 'unanimous') {
                games = games.filter(g => (g.votes?.length || 0) >= 3 && g.status !== 'cleared');
            } else if (currentGameFilter === 'playing') {
                games = games.filter(g => g.status === 'playing');
            } else if (currentGameFilter === 'other') {
                games = games.filter(g => g.platform === 'その他');
            } else if (currentGameFilter === 'cleared') {
                games = games.filter(g => g.status === 'cleared');
            }

            if (games.length === 0) {
                grid.innerHTML = `
                    <div class="col-span-full bg-gaming-card rounded-2xl border border-gaming-border p-8 text-center text-sm text-slate-400">
                        該当する項目がありません。上の「カタログから選ぶ」や「ネット検索」から追加してみましょう！
                    </div>
                `;
                return;
            }

            grid.innerHTML = games.map(g => {
                const votes = g.votes || [];
                const isUnanimous = votes.length >= 3;
                const hasVoted = votes.includes(activeMemberId);
                const suggester = appState.members.find(m => m.id === g.suggestedBy) || appState.members[0];
                const isOtherCategory = g.platform === 'その他';

                return `
                    <div class="rounded-2xl bg-gaming-card border ${isUnanimous ? 'glow-unanimous' : isOtherCategory ? 'border-amber-500/40' : 'border-gaming-border'} p-4 flex flex-col justify-between gap-4 transition relative overflow-hidden">
                        <!-- Top Info Row -->
                        <div class="flex items-start gap-3.5">
                            <img
                                src="${escapeHtml(g.imageUrl)}"
                                onerror="this.src='https://placehold.co/160x160/1e1b4b/a5b4fc?text=GAME'"
                                class="w-20 h-20 rounded-2xl object-cover border border-slate-700 shadow-md shrink-0"
                            >
                            <div class="min-w-0 flex-1 space-y-1.5">
                                <div class="flex items-center flex-wrap gap-1.5">
                                    <span class="px-2 py-0.5 rounded-md ${isOtherCategory ? 'bg-amber-500/20 text-amber-300 border-amber-500/40' : 'bg-slate-800 text-indigo-300 border-slate-700'} font-bold text-[10px] border">
                                        ${escapeHtml(g.platform || 'Crossplay')}
                                    </span>
                                    ${isUnanimous ? `
                                        <span class="px-2 py-0.5 rounded-md bg-pink-500 text-white font-black text-[10px] animate-pulse">
                                            🔥 3/3 満場一致！
                                        </span>
                                    ` : ''}
                                    ${g.status === 'playing' ? `
                                        <span class="px-2 py-0.5 rounded-md bg-emerald-500/20 text-emerald-300 font-bold text-[10px] border border-emerald-500/40">
                                            🎮 いま遊んでる
                                        </span>
                                    ` : g.status === 'cleared' ? `
                                        <span class="px-2 py-0.5 rounded-md bg-slate-800 text-slate-300 font-bold text-[10px] border border-slate-600">
                                            🏆 殿堂入り・休止中
                                        </span>
                                    ` : `
                                        <span class="px-2 py-0.5 rounded-md bg-indigo-500/15 text-indigo-300 font-bold text-[10px] border border-indigo-500/30">
                                            🌱 候補・投票中
                                        </span>
                                    `}
                                </div>
                                <h4 class="font-black text-base text-white leading-snug line-clamp-2" title="${escapeHtml(g.title)}">
                                    ${escapeHtml(g.title)}
                                </h4>
                                <div class="text-[11px] text-slate-400 flex items-center gap-1">
                                    <span>提案:</span>
                                    ${renderAvatarHtml(suggester.avatar, 'w-3.5 h-3.5 text-xs')}
                                    <span>${escapeHtml(suggester.name)}</span>
                                </div>
                            </div>
                        </div>

                        <!-- 3 Members Vote Avatars & Lifecycle Status Switcher -->
                        <div class="space-y-2 bg-slate-950/90 p-3 rounded-xl border border-slate-800/80">
                            <div class="flex items-center justify-between text-xs">
                                <span class="font-bold text-slate-300">やりたい投票状況</span>
                                <span class="font-black ${isUnanimous ? 'text-pink-400' : 'text-indigo-400'}">${votes.length} / 3 人</span>
                            </div>
                            <div class="w-full h-2 rounded-full bg-slate-800 overflow-hidden">
                                <div class="h-full transition-all duration-300 ${isUnanimous ? 'bg-gradient-to-r from-pink-500 to-amber-400' : 'bg-indigo-500'}" style="width: ${(votes.length / 3) * 100}%"></div>
                            </div>
                            <div class="flex items-center justify-between pt-1 gap-1">
                                <div class="flex items-center gap-1">
                                    ${appState.members.map(m => {
                                        const mVoted = votes.includes(m.id);
                                        return `
                                            <span class="px-2 py-0.5 rounded-lg text-[11px] font-bold flex items-center gap-1 ${mVoted ? 'bg-indigo-600/30 text-white border border-indigo-400/50' : 'bg-slate-900 text-slate-600'}">
                                                ${renderAvatarHtml(m.avatar, 'w-3.5 h-3.5 text-xs')}
                                                <span>${mVoted ? '🔥' : '-'}</span>
                                            </span>
                                        `;
                                    }).join('')}
                                </div>
                                <div class="flex items-center gap-1">
                                    <button onclick="toggleGamePlayingStatus('${g.id}')" title="ブーム切替 (候補 ➔ いま遊んでる ➔ 殿堂入り/休止 ➔ 再燃!)" class="px-2 h-7 rounded-lg bg-slate-900 hover:bg-slate-800 text-slate-300 hover:text-emerald-400 text-[10px] font-bold flex items-center gap-1 border border-slate-800">
                                        <i class="fa-solid fa-rotate"></i>
                                        <span>${g.status === 'cleared' ? '再燃🔥' : g.status === 'playing' ? '休止へ' : 'プレイ中へ'}</span>
                                    </button>
                                    <button onclick="deleteGameCard('${g.id}')" title="削除" class="w-7 h-7 rounded-lg bg-slate-900 hover:bg-rose-950 text-slate-500 hover:text-rose-400 text-xs flex items-center justify-center">
                                        <i class="fa-regular fa-trash-can"></i>
                                    </button>
                                </div>
                            </div>
                        </div>

                        <!-- Vote Button for Active Member -->
                        <button
                            onclick="toggleVoteForGame('${g.id}')"
                            class="w-full py-2.5 rounded-xl font-black text-xs flex items-center justify-center gap-2 transition ${
                                hasVoted
                                    ? 'bg-gradient-to-r from-pink-600 to-indigo-600 text-white shadow-lg shadow-pink-600/25'
                                    : 'bg-slate-800 hover:bg-slate-700 text-slate-200 border border-slate-700'
                            }"
                        >
                            <i class="fa-solid fa-fire"></i>
                            <span>${hasVoted ? 'やりたい！投票済み (タップで解除)' : '自分もやりたい！に投票する 🔥'}</span>
                        </button>
                    </div>
                `;
            }).join('');
        }

        window.toggleVoteForGame = function(gameId) {
            const game = appState.games.find(g => g.id === gameId);
            if (!game) return;
            if (!Array.isArray(game.votes)) game.votes = [];

            if (game.votes.includes(activeMemberId)) {
                game.votes = game.votes.filter(id => id !== activeMemberId);
                playUiSound('tap');
            } else {
                game.votes.push(activeMemberId);
                playUiSound(game.votes.length === 3 ? 'match' : 'vote');
                if (game.votes.length === 3) {
                    showToast(`🎉 「${game.title}」が3人満場一致になりました！`);
                }
            }
            pushStateToCloud();
        };

        window.toggleGamePlayingStatus = function(gameId) {
            const game = appState.games.find(g => g.id === gameId);
            if (!game) return;
            if (game.status === 'want') {
                game.status = 'playing';
                showToast(`「${game.title}」を🎮プレイ中に変更しました`);
            } else if (game.status === 'playing') {
                game.status = 'cleared';
                showToast(`「${game.title}」を🏆クリア済に変更しました！`);
            } else {
                game.status = 'want';
            }
            playUiSound('tap');
            pushStateToCloud();
        };

        window.deleteGameCard = function(gameId) {
            appState.games = appState.games.filter(g => g.id !== gameId);
            playUiSound('tap');
            pushStateToCloud();
            showToast('ゲームをリストから削除しました');
        };

        // ------------------------------------------
        // 9. MORI-MORI EXTRA TOOLS (ROULETTE, ROLES, MEMO)
        // ------------------------------------------
        window.spinGameRoulette = function() {
            const onlyHigh = document.getElementById('rouletteOnlyHighVotes').checked;
            let pool = [...appState.games];
            if (onlyHigh) {
                const highPool = pool.filter(g => (g.votes?.length || 0) >= 2);
                if (highPool.length > 0) pool = highPool;
            }

            if (pool.length === 0) {
                showToast('まずはゲーム投票リストにタイトルを追加してください！');
                return;
            }

            const iconEl = document.getElementById('rouletteGameIcon');
            const titleEl = document.getElementById('rouletteGameTitle');
            const subEl = document.getElementById('rouletteGameSub');
            const btn = document.getElementById('spinRouletteBtn');

            btn.disabled = true;
            let ticks = 0;
            const totalTicks = 18;

            const interval = setInterval(() => {
                const randomGame = pool[Math.floor(Math.random() * pool.length)];
                iconEl.src = randomGame.imageUrl;
                titleEl.textContent = randomGame.title;
                subEl.textContent = `抽選中... (${randomGame.platform})`;
                playUiSound('tap');
                ticks++;

                if (ticks >= totalTicks) {
                    clearInterval(interval);
                    const winner = pool[Math.floor(Math.random() * pool.length)];
                    iconEl.src = winner.imageUrl;
                    titleEl.innerHTML = `🎉 今夜は「<span class="text-amber-400">${escapeHtml(winner.title)}</span>」に決定！`;
                    subEl.textContent = `投票数: ${winner.votes?.length || 0}/3人 ・ プラットフォーム: ${winner.platform}`;
                    btn.disabled = false;
                    playUiSound('match');
                }
            }, 90);
        };

        window.shuffleThreeRoles = function(mode) {
            const rolePresets = {
                rpg: ['⚔️ 前衛・アタッカー', '🛡️ タンク・囮役', '💚 後衛・サポート'],
                host: ['👑 部屋立てホスト', '🧭 作戦リーダー', '🎉 ムードメーカー'],
                '1v2': ['😈 ボス・鬼役 (1人)', '🤝 挑戦者ペアA', '🤝 挑戦者ペアB']
            };
            const roles = [...(rolePresets[mode] || rolePresets.rpg)];
            // Fisher-Yates shuffle
            for (let i = roles.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [roles[i], roles[j]] = [roles[j], roles[i]];
            }

            const container = document.getElementById('roleShuffleResults');
            container.innerHTML = appState.members.map((m, idx) => `
                <div class="bg-slate-950 p-3 rounded-xl border border-indigo-500/40 text-center space-y-1 flex flex-col items-center">
                    ${renderAvatarHtml(m.avatar, 'w-7 h-7 text-xl')}
                    <div class="text-xs font-bold text-slate-300 truncate max-w-full">${escapeHtml(m.name)}</div>
                    <div class="text-xs font-black text-amber-400 pt-1">${roles[idx]}</div>
                </div>
            `).join('');
            playUiSound('match');
        };

        function renderPartyTools() {
            const memoInput = document.getElementById('sharedPartyMemoInput');
            if (memoInput && document.activeElement !== memoInput) {
                memoInput.value = appState.partyMemo || '';
            }
            const counterEl = document.getElementById('sessionCounterValue');
            if (counterEl) {
                counterEl.textContent = appState.sessionCount || 0;
            }
            const roleContainer = document.getElementById('roleShuffleResults');
            if (roleContainer && !roleContainer.innerHTML.trim()) {
                shuffleThreeRoles('rpg');
            }
        }

        window.saveSharedPartyNotes = function() {
            appState.partyMemo = document.getElementById('sharedPartyMemoInput').value;
            playUiSound('tap');
            pushStateToCloud();
            showToast('3人の共有メモを同期保存しました！');
        };

        window.incrementSessionCounter = function(amount) {
            appState.sessionCount = (appState.sessionCount || 0) + amount;
            playUiSound('match');
            pushStateToCloud();
            showToast(`累計ゲーム集会が ${appState.sessionCount} 回になりました！🎉`);
        };

        window.copySummaryForLineOrDiscord = function() {
            const matchedKeys = Object.keys(appState.schedules)
                .sort()
                .filter(k => evaluateDayMatch(appState.schedules[k]) !== 'none');

            const unanimousGames = appState.games.filter(g => (g.votes?.length || 0) >= 3);

            let text = `🏯【棒木幕府 - 3人のゲーム評定＆投票】\n`;
            text += `━━━━━━━━━━━━━━\n`;
            text += `📅 3人集まれる候補日: ${matchedKeys.length > 0 ? matchedKeys.map(k => formatJapaneseDate(k)).join(' / ') : '調整中'}\n`;
            text += `🔥 3人満場一致ゲーム: ${unanimousGames.length > 0 ? unanimousGames.map(g => g.title).join('、') : '投票受付中！'}\n`;
            text += `━━━━━━━━━━━━━━\n`;
            text += `👇 予定とやりたいゲームの投票はこちら\n${window.location.href}`;

            const temp = document.createElement('textarea');
            temp.value = text;
            document.body.appendChild(temp);
            temp.select();
            document.execCommand('copy');
            document.body.removeChild(temp);

            playUiSound('match');
            showToast('LINE / Discord用の共有テキストをコピーしました！');
        };

        // ------------------------------------------
        // 9.5 BAKUFU MEMORIES (戦果・神回年表) & TREASURY (御用金・立て替え帳)
        // ------------------------------------------
        function renderBakufuMemoriesAndExpenses() {
            const mvpSelect = document.getElementById('newMemoryMvpSelect');
            if (mvpSelect) {
                mvpSelect.innerHTML = appState.members.map(m => `<option value="${m.id}">殊勲(MVP): ${escapeHtml(m.name)}</option>`).join('');
            }

            const memList = document.getElementById('bakufuMemoriesList');
            if (memList) {
                const memories = appState.memories || [];
                if (memories.length === 0) {
                    memList.innerHTML = `<div class="text-xs text-slate-500 py-3 text-center">まだ戦果記録がありません</div>`;
                } else {
                    memList.innerHTML = memories.map(item => {
                        const mvp = appState.members.find(m => m.id === item.mvpId) || appState.members[0];
                        return `
                            <div class="bg-slate-950/90 border border-slate-800 rounded-xl p-2.5 flex items-center justify-between gap-2">
                                <div class="min-w-0 flex-1">
                                    <div class="flex items-center gap-2 text-[10px] text-amber-400 font-bold">
                                        <span>📅 ${escapeHtml(item.date)}</span>
                                        <span>🏆 MVP: ${escapeHtml(mvp.name)}</span>
                                    </div>
                                    <div class="text-xs font-bold text-white mt-0.5">${escapeHtml(item.text)}</div>
                                </div>
                            </div>
                        `;
                    }).join('');
                }
            }

            const expList = document.getElementById('bakufuExpensesList');
            if (expList) {
                const expenses = appState.expenses || [];
                if (expenses.length === 0) {
                    expList.innerHTML = `<div class="text-xs text-slate-500 py-3 text-center">現在、未精算の立て替えはありません</div>`;
                } else {
                    expList.innerHTML = expenses.map(exp => {
                        const payer = appState.members.find(m => m.id === exp.payerId) || appState.members[0];
                        const perPerson = Math.round((exp.amount || 0) / 3);
                        return `
                            <div class="bg-slate-950/90 border ${exp.settled ? 'border-slate-800 opacity-50' : 'border-emerald-500/40'} rounded-xl p-2.5 flex items-center justify-between gap-2">
                                <div class="min-w-0">
                                    <div class="text-xs font-bold text-white">${escapeHtml(exp.title)} <span class="text-emerald-400 font-black">¥${Number(exp.amount).toLocaleString()}</span></div>
                                    <div class="text-[10px] text-slate-400">立替: ${escapeHtml(payer.name)} （1人あたり 約¥${perPerson.toLocaleString()}）</div>
                                </div>
                                <button onclick="toggleSettleExpense('${exp.id}')" class="px-2.5 py-1 rounded-lg text-[10px] font-black ${exp.settled ? 'bg-slate-800 text-slate-400' : 'bg-emerald-500 text-slate-950'}">
                                    ${exp.settled ? '精算済' : '精算する'}
                                </button>
                            </div>
                        `;
                    }).join('');
                }
            }
        }

        window.addBakufuMemory = function() {
            const textInput = document.getElementById('newMemoryTextInput');
            const mvpSelect = document.getElementById('newMemoryMvpSelect');
            const text = textInput.value.trim();
            if (!text) {
                showToast('戦果・神回の内容を入力してください');
                return;
            }
            if (!Array.isArray(appState.memories)) appState.memories = [];
            const now = new Date();
            appState.memories.unshift({
                id: 'mem_' + Date.now(),
                date: `${now.getFullYear()}/${now.getMonth() + 1}/${now.getDate()}`,
                text: text,
                mvpId: mvpSelect.value || activeMemberId
            });
            textInput.value = '';
            playUiSound('match');
            pushStateToCloud();
            showToast('📜 棒木幕府の年表に新たな歴史を刻みました！');
        };

        window.addBakufuExpense = function() {
            const titleEl = document.getElementById('newExpenseTitleInput');
            const amountEl = document.getElementById('newExpenseAmountInput');
            const title = titleEl.value.trim();
            const amount = parseInt(amountEl.value, 10);
            if (!title || isNaN(amount) || amount <= 0) {
                showToast('項目と金額（円）を入力してください');
                return;
            }
            if (!Array.isArray(appState.expenses)) appState.expenses = [];
            appState.expenses.unshift({
                id: 'exp_' + Date.now(),
                title,
                amount,
                payerId: activeMemberId,
                settled: false
            });
            titleEl.value = '';
            amountEl.value = '';
            playUiSound('tap');
            pushStateToCloud();
            showToast('💰 御用金（立て替え帳）に記録しました！');
        };

        window.toggleSettleExpense = function(expId) {
            const exp = (appState.expenses || []).find(e => e.id === expId);
            if (!exp) return;
            exp.settled = !exp.settled;
            playUiSound('tap');
            pushStateToCloud();
        };

        // ------------------------------------------
        // 9.8 BAKUFU ARCADE (4 MINI-GAMES) & SHOGUNATE BATTLE STATS
        // ------------------------------------------
        let currentMiniGame = 'iai';

        window.selectMiniGame = function(gameKey) {
            currentMiniGame = gameKey;
            ['iai', 'mash', 'memory', 'bomb'].forEach(k => {
                const panel = document.getElementById(`mgPanel-${k}`);
                if (panel) panel.classList.toggle('hidden', k !== gameKey);

                const tab = document.getElementById(`mgTab-${k}`);
                if (tab) {
                    tab.className = k === gameKey
                        ? 'px-3 py-2 rounded-xl text-xs font-black bg-emerald-500 text-slate-950 transition flex items-center gap-1.5 shadow-md'
                        : 'px-3 py-2 rounded-xl text-xs font-bold text-slate-300 hover:bg-slate-800 transition flex items-center gap-1.5';
                }
            });
            playUiSound('tap');
            if (gameKey === 'memory' && (!window._memoryCards || window._memoryCards.length === 0)) {
                initMemoryGame();
            }
            if (gameKey === 'bomb' && (!window._bombWires || window._bombWires.length === 0)) {
                initBombGame();
            }
        };

        function ensureArcadeAndBattleState() {
            if (!appState.arcadeScores) appState.arcadeScores = {};
            if (!appState.battleStats) appState.battleStats = {};
            appState.members.forEach(m => {
                if (!appState.arcadeScores[m.id]) {
                    appState.arcadeScores[m.id] = { iaiBestMs: null, mashBestCount: 0, memoryBestMoves: null };
                }
                if (!appState.battleStats[m.id]) {
                    appState.battleStats[m.id] = { wins: 0, carries: 0, trolls: 0 };
                }
            });
        }

        function renderArcadeLeaderboard() {
            ensureArcadeAndBattleState();
            const grid = document.getElementById('arcadeLeaderboardGrid');
            if (!grid) return;

            grid.innerHTML = appState.members.map(m => {
                const sc = appState.arcadeScores[m.id] || {};
                const isActive = m.id === activeMemberId;
                return `
                    <div class="bg-slate-950/90 border ${isActive ? 'border-emerald-400/70' : 'border-slate-800'} rounded-2xl p-3.5 space-y-2">
                        <div class="flex items-center justify-between">
                            <div class="flex items-center gap-2 min-w-0">
                                ${renderAvatarHtml(m.avatar, 'w-6 h-6 text-lg')}
                                <span class="text-xs sm:text-sm font-black text-white truncate">${escapeHtml(m.name)}</span>
                            </div>
                            ${isActive ? '<span class="text-[10px] font-black px-2 py-0.5 rounded-full bg-emerald-500/20 text-emerald-300">操作中</span>' : ''}
                        </div>
                        <div class="grid grid-cols-3 gap-1.5 text-center text-[11px]">
                            <div class="bg-slate-900 p-2 rounded-xl border border-slate-800">
                                <div class="text-slate-400 text-[10px]">⚡ 居合斬り</div>
                                <div class="font-black text-amber-400 mt-0.5">${sc.iaiBestMs ? `${sc.iaiBestMs}ms` : '未記録'}</div>
                            </div>
                            <div class="bg-slate-900 p-2 rounded-xl border border-slate-800">
                                <div class="text-slate-400 text-[10px]">🥁 太鼓連打</div>
                                <div class="font-black text-pink-400 mt-0.5">${sc.mashBestCount ? `${sc.mashBestCount}回` : '未記録'}</div>
                            </div>
                            <div class="bg-slate-900 p-2 rounded-xl border border-slate-800">
                                <div class="text-slate-400 text-[10px]">🃏 絵札手数</div>
                                <div class="font-black text-indigo-300 mt-0.5">${sc.memoryBestMoves ? `${sc.memoryBestMoves}手` : '未記録'}</div>
                            </div>
                        </div>
                    </div>
                `;
            }).join('');
        }

        // --- MINI-GAME 1: IAI SLASH (REFLEX DUEL) ---
        let iaiState = 'idle'; // 'idle' | 'waiting' | 'now' | 'done'
        let iaiTimer = null;
        let iaiStartTime = 0;

        window.handleIaiArenaTap = function() {
            ensureArcadeAndBattleState();
            const box = document.getElementById('iaiArenaBox');
            const icon = document.getElementById('iaiIconDisplay');
            const main = document.getElementById('iaiMainText');
            const sub = document.getElementById('iaiSubText');

            if (iaiState === 'idle' || iaiState === 'done') {
                iaiState = 'waiting';
                box.className = 'w-full min-h-[220px] sm:min-h-[260px] rounded-2xl border-2 border-amber-500/70 bg-amber-950/30 flex flex-col items-center justify-center p-6 text-center cursor-pointer select-none transition-all duration-150';
                icon.textContent = '🧘‍♂️';
                main.textContent = '構え……（まだ押すな！）';
                sub.textContent = '画面が緑色に光って「斬れ！！」と出るまで集中して待て...';
                playUiSound('tap');

                const randomDelay = 1600 + Math.floor(Math.random() * 2600);
                clearTimeout(iaiTimer);
                iaiTimer = setTimeout(() => {
                    iaiState = 'now';
                    iaiStartTime = performance.now();
                    box.className = 'w-full min-h-[220px] sm:min-h-[260px] rounded-2xl border-4 border-emerald-400 bg-emerald-500/30 flex flex-col items-center justify-center p-6 text-center cursor-pointer select-none glow-match';
                    icon.textContent = '⚡🗡️⚡';
                    main.textContent = '斬れ！！！！（今すぐタップ！）';
                    sub.textContent = '最速で画面を叩け！';
                    playUiSound('vote');
                }, randomDelay);
                return;
            }

            if (iaiState === 'waiting') {
                // Foul / False start
                clearTimeout(iaiTimer);
                iaiState = 'done';
                box.className = 'w-full min-h-[220px] sm:min-h-[260px] rounded-2xl border-2 border-rose-500 bg-rose-950/40 flex flex-col items-center justify-center p-6 text-center cursor-pointer select-none';
                icon.textContent = '💥🙅‍♂️';
                main.textContent = 'お手付き（フライング）！！';
                sub.textContent = '合図が出る前に斬ってしまいました。もう一度タップで再挑戦！';
                return;
            }

            if (iaiState === 'now') {
                const reactionMs = Math.max(1, Math.round(performance.now() - iaiStartTime));
                iaiState = 'done';
                const member = appState.members.find(m => m.id === activeMemberId);
                const memberScore = appState.arcadeScores[activeMemberId];
                const isNewBest = !memberScore.iaiBestMs || reactionMs < memberScore.iaiBestMs;

                if (isNewBest) {
                    memberScore.iaiBestMs = reactionMs;
                    pushStateToCloud();
                }

                let rankTitle = '足軽級';
                if (reactionMs <= 160) rankTitle = '👑 天下無双・将軍級！！';
                else if (reactionMs <= 210) rankTitle = '🔥 達人・剣豪級！';
                else if (reactionMs <= 270) rankTitle = '⚔️ 熟練・侍大将！';

                box.className = 'w-full min-h-[220px] sm:min-h-[260px] rounded-2xl border-2 border-indigo-400 bg-indigo-950/50 flex flex-col items-center justify-center p-6 text-center cursor-pointer select-none';
                icon.textContent = '🏆';
                main.innerHTML = `記録: <span class="text-emerald-400 text-3xl">${reactionMs} ms</span> （${rankTitle}）`;
                sub.textContent = isNewBest
                    ? `🎉 ${member.name} の自己ベストを更新して番付に同期しました！（タップで再挑戦）`
                    : `自己ベスト: ${memberScore.iaiBestMs}ms （タップで再挑戦）`;
                playUiSound('match');
            }
        };

        // --- MINI-GAME 2: 10-SECOND TAIKO MASH ---
        let mashActive = false;
        let mashFinished = false;
        let mashCount = 0;
        let mashEndTime = 0;
        let mashInterval = null;

        window.handleMashButtonTap = function() {
            ensureArcadeAndBattleState();
            if (mashFinished) return;

            if (!mashActive) {
                mashActive = true;
                mashCount = 1;
                mashEndTime = performance.now() + 10000;
                document.getElementById('mashCountDisplay').textContent = `${mashCount} 回`;
                document.getElementById('mashBtnLabel').textContent = '連打ァァァ！！🔥';

                mashInterval = setInterval(() => {
                    const remain = Math.max(0, (mashEndTime - performance.now()) / 1000);
                    document.getElementById('mashTimerDisplay').textContent = `${remain.toFixed(2)}秒`;
                    if (remain <= 0) {
                        clearInterval(mashInterval);
                        finishMashGame();
                    }
                }, 40);
                playUiSound('tap');
                return;
            }

            mashCount++;
            document.getElementById('mashCountDisplay').textContent = `${mashCount} 回`;
            playUiSound('tap');
        };

        function finishMashGame() {
            mashActive = false;
            mashFinished = true;
            const member = appState.members.find(m => m.id === activeMemberId);
            const sc = appState.arcadeScores[activeMemberId];
            const isRecord = !sc.mashBestCount || mashCount > sc.mashBestCount;
            if (isRecord) {
                sc.mashBestCount = mashCount;
                pushStateToCloud();
            }
            document.getElementById('mashBtnLabel').textContent = isRecord
                ? `🎉 終了！新記録 ${mashCount}回 達成！（上のリセットで再挑戦）`
                : `終了！記録 ${mashCount}回（自己ベスト: ${sc.mashBestCount}回）`;
            playUiSound('match');
            showToast(`${member.name} の連打記録: ${mashCount}回！`);
        }

        window.resetMashGame = function() {
            clearInterval(mashInterval);
            mashActive = false;
            mashFinished = false;
            mashCount = 0;
            document.getElementById('mashTimerDisplay').textContent = '10.00秒';
            document.getElementById('mashCountDisplay').textContent = '0 回';
            document.getElementById('mashBtnLabel').textContent = 'ここを連打でスタート！！';
        };

        // --- MINI-GAME 3: SHOGUNATE MEMORY FLIP (神経衰弱) ---
        const MEMORY_SYMBOLS = ['🏯', '⚔️', '🐉', '🦊', '⚡', '🎮'];
        window._memoryCards = [];
        let memoryFlippedIndices = [];
        let memoryMoves = 0;
        let memoryLock = false;

        window.initMemoryGame = function() {
            const deck = [...MEMORY_SYMBOLS, ...MEMORY_SYMBOLS];
            for (let i = deck.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [deck[i], deck[j]] = [deck[j], deck[i]];
            }
            window._memoryCards = deck.map((sym, idx) => ({
                id: idx,
                symbol: sym,
                flipped: false,
                matched: false
            }));
            memoryFlippedIndices = [];
            memoryMoves = 0;
            memoryLock = false;
            const movesEl = document.getElementById('memoryMovesDisplay');
            if (movesEl) movesEl.textContent = '0';
            renderMemoryGrid();
        };

        function renderMemoryGrid() {
            const grid = document.getElementById('memoryCardsGrid');
            if (!grid) return;
            grid.innerHTML = (window._memoryCards || []).map((card, idx) => {
                const open = card.flipped || card.matched;
                return `
                    <button
                        type="button"
                        onclick="flipMemoryCard(${idx})"
                        class="h-20 sm:h-24 rounded-2xl border-2 text-2xl sm:text-3xl font-black flex items-center justify-center transition transform ${
                            card.matched
                                ? 'bg-emerald-950/60 border-emerald-400 text-white scale-95'
                                : open
                                    ? 'bg-indigo-900/80 border-indigo-400 text-white'
                                    : 'bg-slate-950 hover:bg-slate-900 border-slate-800 text-amber-400/50'
                        }"
                    >
                        ${open ? card.symbol : '⛩️'}
                    </button>
                `;
            }).join('');
        }

        window.flipMemoryCard = function(idx) {
            if (memoryLock) return;
            const cards = window._memoryCards || [];
            const target = cards[idx];
            if (!target || target.flipped || target.matched) return;

            target.flipped = true;
            memoryFlippedIndices.push(idx);
            playUiSound('tap');
            renderMemoryGrid();

            if (memoryFlippedIndices.length === 2) {
                memoryMoves++;
                document.getElementById('memoryMovesDisplay').textContent = String(memoryMoves);
                const [firstIdx, secondIdx] = memoryFlippedIndices;
                const firstCard = cards[firstIdx];
                const secondCard = cards[secondIdx];

                if (firstCard.symbol === secondCard.symbol) {
                    firstCard.matched = true;
                    secondCard.matched = true;
                    memoryFlippedIndices = [];
                    renderMemoryGrid();

                    // Check if all matched
                    if (cards.every(c => c.matched)) {
                        ensureArcadeAndBattleState();
                        const sc = appState.arcadeScores[activeMemberId];
                        const isBest = !sc.memoryBestMoves || memoryMoves < sc.memoryBestMoves;
                        if (isBest) {
                            sc.memoryBestMoves = memoryMoves;
                            pushStateToCloud();
                        }
                        playUiSound('match');
                        showToast(`🎉 全ペア制覇！記録: ${memoryMoves}手 ${isBest ? '（自己ベスト更新！）' : ''}`);
                    }
                } else {
                    memoryLock = true;
                    setTimeout(() => {
                        firstCard.flipped = false;
                        secondCard.flipped = false;
                        memoryFlippedIndices = [];
                        memoryLock = false;
                        renderMemoryGrid();
                    }, 650);
                }
            }
        };

        // --- MINI-GAME 4: BAKUDAN ROULETTE (3-PLAYER BOMB CRISIS) ---
        window._bombWires = [];
        let bombTurnIndex = 0;
        let bombGameOver = false;

        window.initBombGame = function() {
            const totalWires = 12;
            const trapIndex = Math.floor(Math.random() * totalWires);
            window._bombWires = Array.from({ length: totalWires }, (_, idx) => ({
                index: idx,
                cut: false,
                isBomb: idx === trapIndex
            }));
            bombTurnIndex = 0;
            bombGameOver = false;
            renderBombGame();
        };

        function renderBombGame() {
            const banner = document.getElementById('bombTurnBanner');
            const grid = document.getElementById('bombWiresGrid');
            if (!grid || !banner) return;

            const currentTurnMember = appState.members[bombTurnIndex % appState.members.length] || appState.members[0];
            if (!bombGameOver) {
                banner.className = 'bg-slate-950 border border-amber-500/40 rounded-xl p-3 text-center text-xs sm:text-sm font-black text-amber-300';
                banner.innerHTML = `現在の手番: ${renderAvatarHtml(currentTurnMember.avatar, 'w-5 h-5 text-base')} <span class="text-white underline">${escapeHtml(currentTurnMember.name)}</span> さん、安全な導火線を1本選んでください！`;
            }

            grid.innerHTML = (window._bombWires || []).map((wire, idx) => {
                if (wire.cut) {
                    return `
                        <div class="h-16 rounded-xl border ${wire.isBomb ? 'bg-rose-600 border-rose-300 text-white animate-bounce' : 'bg-slate-950/60 border-slate-800 text-emerald-400'} flex flex-col items-center justify-center font-black text-xs">
                            <span class="text-lg">${wire.isBomb ? '💥大爆発!!' : '✂️ SAFE'}</span>
                        </div>
                    `;
                }
                return `
                    <button
                        type="button"
                        onclick="cutBombWire(${idx})"
                        class="h-16 rounded-xl bg-slate-900 hover:bg-rose-950/50 border border-slate-700 hover:border-rose-400 text-slate-200 font-black text-xs flex flex-col items-center justify-center gap-1 transition"
                    >
                        <span class="text-base">🧨 導火線 #${idx + 1}</span>
                        <span class="text-[10px] text-slate-400">タップで切る</span>
                    </button>
                `;
            }).join('');
        }

        window.cutBombWire = function(idx) {
            if (bombGameOver) return;
            const wire = (window._bombWires || [])[idx];
            if (!wire || wire.cut) return;

            wire.cut = true;
            const currentTurnMember = appState.members[bombTurnIndex % appState.members.length] || appState.members[0];

            if (wire.isBomb) {
                bombGameOver = true;
                const banner = document.getElementById('bombTurnBanner');
                banner.className = 'bg-rose-950/80 border-2 border-rose-500 rounded-xl p-3.5 text-center text-sm sm:text-base font-black text-rose-200';
                banner.innerHTML = `💥 ドカァァン！！ <strong>${escapeHtml(currentTurnMember.name)}</strong> が爆弾を引きました！（部屋ホスト・罰ゲーム決定！）`;
                playUiSound('match');
            } else {
                bombTurnIndex++;
                playUiSound('tap');
            }
            renderBombGame();
        };

        // --- SHOGUNATE BATTLE STATS & CHALLENGE OMIKUJI ---
        function renderMemberBattleStats() {
            ensureArcadeAndBattleState();
            const grid = document.getElementById('memberBattleStatsGrid');
            if (!grid) return;

            // Compute rank points: win*3 + carry*2 - troll*1
            const scores = appState.members.map(m => {
                const st = appState.battleStats[m.id] || { wins: 0, carries: 0, trolls: 0 };
                return { id: m.id, pts: (st.wins || 0) * 3 + (st.carries || 0) * 2 - (st.trolls || 0) };
            }).sort((a, b) => b.pts - a.pts);

            const rankTitles = ['👑 征夷大将軍', '🏯 御家老 (No.2)', '⚔️ 切り込み隊長'];

            grid.innerHTML = appState.members.map(m => {
                const st = appState.battleStats[m.id] || { wins: 0, carries: 0, trolls: 0 };
                const rankIdx = scores.findIndex(s => s.id === m.id);
                const titleBadge = rankTitles[rankIdx] || '⚔️ 家臣';

                return `
                    <div class="bg-slate-950/90 border border-slate-800 rounded-2xl p-3.5 space-y-3">
                        <div class="flex items-center justify-between">
                            <div class="flex items-center gap-2 min-w-0">
                                ${renderAvatarHtml(m.avatar, 'w-6 h-6 text-lg')}
                                <span class="text-xs sm:text-sm font-black text-white truncate">${escapeHtml(m.name)}</span>
                            </div>
                            <span class="text-[10px] font-black px-2 py-0.5 rounded-full bg-amber-500/20 text-amber-300 border border-amber-500/30">${titleBadge}</span>
                        </div>
                        <div class="grid grid-cols-3 gap-1.5 text-center">
                            <button onclick="incrementBattleStat('${m.id}', 'wins')" class="p-2 rounded-xl bg-slate-900 hover:bg-emerald-950/60 border border-slate-800 hover:border-emerald-500/50 transition">
                                <div class="text-[10px] text-slate-400">🏆 勝利</div>
                                <div class="text-sm font-black text-emerald-400 mt-0.5">${st.wins || 0}</div>
                                <div class="text-[9px] text-slate-500">+1</div>
                            </button>
                            <button onclick="incrementBattleStat('${m.id}', 'carries')" class="p-2 rounded-xl bg-slate-900 hover:bg-indigo-950/60 border border-slate-800 hover:border-indigo-500/50 transition">
                                <div class="text-[10px] text-slate-400">💪 キャリー</div>
                                <div class="text-sm font-black text-indigo-400 mt-0.5">${st.carries || 0}</div>
                                <div class="text-[9px] text-slate-500">+1</div>
                            </button>
                            <button onclick="incrementBattleStat('${m.id}', 'trolls')" class="p-2 rounded-xl bg-slate-900 hover:bg-rose-950/60 border border-slate-800 hover:border-rose-500/50 transition">
                                <div class="text-[10px] text-slate-400">🤡 やらかし</div>
                                <div class="text-sm font-black text-rose-400 mt-0.5">${st.trolls || 0}</div>
                                <div class="text-[9px] text-slate-500">+1</div>
                            </button>
                        </div>
                    </div>
                `;
            }).join('');
        }

        window.incrementBattleStat = function(memberId, field) {
            ensureArcadeAndBattleState();
            appState.battleStats[memberId][field] = (appState.battleStats[memberId][field] || 0) + 1;
            playUiSound('vote');
            pushStateToCloud();
        };

        const CHALLENGE_OMIKUJI_LIST = [
            { badge: '🔥 縛りプレイお題', text: '次の1戦、全員「普段絶対に使わない武器・キャラ」で出陣せよ！' },
            { badge: '👑 将軍命令ルール', text: '次の試合で一番スコアが低かった者は、残り2人を「将軍様」と呼んで敬語で話すこと！' },
            { badge: '🤐 連携チャレンジ', text: 'カタカナ語禁止縛り！カタカナを使ったら即座にアイテムを味方に献上せよ！' },
            { badge: '🎯 1発クリア挑戦', text: '今から30分以内に目標クエスト/1勝を達成できなければ、全員でホラーゲームへ移行！' },
            { badge: '🛡️ 護衛ミッション', text: 'プレイヤー1を「将軍」とし、将軍が1回でもダウンしたら即やり直し！残り2人で全力護衛せよ！' },
            { badge: '🎲 運任せ装備', text: 'ルーレットで出た数字の順番のキャラ・武器だけで次のマッチに挑め！' },
            { badge: '🍻 ご褒美おみくじ【大吉】', text: '大吉！今日は縛りなし！好きなゲームで全員MVPを目指せ！' }
        ];

        window.drawChallengeOmikuji = function() {
            const pick = CHALLENGE_OMIKUJI_LIST[Math.floor(Math.random() * CHALLENGE_OMIKUJI_LIST.length)];
            document.getElementById('omikujiBadge').textContent = pick.badge;
            document.getElementById('omikujiResultText').textContent = pick.text;
            playUiSound('match');
        };

        // ------------------------------------------
        // 10. MODALS FOR MEMBER SETTINGS, STATUS & CUSTOM GAME
        // ------------------------------------------
        window.openMemberSettingsModal = function() {
            const container = document.getElementById('memberEditInputs');
            container.innerHTML = appState.members.map((m, idx) => `
                <div class="bg-slate-950 p-3 rounded-xl border border-slate-800 flex items-center gap-2.5">
                    <input
                        type="text"
                        id="editMemberAvatar-${idx}"
                        value="${escapeHtml(m.avatar)}"
                        maxlength="2"
                        class="w-12 h-10 text-center text-lg rounded-xl bg-slate-900 border border-slate-700 text-white"
                        title="絵文字アイコン"
                    >
                    <input
                        type="text"
                        id="editMemberName-${idx}"
                        value="${escapeHtml(m.name)}"
                        placeholder="メンバー名"
                        class="flex-1 px-3 py-2 rounded-xl bg-slate-900 border border-slate-700 text-sm text-white"
                    >
                </div>
            `).join('');
            const modal = document.getElementById('memberSettingsModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        };

        window.closeMemberSettingsModal = function() {
            const modal = document.getElementById('memberSettingsModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        };

        window.saveMemberProfiles = function() {
            const now = Date.now();
            appState.members.forEach((m, idx) => {
                const avatarVal = document.getElementById(`editMemberAvatar-${idx}`).value.trim();
                const nameVal = document.getElementById(`editMemberName-${idx}`).value.trim();
                if (avatarVal) m.avatar = avatarVal;
                if (nameVal) m.name = nameVal;
                m.updatedAt = now;
            });
            hasCompletedInitialSetup = true;
            localStorage.setItem(STORAGE_KEY_ONBOARDED, 'true');
            localStorage.setItem(STORAGE_KEY_MEMBERS, JSON.stringify(appState.members));
            saveStateToLocalStorage();

            closeMemberSettingsModal();
            playUiSound('match');
            pushStateToCloud();
            showToast('3人のプロフィールを保存しました！リロードしても維持されます');
        };

        window.openStatusUpdateModal = function() {
            const m = appState.members.find(x => x.id === activeMemberId) || appState.members[0];
            document.getElementById('statusModalMemberLabel').textContent = `${m.avatar} ${m.name} の一言ステータス`;
            document.getElementById('statusMessageInput').value = m.status || '';
            const modal = document.getElementById('statusUpdateModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        };

        window.closeStatusUpdateModal = function() {
            const modal = document.getElementById('statusUpdateModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        };

        window.setQuickStatusText = function(text) {
            document.getElementById('statusMessageInput').value = text;
        };

        window.saveStatusMessage = function() {
            const m = appState.members.find(x => x.id === activeMemberId);
            if (m) {
                m.status = document.getElementById('statusMessageInput').value.trim();
                m.updatedAt = Date.now();
            }
            saveStateToLocalStorage();
            closeStatusUpdateModal();
            playUiSound('tap');
            pushStateToCloud();
            showToast('一言ステータスを更新しました！');
        };

        window.openCustomGameModal = function() {
            document.getElementById('customGameTitleInput').value = '';
            document.getElementById('customGameImageInput').value = '';
            document.getElementById('customModalIconCandidates').classList.add('hidden');
            const modal = document.getElementById('customGameModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        };

        window.closeCustomGameModal = function() {
            const modal = document.getElementById('customGameModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        };

        window.openCustomFirebaseModal = function() {
            const modal = document.getElementById('customFirebaseModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        };

        window.closeCustomFirebaseModal = function() {
            const modal = document.getElementById('customFirebaseModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        };

        window.openQuickPublishModal = function() {
            const modal = document.getElementById('quickPublishModal');
            if (modal) {
                modal.classList.remove('hidden');
                modal.classList.add('flex');
            }
        };

        window.closeQuickPublishModal = function() {
            const modal = document.getElementById('quickPublishModal');
            if (modal) {
                modal.classList.add('hidden');
                modal.classList.remove('flex');
            }
        };

        window.downloadStandaloneHtmlFile = function() {
            try {
                const htmlContent = '<!DOCTYPE html>\n' + document.documentElement.outerHTML;
                const blob = new Blob([htmlContent], { type: 'text/html;charset=utf-8' });
                const url = URL.createObjectURL(blob);
                const a = document.createElement('a');
                a.href = url;
                a.download = 'index.html';
                document.body.appendChild(a);
                a.click();
                document.body.removeChild(a);
                URL.revokeObjectURL(url);
                playUiSound('match');
                showToast('🎉 index.html をダウンロードしました！');
            } catch (e) {
                showToast('右上のエディタからコードをコピーして保存してください');
            }
        };

        window.applyCustomFirebaseConfig = async function() {
            const raw = document.getElementById('customFirebaseConfigInput').value.trim();
            if (!raw) {
                showToast('Firebase ConfigのJSONを入力してください');
                return;
            }
            try {
                const parsed = JSON.parse(raw);
                localStorage.setItem(STORAGE_KEY_CUSTOM_FB, JSON.stringify(parsed));
                const app = initializeApp(parsed, 'customApp_' + Date.now());
                auth = getAuth(app);
                db = getFirestore(app);
                await signInAnonymously(auth);
                onAuthStateChanged(auth, (user) => {
                    currentUser = user;
                    if (user) subscribeToPartyHub();
                });
                closeCustomFirebaseModal();
                playUiSound('match');
                showToast('🎉 カスタムFirebase設定を保存し、リアルタイム同期を開始しました！');
            } catch (e) {
                showToast('⚠️ JSONの形式またはFirebase設定を確認してください');
            }
        };

        window.fillCustomModalPreset = function(title, platform, iconUrl) {
            document.getElementById('customGameTitleInput').value = title;
            document.getElementById('customGamePlatformInput').value = platform;
            document.getElementById('customGameImageInput').value = iconUrl;
            playUiSound('tap');
        };

        window.fetchIconForCustomModal = async function() {
            const title = document.getElementById('customGameTitleInput').value.trim();
            if (!title) {
                showToast('先にタイトルを入力してください');
                return;
            }
            const box = document.getElementById('customModalIconCandidates');
            const grid = document.getElementById('customModalIconGrid');
            box.classList.remove('hidden');
            grid.innerHTML = `<span class="text-xs text-slate-400"><i class="fa-solid fa-spinner fa-spin mr-1"></i>ネットからアイコン取得中...</span>`;

            const icons = await fetchGameIconsFromWeb(title, 6);
            if (icons.length === 0) {
                grid.innerHTML = `<span class="text-xs text-slate-400">アイコンが見つかりませんでした（自動でタイトル入りアイコンを生成します）</span>`;
                return;
            }

            grid.innerHTML = icons.map(item => `
                <button type="button" onclick="document.getElementById('customGameImageInput').value='${escapeHtml(item.imageUrl)}'; showToast('アイコンを選択しました！');" class="shrink-0 p-1 rounded-xl border border-slate-700 hover:border-indigo-400 bg-slate-900 transition">
                    <img src="${escapeHtml(item.imageUrl)}" class="w-12 h-12 rounded-lg object-cover">
                </button>
            `).join('');
        };

        window.addCustomGameToBoard = function() {
            const title = document.getElementById('customGameTitleInput').value.trim();
            const platform = document.getElementById('customGamePlatformInput').value;
            const statusEl = document.getElementById('customGameStatusInput');
            const status = statusEl ? statusEl.value : 'want';
            let imageUrl = document.getElementById('customGameImageInput').value.trim();

            if (!title) {
                showToast('タイトルまたは内容を入力してください');
                return;
            }
            if (!imageUrl) {
                const bgHex = platform === 'その他' ? '3b0764/f472b6' : '312e81/a5b4fc';
                imageUrl = `https://placehold.co/200x200/${bgHex}?text=${encodeURIComponent(title.slice(0, 10))}`;
            }

            appState.games.unshift({
                id: 'g_' + Date.now(),
                title,
                platform,
                imageUrl,
                votes: [activeMemberId],
                suggestedBy: activeMemberId,
                status: status
            });

            closeCustomGameModal();
            playUiSound('vote');
            pushStateToCloud();
            showToast(`「${title}」をリストに追加しました！`);
        };

        // ------------------------------------------
        // 11. NAVIGATION & HELPERS
        // ------------------------------------------
        window.switchTab = function(tabName) {
            const tabs = ['calendar', 'games', 'arcade', 'party', 'appguide'];
            tabs.forEach(t => {
                const view = document.getElementById(`view-${t}`);
                if (view) view.classList.toggle('hidden', t !== tabName);

                const deskBtn = document.getElementById(`tabBtn-${t}`);
                if (deskBtn) {
                    deskBtn.className = t === tabName
                        ? 'tab-btn px-5 py-2.5 rounded-xl font-bold text-sm flex items-center gap-2 transition bg-indigo-600 text-white shadow-lg shadow-indigo-600/30'
                        : 'tab-btn px-5 py-2.5 rounded-xl font-bold text-sm flex items-center gap-2 transition text-slate-300 hover:bg-slate-800';
                }

                const mobBtn = document.getElementById(`mobTab-${t}`);
                if (mobBtn) {
                    mobBtn.className = t === tabName
                        ? 'flex flex-col items-center justify-center py-1.5 rounded-xl text-indigo-400 bg-indigo-500/15 font-bold'
                        : 'flex flex-col items-center justify-center py-1.5 rounded-xl text-slate-400 font-bold';
                }
            });
            playUiSound('tap');
            if (tabName === 'arcade') {
                renderArcadeLeaderboard();
                selectMiniGame(currentMiniGame || 'iai');
            }
        };

        function updateGlobalCounters() {
            const matchedCount = Object.keys(appState.schedules)
                .filter(k => evaluateDayMatch(appState.schedules[k]) !== 'none').length;
            const unanimousCount = appState.games.filter(g => (g.votes?.length || 0) >= 3).length;

            document.getElementById('matchCountBadge').textContent = matchedCount;
            document.getElementById('gameCountBadge').textContent = appState.games.length;
            document.getElementById('headerMatchSummary').textContent = `${matchedCount}日`;
            document.getElementById('headerUnanimousSummary').textContent = `${unanimousCount}本`;
        }

        function formatJapaneseDate(dateKey) {
            const parts = dateKey.split('-');
            if (parts.length !== 3) return dateKey;
            const y = parseInt(parts[0], 10);
            const m = parseInt(parts[1], 10) - 1;
            const d = parseInt(parts[2], 10);
            const dowNames = ['日', '月', '火', '水', '木', '金', '土'];
            const dow = new Date(y, m, d).getDay();
            return `${m + 1}/${d}(${dowNames[dow]})`;
        }

        function escapeHtml(str) {
            if (!str) return '';
            return String(str)
                .replace(/&/g, '&amp;')
                .replace(/</g, '&lt;')
                .replace(/>/g, '&gt;')
                .replace(/"/g, '&quot;')
                .replace(/'/g, '&#039;');
        }

        function showToast(msg) {
            const box = document.getElementById('toastBox');
            const text = document.getElementById('toastMessage');
            text.textContent = msg;
            box.classList.remove('translate-y-20', 'opacity-0');
            clearTimeout(window._toastTimer);
            window._toastTimer = setTimeout(() => {
                box.classList.add('translate-y-20', 'opacity-0');
            }, 2600);
        }

        // Start App
        window.addEventListener('DOMContentLoaded', () => {
            renderAll();
            initRealtimeSync();
            // Only open initial registration modal if onboarding has not been completed yet
            setTimeout(() => {
                const savedOnboarded = localStorage.getItem(STORAGE_KEY_ONBOARDED);
                const activeMember = appState.members.find(m => m.id === activeMemberId) || appState.members[0];
                if (savedOnboarded !== 'true' && !hasCompletedInitialSetup && isDefaultMemberName(activeMember.name)) {
                    openOnboardingModal(false);
                }
            }, 350);
        });
    </script>
</body>
</html>
