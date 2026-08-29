# 🌌 exam60: The Next-Gen Class 10th GK Ecosystem

Welcome to **exam60**, an ultra-premium, high-fidelity knowledge application engineered for Class 10th students. This is not just a quiz app—it is a futuristic cognitive learning platform built to dominate Board Exams, NTSE, and Olympiads.

---

## 💎 Elite Features & Architecture (ऐप की मुख्य लग्जरी विशेषताएं)

If we were to build the ultimate Class 10th GK Application, these are the **10 revolutionary core features** integrated into its DNA:

### 🧠 1. Neuro-Adaptive AI Learning Engine
Our proprietary AI analyzes the student’s response time and cognitive patterns in real-time. It automatically scales the difficulty of GK questions from school-board level to national-competition level based on individual performance.

### 🎮 2. Gamified 1v1 Live GK Battles
Students can challenge peers across the nation in real-time, high-speed 1v1 general knowledge duels. Features a dynamic matchmaking system, live leaderboard streaks, and digital trophies to maximize engagement.

### 🎨 3. Immersive 4K Infographic Dashboards
Bypass boring text. Historical timelines, world geography maps, and complex scientific innovations are rendered through stunning, high-definition interactive visuals and custom micro-charts.

### ⚡ 4. Curated Daily Booster Shots
Every morning, the app delivers exactly 5 highly critical, high-yield general knowledge facts directly to the notification shade. Powered by predictive algorithms to feature questions most likely to appear in exams.

### 📊 5. Real-Time Global Percentile & Analytics
Provides an elite, deep-dive performance dashboard. Instead of basic scores, students see their exact nationwide rank, strength/weakness heatmaps, and precise time spent per question.

### 🎯 6. Board Topper’s Keyword Highlighter
When reviewing answers, our smart engine uses specialized natural language processing (NLP) to instantly highlight high-scoring keywords used by previous board toppers, training students how to write flawless answers.

### 🎙️ 7. AI Voice-Powered Doubt Solver
An integrated, voice-activated AI tutor. If a student encounters a tricky historical date or scientific fact, they can simply ask out loud and receive instant, verified audio explanations.

### 🌙 8. Cinematic Dark Mode & Aesthetic UI
Built with an ultra-premium, low-contrast dark palette designed to reduce ocular fatigue during late-night study sessions. Every transition, animation, and button press feels completely fluid and cinematic.

### 🔄 9. Hyper-Sync Offline Caching
Features advanced local database synchronization. Once the app syncs, all core GK modules and saved notes are fully accessible without internet connectivity, ensuring uninterrupted learning anywhere.
## 🛠️ Tech Stack & Architecture (टेक्नोलॉजी)
* **Frontend:** HTML5, CSS3, Tailwind CSS (For Ultra-Smooth Aesthetic UI)
* **Backend:** Node.js / Express (For Fast API Responses)
* **Database:** MongoDB / Firebase (For Real-Time Global Percentile & Sync)
* **AI Integration:** OpenAI API / Custom NLP Model (For AI Doubt Solver)
### 🏆 10. Olympiad & NTSE Elite Edge Mode
A dedicated, high-tier section inside the app that completely bypasses rote memorization. It focuses entirely on logical reasoning, analytical skills, and advanced general awareness required for prestige scholarships.

---

## 🛠️ Project Ecosystem
* **Project Name:** exam60
* **Target Audience:** Class 10th Board, NTSE, & National Olympiad Aspirants
* **UI Philosophy:** Minimalism, High-Fidelity Graphics, Ultra-Smooth Transitions
<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>exam60: बिहार बोर्ड (BSEB) कक्षा 10वीं लाइव क्विज़</title>
    <!-- Tailwind CSS स्टाइलिंग के लिए -->
    <script src="https://tailwindcss.com"></script>
