<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Class 11 ISC Hindi Unit Test 2 Practice Hub</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Rozha+One&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Poppins', sans-serif; }
        .hindi-title { font-family: 'Rozha One', serif; }
    </style>
</head>
<body class="bg-gradient-to-br from-indigo-50 via-purple-50 to-pink-50 min-p-4 min-h-screen">

    <div class="max-w-4xl mx-auto py-8 px-4">
        <!-- Header -->
        <header class="text-center mb-8 bg-white p-6 rounded-2xl shadow-lg border border-indigo-100">
            <h1 class="hindi-title text-3xl md:text-4xl text-indigo-900 mb-2">कक्षा 11 - ISC हिंदी यूनिट टेस्ट 2</h1>
            <p class="text-gray-600 font-medium">पाठ्यक्रम: 'सती' (कहानी), 'आह! धरती कितना देती है' (कविता), मुहावरे एवं अशुद्ध वाक्य संशोधन</p>
            <div class="flex justify-center gap-4 mt-4">
                <button onclick="switchTab('mcq')" id="btn-mcq" class="px-6 py-2 rounded-full font-semibold transition-all shadow-md bg-indigo-600 text-white">20 मार्क्स MCQs (इंटरैक्टिव)</button>
                <button onclick="switchTab('practice')" id="btn-practice" class="px-6 py-2 rounded-full font-semibold transition-all shadow-md bg-gray-200 text-gray-700 hover:bg-indigo-100">20 मार्क्स अभ्यास प्रश्न</button>
            </div>
        </header>

        <!-- MCQ Section -->
        <div id="section-mcq" class="bg-white rounded-2xl shadow-xl p-6 md:p-8 border border-indigo-50">
            <div class="flex justify-between items-center mb-6 pb-4 border-b border-gray-100">
                <h2 class="text-xl font-bold text-gray-800 flex items-center gap-2">
                    <span class="bg-indigo-100 text-indigo-700 px-3 py-1 rounded-lg text-sm">बहुविकल्पीय प्रश्न (20 अंक)</span>
                </h2>
                <span id="question-tracker" class="text-sm font-semibold text-indigo-600">प्रश्न 1 / 20</span>
            </div>

            <div id="quiz-container">
                <!-- Question Box -->
                <div id="question-text" class="text-lg font-semibold text-gray-900 mb-6"></div>

                <!-- Options -->
                <div id="options-container" class="space-y-3 mb-6"></div>

                <!-- Explanation Box -->
                <div id="explanation-box" class="hidden p-4 rounded-xl mb-6 text-sm font-medium"></div>

                <!-- Navigation -->
                <div class="flex justify-between items-center pt-4 border-t border-gray-100">
                    <button id="prev-btn" onclick="prevQuestion()" class="px-5 py-2.5 rounded-xl border border-gray-300 text-gray-700 font-medium hover:bg-gray-50 transition disabled:opacity-50" disabled>पिछला</button>
                    <button id="next-btn" onclick="nextQuestion()" class="px-6 py-2.5 rounded-xl bg-indigo-600 text-white font-medium hover:bg-indigo-700 transition shadow-md shadow-indigo-200">अगला प्रश्न</button>
                </div>
            </div>

            <!-- Result View -->
            <div id="result-container" class="hidden text-center py-8">
                <div class="text-6xl mb-4">🎉</div>
                <h3 class="text-2xl font-bold text-gray-900 mb-2">क्विज़ संपन्न हुआ!</h3>
                <p id="score-display" class="text-lg text-gray-600 mb-6"></p>
                <button onclick="restartQuiz()" class="px-8 py-3 bg-indigo-600 text-white font-semibold rounded-xl shadow-lg hover:bg-indigo-700 transition">दोबारा प्रयास करें</button>
            </div>
        </div>

        <!-- Practice Subjective Section -->
        <div id="section-practice" class="hidden bg-white rounded-2xl shadow-xl p-6 md:p-8 border border-indigo-50">
            <h2 class="text-xl font-bold text-gray-800 mb-2">लिखित एवं अभ्यास प्रश्न (20 अंक)</h2>
            <p class="text-gray-500 text-sm mb-6">अपने उत्तर लिखने के बाद 'उत्तर देखें' बटन पर क्लिक करके अपने उत्तर की जाँच करें।</p>

            <div class="space-y-6">
                <!-- Question 1 -->
                <div class="p-5 rounded-2xl bg-gray-50 border border-gray-200">
                    <span class="text-xs font-bold text-indigo-600 uppercase tracking-wider">सती कहानी (5 अंक)</span>
                    <h3 class="font-semibold text-gray-900 mt-1 mb-3">प्रश्न 1: 'सती' कहानी के आधार पर मणिकर्णिका (मणि) के चरित्र की प्रमुख विशेषताओं पर प्रकाश डालिए।</h3>
                    <button onclick="toggleAnswer('ans-1')" class="text-sm font-medium text-indigo-600 hover:text-indigo-800 underline">उत्तर देखें / छिपाएँ</button>
                    <div id="ans-1" class="hidden mt-3 p-4 bg-white rounded-xl text-sm text-gray-700 border border-indigo-100 shadow-inner">
                        <strong>मॉडल उत्तर:</strong> शिवानी द्वारा रचित 'सती' कहानी की मुख्य पात्र मणिकर्णिका (मणि) आत्मानुशासित, संवेदनशील, विद्रोही और स्वाभिमानी स्वभाव की है। वह रूढ़िवादी सामाजिक मान्यताओं के विरुद्ध अपने आत्मसम्मान को सर्वोपरि रखती है। उसके चरित्र में गहन करुणा के साथ-साथ परिस्थितियों से जूझने का साहस भी झलकता है।
                    </div>
                </div>

                <!-- Question 2 -->
                <div class="p-5 rounded-2xl bg-gray-50 border border-gray-200">
                    <span class="text-xs font-bold text-indigo-600 uppercase tracking-wider">आह! धरती कितना देती है (5 अंक)</span>
                    <h3 class="font-semibold text-gray-900 mt-1 mb-3">प्रश्न 2: सुमित्रानंदन पंत जी ने 'आह! धरती कितना देती है' कविता के माध्यम से मनुष्य के लालच और प्रकृति की उदारता के बीच क्या संदेश दिया है?</h3>
                    <button onclick="toggleAnswer('ans-2')" class="text-sm font-medium text-indigo-600 hover:text-indigo-800 underline">उत्तर देखें / छिपाएँ</button>
                    <div id="ans-2" class="hidden mt-3 p-4 bg-white rounded-xl text-sm text-gray-700 border border-indigo-100 shadow-inner">
                        <strong>मॉडल उत्तर:</strong> कवि ने बताया है कि मनुष्य अपनी कंजूसी और स्वार्थवश धरती को सोना या धन देकर भी बदले में केवल नगण्य चीजें ही पाना चाहता है, जबकि प्रकृति (धरती) बेहद उदार है। वह मनुष्य द्वारा दिए गए छोटे से बीज या त्याग को कई गुना लौटा देती है। कविता मनुष्य की संकीर्ण मानसिकता और प्रकृति की अनंत उदारता का सुंदर contrast प्रस्तुत करती है।
                    </div>
                </div>

                <!-- Question 3 -->
                <div class="p-5 rounded-2xl bg-gray-50 border border-gray-200">
                    <span class="text-xs font-bold text-indigo-600 uppercase tracking-wider">मुहावरे (5 अंक)</span>
                    <h3 class="font-semibold text-gray-900 mt-1 mb-3">प्रश्न 3: निम्नलिखित पाँच मुहावरों का अर्थ लिखकर वाक्यों में प्रयोग कीजिए:</h3>
                    <ol class="list-decimal list-inside text-sm text-gray-800 space-y-1 mb-3">
                        <li>आँखें खुलना</li>
                        <li>अँगूठा दिखाना</li>
                        <li>कान भरना</li>
                        <li>नौ दो ग्यारह होना</li>
                        <li>श्रीगणेश करना</li>
                    </ol>
                    <button onclick="toggleAnswer('ans-3')" class="text-sm font-medium text-indigo-600 hover:text-indigo-800 underline">उत्तर देखें / छिपाएँ</button>
                    <div id="ans-3" class="hidden mt-3 p-4 bg-white rounded-xl text-sm text-gray-700 border border-indigo-100 shadow-inner space-y-2">
                        <p><strong>1. आँखें खुलना (वास्तविकता का ज्ञान होना):</strong> ठगी का शिकार होने के बाद सोहन की आँखें खुल गईं।</p>
                        <p><strong>2. अँगूठा दिखाना (ऐन वक्त पर मना करना):</strong> जरूरत के समय मित्र द्वारा मदद से अँगूठा दिखाने पर सोहन निराश हो गया।</p>
                        <p><strong>3. कान भरना (चुगली करना):</strong> सहकर्मी के खिलाफ बॉस के कान भरना उसकी आदत बन चुकी थी।</p>
                        <p><strong>4. नौ दो ग्यारह होना (भाग जाना):</strong> पुलिस को आते देख चोर पलक झपकते ही नौ दो ग्यारह हो गए।</p>
                        <p><strong>5. श्रीगणेश करना (शुभारंभ करना):</strong> नए कार्यालय का निर्माण कार्य हवन के साथ श्रीगणेश किया गया।</p>
                    </div>
                </div>

                <!-- Question 4 -->
                <div class="p-5 rounded-2xl bg-gray-50 border border-gray-200">
                    <span class="text-xs font-bold text-indigo-600 uppercase tracking-wider">अशुद्ध वाक्य संशोधन (5 अंक)</span>
                    <h3 class="font-semibold text-gray-900 mt-1 mb-3">प्रश्न 4: निम्नलिखित पाँच अशुद्ध वाक्यों को शुद्ध करके लिखिए:</h3>
                    <ol class="list-decimal list-inside text-sm text-gray-800 space-y-1 mb-3">
                        <li>वृक्ष पर से पत्ता गिरा।</li>
                        <li>राम और सीता वन को गई।</li>
                        <li>मुझे एक फूलों की माला चाहिए।</li>
                        <li>वहाँ भारी भीड़ जमा थी।</li>
                        <li>वह आँखों से अंधा है।</li>
                    </ol>
                    <button onclick="toggleAnswer('ans-4')" class="text-sm font-medium text-indigo-600 hover:text-indigo-800 underline">उत्तर देखें / छिपाएँ</button>
                    <div id="ans-4" class="hidden mt-3 p-4 bg-white rounded-xl text-sm text-gray-700 border border-indigo-100 shadow-inner space-y-2">
                        <p><strong>1.</strong> वृक्ष से पत्ता गिरा। (या पेड़ से पत्ता गिरा)</p>
                        <p><strong>2.</strong> राम और सीता वन को गए।</p>
                        <p><strong>3.</strong> मुझे फूलों की एक माला चाहिए।</p>
                        <p><strong>4.</strong> वहाँ भारी भीड़ जमा थी / जमावड़ा था। (या 'वहाँ बहुत भीड़ थी')</p>
                        <p><strong>5.</strong> वह अंधा है। (या 'वह जन्म से अंधा है' - 'आँखों से' पुनरुक्ति दोष है)</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        const questions = [
            // सती कहानी (1-5)
            {
                question: "'सती' कहानी की लेखिका कौन हैं?",
                options: ["महादेवी वर्मा", "शिवानी", "मन्नू भंडारी", "कृष्णा सोबती"],
                correct: 1,
                explanation: "'सती' प्रसिद्ध लेखिका शिवानी द्वारा रचित एक अत्यंत मर्मस्पर्शी कहानी है।"
            },
            {
                question: "'सती' कहानी में मुख्य पात्र मणिकर्णिका (मणि) के जीवन का केंद्रीय संघर्ष किससे जुड़ा है?",
                options: ["पारिवारिक संपत्ति", "आत्मसम्मान और सामाजिक रूढ़ियाँ", "विदेश यात्रा", "राजनीतिक पद"],
                correct: 1,
                explanation: "मणि का संघर्ष रूढ़िवादी समाज के बीच अपने स्वाभिमान और आत्मसम्मान की रक्षा से जुड़ा है।"
            },
            {
                question: "शिवानी की लेखन शैली की मुख्य विशेषता क्या मानी जाती है?",
                options: ["शुष्क दार्शनिकता", "क्षेत्रीय आंचलकता और नाटकीय संवेदनशीलता", "केवल हास्य-व्यंग्य", "पत्रकारिता शैली"],
                correct: 1,
                explanation: "शिवानी की कहानियों में आंचलिकाता, नाटकीयता और भावनाओं का तीव्र प्रवाह देखने को मिलता है।"
            },
            {
                question: "'सती' कहानी समाज के किस वर्ग की विडंबनाओं को उजागर करती है?",
                options: ["उच्च वर्ग की खोखली नैतिकता", "श्रमिक वर्ग की समस्याएँ", "छात्र जीवन", "औद्योगिक संघर्ष"],
                correct: 0,
                explanation: "यह कहानी उच्च वर्गीय पाखंड और रूढ़ियों पर करारा प्रहार करती है।"
            },
            {
                question: "मणि के चरित्र में निम्नलिखित में से कौन सा गुण सबसे प्रमुख है?",
                options: ["कायरता", "आत्मबल और दृढ़ता", "उदासीनता", "लोभ"],
                correct: 1,
                explanation: "मणि अत्यंत दृढ़निश्चयी और आत्मबल से परिपूर्ण पात्र है।"
            },

            // आह! धरती कितना देती है (6-10)
            {
                question: "'आह! धरती कितना देती है' कविता के रचयिता कौन हैं?",
                options: ["सुमित्रानंदन पंत", "सूर्यकांत त्रिपाठी 'निराला'", "जयशंकर प्रसाद", "महादेवी वर्मा"],
                correct: 0,
                explanation: "यह कविता प्रकृति के सुकुमार कवि सुमित्रानंदन पंत जी की है।"
            },
            {
                question: "कवि ने धरती की किस विशेषता को रेखांकित किया है?",
                options: ["उसकी अनुदारता", "उसकी अनंत उदारता और सहनशीलता", "उसका रूखापन", "उसकी निर्जीवता"],
                correct: 1,
                explanation: "कवि ने धरती की उदारता का वर्णन किया है जो छोटे से बीज को भी वृक्ष और अनाज में बदल देती है।"
            },
            {
                question: "कविता में मनुष्य के किस दुर्गुण पर व्यंग्य किया गया है?",
                options: ["परोपकार", "लोभ और संकीर्ण स्वार्थ", "साहस", "दयालुता"],
                correct: 1,
                explanation: "कवि ने मनुष्य के लोभी स्वभाव पर व्यंग्य किया है जो धरती को कम देकर अधिक पाना चाहता है।"
            },
            {
                question: "कवि ने धरती को क्या साबित करने का प्रयास किया है?",
                options: ["वह सबसे अमीर रत्नगर्भा है", "वह मनुष्य के त्याग का कई गुना प्रतिफल देती है", "वह बंजर हो चुकी है", "वह मानव विरोधी है"],
                correct: 1,
                explanation: "धरती मनुष्य द्वारा बोए गए एक दाने को हजारों गुना फसल में बदल कर लौटा देती है।"
            },
            {
                question: "सुमित्रानंदन पंत किस धारा के प्रमुख कवि माने जाते हैं?",
                options: ["छायावाद", "प्रगतिवाद", "प्रयोगवाद", "रीतिकालीन"],
                correct: 0,
                explanation: "सुमित्रानंदन पंत छायावाद के प्रमुख स्तंभों में से एक हैं।"
            },

            // मुहावरे (11-15)
            {
                question: "'अंगूठा दिखाना' मुहावरे का सही अर्थ क्या है?",
                options: ["मदद करना", "ऐन वक्त पर मना करना", "चिढ़ाना", "तारीफ करना"],
                correct: 1,
                explanation: "अँगूठा दिखाने का अर्थ आवश्यकता पड़ने पर साफ मना कर देना होता है।"
            },
            {
                question: "'नौ दो ग्यारह होना' का सही अर्थ है:",
                options: ["गिनती करना", "भाग जाना", "झगड़ा करना", "सहयोग करना"],
                correct: 1,
                explanation: "नौ दो ग्यारह होने का अर्थ डरकर या चुपके से भाग जाना है।"
            },
            {
                question: "'कान भरना' मुहावरे का अर्थ क्या है?",
                options: ["सुई से कान साफ करना", "चुगली करना या भड़काना", "संगीत सुनना", "कान की बीमारी होना"],
                correct: 1,
                explanation: "किसी के विरुद्ध किसी के कान भरना यानी चुगली करना या भड़काना।"
            },
            {
                question: "'श्रीगणेश करना' का अर्थ है:",
                options: ["पूजा करना", "किसी कार्य का शुभारंभ करना", "समापन करना", "गणेश जी को याद करना"],
                correct: 1,
                explanation: "श्रीगणेश करने का अर्थ किसी भी नए कार्य की शुरुआत करना है।"
            },
            {
                question: "'आँखें चार होना' का उपयुक्त अर्थ है:",
                options: ["आमने-सामने होना या प्रेम होना", "चार आँखें होना", "चश्मा लगाना", "नाराज होना"],
                correct: 0,
                explanation: "आँखें चार होने का अर्थ आमने-सामने होना या प्रेम संबंध स्थापित होना है।"
            },

            // अशुद्ध वाक्य संशोधन (16-20)
            {
                question: "अशुद्ध वाक्य: 'वृक्ष पर से पत्ता गिरा।' इसका शुद्ध रूप क्या होगा?",
                options: ["वृक्ष पर पत्ता गिरा।", "वृक्ष से पत्ता गिरा।", "पत्ता वृक्ष गिरा।", "वृक्ष के ऊपर पत्ता गिरा।"],
                correct: 1,
                explanation: "अलग होने के अर्थ में 'से' कारक चिन्ह का प्रयोग होता है, 'पर से' अनुचित है।"
            },
            {
                question: "अशुद्ध वाक्य: 'राम और सीता वन को गई।' इसका शुद्ध रूप क्या होगा?",
                options: ["राम और सीता वन को गए।", "राम और सीता वन को गई थीं।", "राम और सीता वन गए।", "क और ग दोनों सही हैं"],
                correct: 3,
                explanation: "पुल्लिंग और स्त्रीलिंग दोनों होने पर क्रिया पुल्लिंग बहुवचन 'गए' होती है।"
            },
            {
                question: "अशुद्ध वाक्य: 'मुझे एक फूलों की माला चाहिए।' इसका शुद्ध रूप क्या होगा?",
                options: ["मुझे फूलों की एक माला चाहिए।", "मुझे एक फूल की माला चाहिए।", "मुझे माला फूलों की चाहिए।", "मुझे फूलों माला चाहिए।"],
                correct: 0,
                explanation: "'एक' शब्द माला के साथ आएगा न कि फूलों के साथ, क्योंकि माला एक है फूल अनेक।"
            },
            {
                question: "अशुद्ध वाक्य: 'वहाँ भारी भीड़ जमा थी।' इसका शुद्ध रूप क्या है?",
                options: ["वहाँ भारी भीड़ थी।", "वहाँ बहुत भीड़ थी।", "वहाँ भीड़ जमा थी।", "उपरोक्त सभी शुद्ध हैं"],
                correct: 1,
                explanation: "'भीड़' के साथ 'भारी' की जगह 'बहुत' का प्रयोग अधिक सटीक और व्याकरण सम्मत है।"
            },
            {
                question: "अशुद्ध वाक्य: 'वह आँखों से अंधा है।' इसका शुद्ध रूप क्या होगा?",
                options: ["वह अंधा है।", "वह आँख से अंधा है।", "वह नेत्रहीन है।", "क और ग दोनों"],
                correct: 3,
                explanation: "'आँखों से अंधा' में पुनरुक्ति दोष है, केवल 'वह अंधा है' या 'वह नेत्रहीन है' अधिक शुद्ध है।"
            }
        ];

        let currentQuestion = 0;
        let score = 0;
        let selectedOptions = new Array(questions.length).fill(null);

        function switchTab(tab) {
            const mcqSec = document.getElementById('section-mcq');
            const pracSec = document.getElementById('section-practice');
            const btnMcq = document.getElementById('btn-mcq');
            const btnPrac = document.getElementById('btn-practice');

            if(tab === 'mcq') {
                mcqSec.classList.remove('hidden');
                pracSec.classList.add('hidden');
                btnMcq.className = "px-6 py-2 rounded-full font-semibold transition-all shadow-md bg-indigo-600 text-white";
                btnPrac.className = "px-6 py-2 rounded-full font-semibold transition-all shadow-md bg-gray-200 text-gray-700 hover:bg-indigo-100";
            } else {
                mcqSec.classList.add('hidden');
                pracSec.classList.remove('hidden');
                btnPrac.className = "px-6 py-2 rounded-full font-semibold transition-all shadow-md bg-indigo-600 text-white";
                btnMcq.className = "px-6 py-2 rounded-full font-semibold transition-all shadow-md bg-gray-200 text-gray-700 hover:bg-indigo-100";
            }
        }

        function loadQuestion() {
            const q = questions[currentQuestion];
            document.getElementById('question-tracker').innerText = `प्रश्न ${currentQuestion + 1} / ${questions.length}`;
            document.getElementById('question-text').innerText = q.question;

            const optsContainer = document.getElementById('options-container');
            optsContainer.innerHTML = '';

            q.options.forEach((opt, idx) => {
                const btn = document.createElement('button');
                btn.className = `w-full text-left p-4 rounded-xl border-2 transition-all font-medium flex items-center justify-between ${
                    selectedOptions[currentQuestion] === idx 
                        ? (idx === q.correct ? 'border-green-500 bg-green-50 text-green-900' : 'border-red-500 bg-red-50 text-red-900')
                        : 'border-gray-200 hover:border-indigo-300 hover:bg-indigo-50/30 text-gray-800'
                }`;
                
                btn.innerHTML = `<span>${opt}</span>`;
                btn.onclick = () => selectOption(idx);
                optsContainer.appendChild(btn);
            });

            const expBox = document.getElementById('explanation-box');
            if(selectedOptions[currentQuestion] !== null) {
                showExplanation();
            } else {
                expBox.classList.add('hidden');
            }

            document.getElementById('prev-btn').disabled = currentQuestion === 0;
            document.getElementById('next-btn').innerText = currentQuestion === questions.length - 1 ? 'परिणाम देखें' : 'अगला प्रश्न';
        }

        function selectOption(idx) {
            if(selectedOptions[currentQuestion] !== null) return; // already answered

            selectedOptions[currentQuestion] = idx;
            if(idx === questions[currentQuestion].correct) {
                score++;
            }
            loadQuestion();
        }

        function showExplanation() {
            const q = questions[currentQuestion];
            const expBox = document.getElementById('explanation-box');
            const isCorrect = selectedOptions[currentQuestion] === q.correct;
            
            expBox.className = `p-4 rounded-xl mb-6 text-sm font-medium ${isCorrect ? 'bg-green-100 text-green-800 border border-green-200' : 'bg-red-100 text-red-800 border border-red-200'}`;
            expBox.innerHTML = `<strong>${isCorrect ? 'सटीक उत्तर! 👍' : 'गलत उत्तर।'}</strong> ${q.explanation}`;
            expBox.classList.remove('hidden');
        }

        function nextQuestion() {
            if(currentQuestion < questions.length - 1) {
                currentQuestion++;
                loadQuestion();
            } else {
                showResult();
            }
        }

        function prevQuestion() {
            if(currentQuestion > 0) {
                currentQuestion--;
                loadQuestion();
            }
        }

        function showResult() {
            document.getElementById('quiz-container').classList.add('hidden');
            const res = document.getElementById('result-container');
            res.classList.remove('hidden');
            document.getElementById('score-display').innerText = `आपने 20 में से ${score} अंक प्राप्त किए हैं!`;
        }

        function restartQuiz() {
            currentQuestion = 0;
            score = 0;
            selectedOptions = new Array(questions.length).fill(null);
            document.getElementById('result-container').classList.add('hidden');
            document.getElementById('quiz-container').classList.remove('hidden');
            loadQuestion();
        }

        function toggleAnswer(id) {
            const el = document.getElementById(id);
            el.classList.toggle('hidden');
        }

        // Initial load
        window.onload = loadQuestion;
    </script>
</body>
</html>
```eof

यह इंटरैक्टिव प्रैक्टिस टेस्ट एप्लीकेशन आपके पूरे यूनिट टेस्ट 2 सिलेबस ('सती', 'आह! धरती कितना देती है', मुहावरे और अशुद्ध वाक्य संशोधन) को कवर करता है। आप इसे किसी भी वेब ब्राउज़र में खोलकर अपने स्कोर की जाँच कर सकते हैं और लिखित प्रश्नों के मॉडल उत्तर भी देख सकते हैं। परीक्षा के लिए शुभकामनाएँ!
