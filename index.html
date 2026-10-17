```html
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>لعبة قصف جبهات - Roast Battle</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Cairo -->
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700;900&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            purple: '#6d28d9',
                            dark: '#0f172a',
                            neon: '#f59e0b',
                            pink: '#ec4899',
                            danger: '#ef4444',
                            success: '#10b981'
                        }
                    },
                    fontFamily: {
                        cairo: ['Cairo', 'sans-serif']
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Cairo', sans-serif;
            user-select: none;
            background: #090d16;
            color: #fff;
            overflow-x: hidden;
        }

        /* Screen Shake Animation */
        .shake {
            animation: shake 0.5s cubic-bezier(.36,.07,.19,.97) both;
        }

        @keyframes shake {
            10%, 90% { transform: translate3d(-2px, 0, 0); }
            20%, 80% { transform: translate3d(4px, 0, 0); }
            30%, 50%, 70% { transform: translate3d(-6px, 0, 0); }
            40%, 60% { transform: translate3d(6px, 0, 0); }
        }

        /* Exploding Animation for Head */
        .explode {
            animation: explode 0.6s ease-out forwards;
        }

        @keyframes explode {
            0% { transform: scale(1) rotate(0deg); opacity: 1; }
            50% { transform: scale(1.4) rotate(15deg); filter: hue-rotate(90deg) contrast(200%); }
            100% { transform: scale(0.8) rotate(-10deg); opacity: 1; }
        }

        /* Pulse FX */
        .pulse-bg {
            animation: pulse-bg 2s infinite alternate;
        }

        @keyframes pulse-bg {
            0% { background-color: rgba(109, 40, 217, 0.15); }
            100% { background-color: rgba(236, 72, 153, 0.25); }
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 6px;
        }
        ::-webkit-scrollbar-thumb {
            background: #6d28d9;
            border-radius: 10px;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col justify-between items-center p-3 md:p-6 relative">

    <!-- Background Decoration -->
    <div class="fixed inset-0 pointer-events-none z-0 overflow-hidden">
        <div class="absolute top-10 left-10 w-72 h-72 bg-purple-600/20 rounded-full blur-3xl"></div>
        <div class="absolute bottom-10 right-10 w-96 h-96 bg-pink-600/20 rounded-full blur-3xl"></div>
    </div>

    <!-- Header / Top Bar -->
    <header class="w-full max-w-2xl bg-slate-900/80 backdrop-blur border border-slate-800 rounded-2xl p-4 flex justify-between items-center shadow-xl z-10 mb-4">
        <div class="flex items-center gap-3">
            <div class="bg-gradient-to-tr from-amber-500 to-pink-500 p-2 rounded-xl text-slate-950 font-black text-xl shadow-lg">
                <i class="fa-solid font-black fa-explosion"></i>
            </div>
            <div>
                <h1 class="text-xl md:text-2xl font-black bg-gradient-to-r from-amber-400 via-pink-500 to-purple-400 bg-clip-text text-transparent">
                    قصف جبهات
                </h1>
                <p class="text-xs text-slate-400">التحدي العربي للردود القاتلة 🔥</p>
            </div>
        </div>

        <!-- High Score & Mute Toggle -->
        <div class="flex items-center gap-3">
            <div class="text-left bg-slate-800/80 px-3 py-1.5 rounded-xl border border-slate-700">
                <div class="text-[10px] text-slate-400">أعلى نتيجة</div>
                <div id="highScore" class="text-amber-400 font-bold text-sm">0</div>
            </div>
            <button id="soundToggleBtn" onclick="toggleSound()" class="w-10 h-10 bg-slate-800 hover:bg-slate-700 rounded-xl flex items-center justify-center border border-slate-700 transition active:scale-95 text-amber-400">
                <i id="soundIcon" class="fa-solid fa-volume-high"></i>
            </button>
        </div>
    </header>

    <!-- Main Game Container -->
    <main class="w-full max-w-2xl flex-1 flex flex-col justify-center items-center z-10">

        <!-- START SCREEN -->
        <div id="startScreen" class="w-full bg-slate-900/90 border border-slate-800 rounded-3xl p-6 md:p-8 text-center shadow-2xl backdrop-blur flex flex-col items-center">
            <div class="text-6xl mb-4 animate-bounce">💥😎</div>
            <h2 class="text-2xl md:text-3xl font-black text-white mb-3">هل أنت جاهز لـ "قصف الجبهات"؟</h2>
            <p class="text-slate-300 text-sm md:text-base leading-relaxed mb-6 max-w-md">
                واجه الخصوم المستفزين، اختار أقوى واشرس رد قبل ما يخلص الوقت! كل رد قاتل ينسف جبهة الخصم ويعطيك نقاط مضاعفة.
            </p>

            <div class="w-full max-w-xs space-y-3 mb-6 text-right text-xs text-slate-400 bg-slate-950/50 p-4 rounded-2xl border border-slate-800/80">
                <div class="flex items-center gap-2"><i class="fa-solid fa-fire text-amber-400"></i> الرد القاتل يعطيك نقاط عالية.</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-bolt text-yellow-400"></i> كل ما كنت أسرع، كل ما حصلت بونص سرعة!</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-heart-crack text-rose-400"></i> الرد الضعيف ينقص جبهتك أنت!</div>
            </div>

            <button onclick="startGame()" class="w-full max-w-xs py-4 bg-gradient-to-r from-amber-500 via-pink-600 to-purple-600 text-white font-black text-lg rounded-2xl shadow-lg hover:brightness-110 active:scale-95 transition flex items-center justify-center gap-3">
                <i class="fa-solid fa-play"></i> ابدأ التحدي الآن
            </button>
        </div>

        <!-- GAMEPLAY SCREEN -->
        <div id="gameScreen" class="w-full flex-col items-center gap-4 hidden">

            <!-- Stats Bar -->
            <div class="w-full bg-slate-900/80 border border-slate-800 rounded-2xl p-3 flex justify-between items-center shadow-lg">
                <!-- Level Info -->
                <div class="flex items-center gap-2">
                    <span class="text-xs text-slate-400">الخصم:</span>
                    <span id="opponentName" class="font-bold text-amber-400 text-sm md:text-base">الولد المتباهي</span>
                </div>

                <!-- Score -->
                <div class="flex items-center gap-2">
                    <i class="fa-solid fa-trophy text-amber-400 text-sm"></i>
                    <span id="currentScore" class="font-black text-lg text-white">0</span>
                </div>
            </div>

            <!-- Health Bars Section -->
            <div class="w-full grid grid-cols-2 gap-3">
                <!-- Player Health -->
                <div class="bg-slate-900/80 border border-slate-800 p-2.5 rounded-2xl">
                    <div class="flex justify-between items-center mb-1 text-xs font-bold">
                        <span class="text-emerald-400"><i class="fa-solid fa-user-shield"></i> جبهتك</span>
                        <span id="playerHpText" class="text-slate-300">100%</span>
                    </div>
                    <div class="w-full bg-slate-950 h-3 rounded-full overflow-hidden p-0.5 border border-slate-800">
                        <div id="playerHpBar" class="bg-gradient-to-r from-emerald-500 to-teal-400 h-full rounded-full transition-all duration-300" style="width: 100%;"></div>
                    </div>
                </div>

                <!-- Opponent Health -->
                <div class="bg-slate-900/80 border border-slate-800 p-2.5 rounded-2xl">
                    <div class="flex justify-between items-center mb-1 text-xs font-bold">
                        <span class="text-rose-400"><i class="fa-solid fa-skull"></i> جبهة الخصم</span>
                        <span id="opponentHpText" class="text-slate-300">100%</span>
                    </div>
                    <div class="w-full bg-slate-950 h-3 rounded-full overflow-hidden p-0.5 border border-slate-800">
                        <div id="opponentHpBar" class="bg-gradient-to-r from-rose-500 to-pink-500 h-full rounded-full transition-all duration-300" style="width: 100%;"></div>
                    </div>
                </div>
            </div>

            <!-- Opponent Stage / Avatar & Speech Box -->
            <div id="stageCard" class="w-full bg-slate-900/90 border border-slate-800 rounded-3xl p-5 flex flex-col items-center relative shadow-2xl backdrop-blur min-h-[260px] justify-between">
                
                <!-- Timer Bar Top -->
                <div class="w-full bg-slate-950/80 h-2 rounded-full overflow-hidden border border-slate-800 mb-3">
                    <div id="timerBar" class="bg-amber-400 h-full transition-all duration-100 ease-linear" style="width: 100%;"></div>
                </div>

                <!-- Character Graphic -->
                <div id="opponentAvatarContainer" class="relative my-2 transition-transform duration-300">
                    <div id="avatarEmoji" class="text-7xl md:text-8xl filter drop-shadow-[0_10px_15px_rgba(0,0,0,0.5)]">
                        😏
                    </div>
                    <!-- Impact FX Overlay -->
                    <div id="impactFx" class="absolute inset-0 flex items-center justify-center text-5xl opacity-0 pointer-events-none">
                        💥
                    </div>
                </div>

                <!-- Speech Bubble (Opponent Roast) -->
                <div class="w-full bg-gradient-to-b from-slate-800 to-slate-900 border border-amber-500/30 p-4 rounded-2xl relative shadow-lg text-center mt-2">
                    <!-- Bubble Arrow -->
                    <div class="absolute -top-3 left-1/2 -translate-x-1/2 w-0 h-0 border-l-[10px] border-l-transparent border-r-[10px] border-r-transparent border-b-[12px] border-b-slate-800"></div>
                    
                    <p id="opponentQuote" class="text-amber-200 font-bold text-base md:text-lg leading-snug">
                        "جاري تحضير الجبهة..."
                    </p>
                </div>
            </div>

            <!-- Responses Options (Player Choices) -->
            <div id="optionsContainer" class="w-full grid grid-cols-1 gap-2.5">
                <!-- Dynamic choices inserted here -->
            </div>
        </div>

        <!-- GAME OVER / VICTORY SCREEN -->
        <div id="resultScreen" class="w-full bg-slate-900/95 border border-slate-800 rounded-3xl p-6 text-center shadow-2xl backdrop-blur hidden flex-col items-center">
            <div id="resultIcon" class="text-7xl mb-3">👑</div>
            <h2 id="resultTitle" class="text-3xl font-black mb-2 text-amber-400">فوز ساحق!</h2>
            <p id="resultSubtitle" class="text-slate-300 text-sm mb-6">نسفت جبهات كل الخصوم وبقيت ملك الردود!</p>

            <!-- Final Stats Badge -->
            <div class="bg-slate-950 p-4 rounded-2xl border border-slate-800 w-full max-w-xs space-y-2 mb-6">
                <div class="flex justify-between items-center text-sm">
                    <span class="text-slate-400">النقاط النهائية:</span>
                    <span id="finalScore" class="font-black text-amber-400 text-lg">0</span>
                </div>
                <div class="flex justify-between items-center text-sm">
                    <span class="text-slate-400">عدد القصفات الناجحة:</span>
                    <span id="finalRoastsCount" class="font-bold text-emerald-400">0</span>
                </div>
            </div>

            <button onclick="startGame()" class="w-full max-w-xs py-3.5 bg-gradient-to-r from-amber-500 via-pink-600 to-purple-600 text-white font-black rounded-2xl shadow-lg hover:brightness-110 active:scale-95 transition flex items-center justify-center gap-2">
                <i class="fa-solid fa-rotate-right"></i> العب مرة ثانية
            </button>
        </div>

    </main>

    <!-- Footer -->
    <footer class="w-full text-center text-slate-500 text-xs py-2 z-10 mt-4">
        صنعت بكل شغف وتحدي 🔥 | قصف جبهات 2D
    </footer>

    <!-- GAME LOGIC SCRIPT -->
    <script>
        // Web Audio Synthesizer (No external sound files required)
        class SoundFX {
            constructor() {
                this.ctx = null;
                this.muted = false;
            }

            init() {
                if (!this.ctx) {
                    this.ctx = new (window.AudioContext || window.webkitAudioContext)();
                }
            }

            playTone(freq, type, duration, vol = 0.1) {
                if (this.muted) return;
                this.init();
                try {
                    const osc = this.ctx.createOscillator();
                    const gain = this.ctx.createGain();
                    osc.type = type;
                    osc.frequency.setValueAtTime(freq, this.ctx.currentTime);
                    gain.gain.setValueAtTime(vol, this.ctx.currentTime);
                    gain.gain.exponentialRampToValueAtTime(0.0001, this.ctx.currentTime + duration);
                    osc.connect(gain);
                    gain.connect(this.ctx.destination);
                    osc.start();
                    osc.stop(this.ctx.currentTime + duration);
                } catch(e) {}
            }

            playExplosion() {
                if (this.muted) return;
                this.init();
                try {
                    const bufferSize = this.ctx.sampleRate * 0.4;
                    const buffer = this.ctx.createBuffer(1, bufferSize, this.ctx.sampleRate);
                    const data = buffer.getChannelData(0);
                    for (let i = 0; i < bufferSize; i++) {
                        data[i] = Math.random() * 2 - 1;
                    }
                    const noise = this.ctx.createBufferSource();
                    noise.buffer = buffer;
                    const filter = this.ctx.createBiquadFilter();
                    filter.type = 'lowpass';
                    filter.frequency.setValueAtTime(800, this.ctx.currentTime);
                    filter.frequency.exponentialRampToValueAtTime(50, this.ctx.currentTime + 0.4);
                    
                    const gain = this.ctx.createGain();
                    gain.gain.setValueAtTime(0.3, this.ctx.currentTime);
                    gain.gain.exponentialRampToValueAtTime(0.01, this.ctx.currentTime + 0.4);

                    noise.connect(filter);
                    filter.connect(gain);
                    gain.connect(this.ctx.destination);
                    noise.start();
                } catch(e) {}
            }

            playFail() {
                this.playTone(180, 'sawtooth', 0.3, 0.2);
                setTimeout(() => this.playTone(120, 'sawtooth', 0.4, 0.2), 200);
            }

            playWin() {
                const notes = [261.63, 329.63, 392.00, 523.25];
                notes.forEach((freq, idx) => {
                    setTimeout(() => this.playTone(freq, 'triangle', 0.2, 0.15), idx * 100);
                });
            }
        }

        const sound = new SoundFX();
        function toggleSound() {
            sound.muted = !sound.muted;
            const icon = document.getElementById('soundIcon');
            if(sound.muted) {
                icon.className = 'fa-solid fa-volume-xmark text-slate-500';
            } else {
                icon.className = 'fa-solid fa-volume-high text-amber-400';
                sound.playTone(440, 'sine', 0.1);
            }
        }

        // Game Data & Opponents
        const opponents = [
            {
                name: "الولد المتباهي 😎",
                emoji: "😎",
                roasts: [
                    {
                        question: "شفت سيارتي الجديدة؟ أنت شوكت تشتري وحدة مثلها؟",
                        choices: [
                            { text: "أشتري لما أنت تشتري ذوق وياها! 🚗🔥", type: "devastating", damage: 45 },
                            { text: "الله يباركلك بيها حبيبي.", type: "weak", damage: 10 },
                            { text: "أصلاً أنا أحب أمشي على رجلي صحة!", type: "bad", damage: -15 }
                        ]
                    },
                    {
                        question: "ليش دايماً لما تحچي محد يسمعلك؟",
                        choices: [
                            { text: "لأن الكلام موجه للبشر مو لإلك! 🤐💥", type: "devastating", damage: 55 },
                            { text: "يمكن صوتي ناصي شوية...", type: "bad", damage: -15 },
                            { text: "كل واحد حنيته بقلبه.", type: "weak", damage: 10 }
                        ]
                    }
                ]
            },
            {
                name: "المتنمر الإلكتروني 🤖",
                emoji: "👹",
                roasts: [
                    {
                        question: "شنو هالمنشورات اللي تنشرها؟ تجيب المغص!",
                        choices: [
                            { text: "المهم جايبتك لصفحتي مسافة الطريق! 🚀🔥", type: "devastating", damage: 50 },
                            { text: "إذا ما تعجبك لا تباوع عليها.", type: "weak", damage: 10 },
                            { text: "آسف راح أمسحها لعيونك...", type: "bad", damage: -20 }
                        ]
                    },
                    {
                        question: "وين لعبتك اللي كنت تسولف بيها وتتفلسف؟",
                        choices: [
                            { text: "قاعد أقصيف بيك بيها حالياً! 🎯🔥", type: "devastating", damage: 50 },
                            { text: "بعدها تحت التطوير محتاجة وقت.", type: "weak", damage: 5 },
                            { text: "نسيت السيرفر مفتوح وراحت...", type: "bad", damage: -15 }
                        ]
                    }
                ]
            },
            {
                name: "صديقك المنفس 😒",
                emoji: "😒",
                roasts: [
                    {
                        question: "ليش كل ما تلعب بفرقتنا نخسر؟",
                        choices: [
                            { text: "لأن وجهك نحس يعكس الخسارة قبل لا نبدأ! 🪞💥", type: "devastating", damage: 60 },
                            { text: "السبب الحظ مو مني والله.", type: "weak", damage: 10 },
                            { text: "المرة الجاية راح أركز أكثر.", type: "bad", damage: -10 }
                        ]
                    },
                    {
                        question: "ترا القعدة وياك تضيق الخلق والروح!",
                        choices: [
                            { text: "الباب يتسع لجمل.. جرب تطلع وتشوف الراحة! 🚪🔥", type: "devastating", damage: 60 },
                            { text: "سامحني إذا ضايقتك بكلمة.", type: "bad", damage: -20 },
                            { text: "أنت اصلاً دايماً ضايق.", type: "weak", damage: 10 }
                        ]
                    }
                ]
            }
        ];

        // Game State Variables
        let currentOpponentIndex = 0;
        let currentRoastIndex = 0;
        let score = 0;
        let playerHp = 100;
        let opponentHp = 100;
        let timer = null;
        let timeLeft = 12; // تم زيادة الوقت إلى 12 ثانية
        let successfulRoastsCount = 0;
        let highScore = localStorage.getItem('qasf_high_score') || 0;

        document.getElementById('highScore').innerText = highScore;

        function startGame() {
            sound.init();
            currentOpponentIndex = 0;
            currentRoastIndex = 0;
            score = 0;
            playerHp = 100;
            opponentHp = 100;
            successfulRoastsCount = 0;

            document.getElementById('startScreen').classList.add('hidden');
            document.getElementById('resultScreen').classList.add('hidden');
            document.getElementById('resultScreen').classList.remove('flex');
            document.getElementById('gameScreen').classList.remove('hidden');
            document.getElementById('gameScreen').classList.add('flex');

            updateStatsUI();
            loadRound();
        }

        function updateStatsUI() {
            document.getElementById('currentScore').innerText = score;
            document.getElementById('playerHpText').innerText = `${Math.max(0, playerHp)}%`;
            document.getElementById('playerHpBar').style.width = `${Math.max(0, playerHp)}%`;
            document.getElementById('opponentHpText').innerText = `${Math.max(0, opponentHp)}%`;
            document.getElementById('opponentHpBar').style.width = `${Math.max(0, opponentHp)}%`;
        }

        function loadRound() {
            if (currentOpponentIndex >= opponents.length) {
                endGame(true);
                return;
            }

            const opponent = opponents[currentOpponentIndex];
            document.getElementById('opponentName').innerText = opponent.name;
            document.getElementById('avatarEmoji').innerText = opponent.emoji;

            // Reset Round States
            const currentRoast = opponent.roasts[currentRoastIndex];
            document.getElementById('opponentQuote').innerText = `"${currentRoast.question}"`;

            // Render Options
            const container = document.getElementById('optionsContainer');
            container.innerHTML = '';

            // Shuffle options slightly
            const shuffledChoices = [...currentRoast.choices].sort(() => Math.random() - 0.5);

            shuffledChoices.forEach((choice) => {
                const btn = document.createElement('button');
                btn.className = "w-full bg-slate-900/90 hover:bg-slate-800 border border-slate-700/80 hover:border-amber-500/50 p-3.5 rounded-2xl text-right font-bold text-sm md:text-base text-slate-100 transition duration-150 active:scale-[0.98] shadow-md flex items-center justify-between group";
                
                btn.innerHTML = `
                    <span>${choice.text}</span>
                    <i class="fa-solid fa-chevron-left text-slate-600 group-hover:text-amber-400 group-hover:-translate-x-1 transition-all"></i>
                `;
                
                btn.onclick = () => handleChoice(choice);
                container.appendChild(btn);
            });

            startTimer();
        }

        function startTimer() {
            clearInterval(timer);
            timeLeft = 12; // تم زيادة الوقت الابتدائي إلى 12 ثانية
            const timerBar = document.getElementById('timerBar');
            timerBar.style.width = '100%';

            timer = setInterval(() => {
                timeLeft -= 0.1;
                const percent = (timeLeft / 12) * 100; // حساب النسبة المئوية على أساس 12 ثانية
                timerBar.style.width = `${Math.max(0, percent)}%`;

                if (timeLeft <= 0) {
                    clearInterval(timer);
                    // Time Out Penalty
                    handleChoice({ type: 'timeout', damage: -20 });
                }
            }, 100);
        }

        function handleChoice(choice) {
            clearInterval(timer);

            const stageCard = document.getElementById('stageCard');
            const avatarContainer = document.getElementById('opponentAvatarContainer');
            const impactFx = document.getElementById('impactFx');

            if (choice.type === 'devastating') {
                // Critical Hit!
                sound.playExplosion();
                successfulRoastsCount++;
                
                // Bonus for fast response based on 12 seconds
                const speedBonus = Math.floor(timeLeft * 25);
                const roundPoints = 300 + speedBonus;
                score += roundPoints;

                opponentHp -= choice.damage;

                // Visual Effects
                stageCard.classList.add('shake');
                avatarContainer.classList.add('explode');
                impactFx.innerText = "💥🔥";
                impactFx.style.opacity = '1';

                setTimeout(() => {
                    stageCard.classList.remove('shake');
                    avatarContainer.classList.remove('explode');
                    impactFx.style.opacity = '0';
                }, 600);

            } else {
                // Fail / Weak Response
                sound.playFail();
                playerHp += choice.damage; // damage is negative or low

                stageCard.classList.add('shake');
                impactFx.innerText = choice.type === 'timeout' ? "⏰❌" : "🤡";
                impactFx.style.opacity = '1';

                setTimeout(() => {
                    stageCard.classList.remove('shake');
                    impactFx.style.opacity = '0';
                }, 500);
            }

            updateStatsUI();

            // Check Win / Lose / Next Round Conditions
            setTimeout(() => {
                if (playerHp <= 0) {
                    endGame(false);
                } else if (opponentHp <= 0) {
                    // Next Opponent
                    currentOpponentIndex++;
                    currentRoastIndex = 0;
                    opponentHp = 100;
                    updateStatsUI();
                    loadRound();
                } else {
                    // Next Roast of same opponent
                    currentRoastIndex++;
                    if (currentRoastIndex >= opponents[currentOpponentIndex].roasts.length) {
                        currentOpponentIndex++;
                        currentRoastIndex = 0;
                        opponentHp = 100;
                    }
                    updateStatsUI();
                    loadRound();
                }
            }, 800);
        }

        function endGame(isWin) {
            clearInterval(timer);
            document.getElementById('gameScreen').classList.add('hidden');
            document.getElementById('resultScreen').classList.remove('hidden');
            document.getElementById('resultScreen').classList.add('flex');

            const title = document.getElementById('resultTitle');
            const icon = document.getElementById('resultIcon');
            const subtitle = document.getElementById('resultSubtitle');

            if (isWin) {
                sound.playWin();
                icon.innerText = "👑";
                title.innerText = "فوز ساحق ومستحق!";
                title.className = "text-3xl font-black mb-2 text-amber-400";
                subtitle.innerText = "أثبتت إنك ملك قصف الجبهات بلا منازع!";
            } else {
                sound.playFail();
                icon.innerText = "💀";
                title.innerText = "انقصفت جبهتك!";
                title.className = "text-3xl font-black mb-2 text-rose-500";
                subtitle.innerText = "يحتاج تتدرب أكثر على الردود السريعة وترجع تتحدى!";
            }

            document.getElementById('finalScore').innerText = score;
            document.getElementById('finalRoastsCount').innerText = successfulRoastsCount;

            // Save Highscore
            if (score > highScore) {
                highScore = score;
                localStorage.setItem('qasf_high_score', highScore);
                document.getElementById('highScore').innerText = highScore;
            }
        }
    </script>
</body>
</html>
```