</head>
<body class="bg-slate-50 min-h-screen flex items-center justify-center p-4 font-sans">

    <!-- क्विज़ बॉक्स कंटेनर -->
    <div class="bg-white w-full max-w-xl rounded-2xl shadow-xl border border-slate-100 p-6 md:p-8">
        
        <!-- हेडर: प्रश्न संख्या और टाइमर -->
        <div class="flex justify-between items-center mb-6">
            <span id="question-number" class="text-sm font-semibold text-red-600 bg-red-50 px-3 py-1 rounded-full">प्रश्न 1</span>
            <div class="text-sm font-medium text-slate-500 flex items-center gap-1">
                ⏱️ समय: <span id="timer" class="text-slate-700 font-bold">20</span> सेकेंड
            </div>
        </div>

        <!-- प्रश्न का टेक्स्ट -->
        <h2 id="question-text" class="text-lg md:text-xl font-bold text-slate-800 mb-6 leading-snug">
            प्रश्न लोड हो रहा है...
        </h2>

        <!-- विकल्पों की सूची -->
        <div id="options-container" class="space-y-3 mb-6">
            <!-- यहाँ जावास्क्रिप्ट द्वारा विकल्प जोड़े जाएंगे -->
        </div>

        <!-- फुटर: स्कोर ट्रैकर और अगला बटन -->
        <div class="flex justify-between items-center border-t border-slate-100 pt-4">
            <div class="text-sm text-slate-600">
                सही उत्तर: <span id="current-score" class="font-bold text-green-600">0</span>
            </div>
            <button id="next-btn" onclick="nextQuestion()" class="hidden bg-red-600 hover:bg-red-700 text-white font-semibold px-5 py-2 rounded-lg transition text-sm shadow-md">
                अगला प्रश्न →
            </button>
        </div>
    </div>

    <!-- क्विज़ का लॉजिक और बिहार बोर्ड के प्रश्न -->
    <script>
        const quizData = [
            {
                question: "1. 'नेपोलियन संहिता' (Napoleonic Code) किस वर्ष लागू की गई थी?",
                options: ["1789 में", "1791 में", "1801 में", "1804 में"],
                correct: 3
            },
            {
                question: "2. कार्ल मार्क्स का जन्म कहाँ हुआ था?",
                options: ["इंग्लैंड", "जर्मनी", "इटली", "रूस"],
                correct: 1
            },
            {
                question: "3. बिहार में रज्जू मार्ग (Ropeway) कहाँ स्थित है?",
                options: ["बिहारशरीफ", "राजगीर", "गया", "बांका"],
                correct: 1
            },
            {
                question: "4. भारत के किस राज्य में सौर ऊर्जा के विकास की सर्वाधिक संभावनाएं हैं?",
                options: ["असम", "अरुणाचल प्रदेश", "राजस्थान", "मेघालय"],
                correct: 2
            },
            {
                question: "5. निम्नलिखित में से किसे 'पिछड़ा राज्य' (BIMARU State) कहा जाता है?",
                options: ["पंजाब", "केरल", "बिहार", "दिल्ली"],
                correct: 2
            }
        ];

        let currentIdx = 0;
        let score = 0;
        let timerCount = 20; // बिहार बोर्ड के लिए 20 सेकेंड का समय
        let timerInterval;

        function loadQuestion() {
            clearInterval(timerInterval);
            timerCount = 20;
            document.getElementById("timer").innerText = timerCount;
            
            const q = quizData[currentIdx];
            document.getElementById("question-number").innerText = `प्रश्न ${currentIdx + 1} / ${quizData.length}`;
            document.getElementById("question-text").innerText = q.question;
            document.getElementById("next-btn").classList.add("hidden");

            const optContainer = document.getElementById("options-container");
            optContainer.innerHTML = "";

            q.options.forEach((option, index) => {
                const btn = document.createElement("button");
                btn.className = "w-full text-left p-4 rounded-xl border-2 border-slate-100 hover:border-red-500 hover:bg-red-50/30 font-medium text-slate-700 transition duration-200 block text-sm md:text-base";
                btn.innerText = option;
                btn.onclick = () => checkAnswer(index, btn);
                optContainer.appendChild(btn);
            });

            startTimer();
        }

        function startTimer() {
            timerInterval = setInterval(() => {
                timerCount--;
                document.getElementById("timer").innerText = timerCount;
                if(timerCount <= 0) {
                    clearInterval(timerInterval);
                    disableOptions();
                    showCorrectAnswerAutomatically();
                    document.getElementById("next-btn").classList.remove("hidden");
                }
            }, 1000);
        }

        function checkAnswer(selectedIdx, clickedBtn) {
            clearInterval(timerInterval);
            const correctIdx = quizData[currentIdx].correct;
            const allButtons = document.getElementById("options-container").children;

            if(selectedIdx === correctIdx) {
                clickedBtn.className = "w-full text-left p-4 rounded-xl border-2 border-green-500 bg-green-50 font-semibold text-green-700 block text-sm md:text-base";
                score++;
                document.getElementById("current-score").innerText = score;
            } else {
                clickedBtn.className = "w-full text-left p-4 rounded-xl border-2 border-red-500 bg-red-50 font-semibold text-red-700 block text-sm md:text-base";
                allButtons[correctIdx].className = "w-full text-left p-4 rounded-xl border-2 border-green-500 bg-green-50 font-semibold text-green-700 block text-sm md:text-base";
            }

            disableOptions();
            document.getElementById("next-btn").classList.remove("hidden");
        }

        function showCorrectAnswerAutomatically() {
            const correctIdx = quizData[currentIdx].correct;
            const allButtons = document.getElementById("options-container").children;
            allButtons[correctIdx].className = "w-full text-left p-4 rounded-xl border-2 border-green-500 bg-green-50 font-semibold text-green-700 block text-sm md:text-base";
        }

        function disableOptions() {
            const allButtons = document.getElementById("options-container").children;
            for(let btn of allButtons) {
                btn.disabled = true;
            }
        }

        function nextQuestion() {
            currentIdx++;
            if(currentIdx < quizData.length) {
                loadQuestion();
            } else {
                showResults();
            }
        }

        function showResults() {
            const container = document.getElementById("options-container").parentElement;
            container.innerHTML = `
                <div class="text-center py-4">
                    <span class="text-5xl">🏆</span>
                    <h2 class="text-2xl font-bold text-slate-800 mt-4 mb-2">क्विज़ समाप्त!</h2>
                    <p class="text-slate-600 text-lg mb-6">आपका कुल स्कोर: <span class="font-bold text-red-600 text-xl">${score} / ${quizData.length}</span></p>
                    <button onclick="window.location.reload()" class="w-full bg-red-600 hover:bg-red-700 text-white font-semibold py-3 rounded-xl transition shadow-md">फिर से टेस्ट दें</button>
                </div>
            `;
        }

        // पहली बार प्रश्न लोड करने के लिए
        loadQuestion();
    </script>
</body>
</html>
