<!doctype html>
<html lang="en" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ISTEPS-ICT Educational Platform</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script src="/_sdk/element_sdk.js"></script>
  <style>
    body {
      box-sizing: border-box;
    }
    
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap');
    
    * {
      font-family: 'Inter', sans-serif;
    }
    
    .quiz-option {
      transition: all 0.2s ease;
      cursor: pointer;
    }
    
    .quiz-option:hover {
      transform: translateX(4px);
    }
    
    .quiz-option.selected {
      border-width: 2px;
    }
    
    .quiz-option.correct {
      animation: correctPulse 0.5s ease;
    }
    
    .quiz-option.incorrect {
      animation: shake 0.5s ease;
    }
    
    @keyframes correctPulse {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.02); }
    }
    
    @keyframes shake {
      0%, 100% { transform: translateX(0); }
      25% { transform: translateX(-10px); }
      75% { transform: translateX(10px); }
    }
    
    .fade-in {
      animation: fadeIn 0.3s ease;
    }
    
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .input-field {
      transition: all 0.2s ease;
    }

    .input-field:focus {
      outline: none;
      transform: translateY(-2px);
    }

    .timer-warning {
      animation: pulse 1s ease-in-out infinite;
    }

    @keyframes pulse {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.7; }
    }

    .timer-critical {
      animation: flashRed 0.5s ease-in-out infinite;
    }

    @keyframes flashRed {
      0%, 100% { background-color: #ef4444; }
      50% { background-color: #dc2626; }
    }
  </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
 </head>
 <body class="h-full">
  <div id="app-wrapper" class="h-full w-full overflow-auto"><!-- Main Content -->
   <div id="main-content" class="min-h-full w-full"><!-- Header -->
    <header class="w-full py-8 px-6 shadow-sm">
     <div class="max-w-6xl mx-auto">
      <h1 id="site-title" class="text-4xl font-bold mb-2">ISTEPS-ICT SELF TUTORING EDUCATIONAL PLATFORMS</h1>
      <p id="lesson-title" class="text-xl font-semibold">Lesson 4: Interactive Media</p>
     </div>
    </header><!-- Content Section -->
    <main class="w-full py-8 px-6">
     <div class="max-w-6xl mx-auto"><!-- Introduction -->
      <section class="mb-8 p-6 rounded-lg shadow-md">
       <h2 class="text-2xl font-bold mb-4">What is Interactive Multimedia?</h2>
       <p class="text-lg mb-4 leading-relaxed">Interactive Multimedia is defined as any computer-delivered electronic system that allows user to control, combine, and manipulate different types of media. It signifies that interactive multimedia is about using multimedia to provide information or communicate.</p>
      </section><!-- Uses Section -->
      <section class="mb-8 p-6 rounded-lg shadow-md">
       <h2 class="text-2xl font-bold mb-4">Uses of Interactive Multimedia</h2>
       <ul class="list-disc list-inside space-y-2 text-lg">
        <li>Education</li>
        <li>Training</li>
        <li>Games</li>
        <li>Simulation</li>
        <li>Information Presentation</li>
        <li>Corporate Presentation</li>
       </ul>
      </section><!-- Multimedia Definition -->
      <section class="mb-8 p-6 rounded-lg shadow-md">
       <h2 class="text-2xl font-bold mb-4">Multimedia</h2>
       <p class="text-lg leading-relaxed">Multimedia is a content that uses a combination of different content forms such as text, audio, images, animations, video and interactive content. Multimedia contrasts with media that use only rudimentary computer displays such as text-only or traditional forms of printed or hand-produced material.</p>
      </section><!-- Multimedia Contents -->
      <section class="mb-8 p-6 rounded-lg shadow-md">
       <h2 class="text-2xl font-bold mb-4">Multimedia Contents</h2>
       <div class="space-y-4">
        <div class="p-4 rounded-lg">
         <h3 class="text-xl font-semibold mb-2">1. Videos</h3>
         <p class="text-lg">Through video hosting sites, you can take a video and show it to the entire world (e.g. YouTube)</p>
        </div>
        <div class="p-4 rounded-lg">
         <h3 class="text-xl font-semibold mb-2">2. Sound, Music or Audio</h3>
         <p class="text-lg">If videos are too much for you, you can always record sounds. You can share your sound bites to the entire world (e.g. SoundCloud).</p>
        </div>
        <div class="p-4 rounded-lg">
         <h3 class="text-xl font-semibold mb-2">3. Online Games</h3>
         <p class="text-lg">Game developers now create what is called "browser-based games." You do not need to install these games to your computer as they run in most updated web browsers (AdventureQuest, Farmville, Candy Crush)</p>
        </div>
        <div class="p-4 rounded-lg">
         <h3 class="text-xl font-semibold mb-2">4. Online Tests</h3>
         <p class="text-lg">Online survey forms and tests that automatically display the results when finished (Online IQ and Personality Tests).</p>
        </div>
        <div class="p-4 rounded-lg">
         <h3 class="text-xl font-semibold mb-2">5. Courseware</h3>
         <p class="text-lg">Online courses that simulate the classroom online (e.g., E-learning Courses using a Learning Management System)</p>
        </div>
        <div class="p-4 rounded-lg">
         <h3 class="text-xl font-semibold mb-2">6. Podcasts</h3>
         <p class="text-lg">An episodic series of audio or text files streamed online (e.g., Stuff You Should Know, TED Talks, The Starters, Ear Biscuits).</p>
        </div>
        <div class="p-4 rounded-lg">
         <h3 class="text-xl font-semibold mb-2">7. Vodcasts</h3>
         <p class="text-lg">An episodic series of video streamed online (e.g., YouTube series/shows like Video Game High School, Good Mythical Morning).</p>
        </div>
       </div>
      </section><!-- Quiz Button -->
      <div class="text-center mb-12"><button id="quiz-button" class="px-8 py-4 rounded-lg font-bold text-xl shadow-lg hover:shadow-xl transition-all duration-200 transform hover:scale-105"> 📝 Take the Quiz </button>
      </div>
     </div>
    </main><!-- Footer -->
    <footer class="w-full py-6 px-6 text-center">
     <p id="footer-text" class="text-base font-semibold mb-1">Research Study by JOEL P. RODRIGUEZ, LPT, MAVEd</p>
     <p class="text-sm">© 2024 ISTEPS-ICT Educational Platform</p>
    </footer>
   </div><!-- Quiz Modal -->
   <div id="quiz-modal" class="fixed inset-0 flex items-center justify-center p-4 hidden" style="z-index: 1000;">
    <div class="absolute inset-0 opacity-90"></div>
    <div class="relative w-full max-w-3xl max-h-[90%] overflow-y-auto rounded-xl shadow-2xl p-8"><button id="close-quiz" class="absolute top-4 right-4 text-3xl font-bold hover:opacity-70 transition-opacity">×</button>
     <h2 id="quiz-title" class="text-3xl font-bold mb-6 text-center">Interactive Media Quiz</h2><!-- Student Information Form -->
     <div id="student-info-form" class="mb-8">
      <div class="space-y-4">
       <div><label for="student-name" class="block text-lg font-semibold mb-2">Name:</label> <input type="text" id="student-name" class="input-field w-full px-4 py-3 rounded-lg border-2" placeholder="Enter your full name" required>
       </div>
       <div><label for="student-grade" class="block text-lg font-semibold mb-2">Grade:</label> <input type="text" id="student-grade" class="input-field w-full px-4 py-3 rounded-lg border-2" placeholder="Enter your grade level" required>
       </div>
       <div><label for="student-section" class="block text-lg font-semibold mb-2">Section:</label> <input type="text" id="student-section" class="input-field w-full px-4 py-3 rounded-lg border-2" placeholder="Enter your section" required>
       </div>
       <div id="info-error" class="text-red-600 font-semibold hidden">
        Please fill in all fields before starting the quiz.
       </div><button id="start-quiz-button" class="w-full py-3 rounded-lg font-semibold shadow-md hover:shadow-lg transition-all"> Start Quiz → </button>
      </div>
     </div><!-- Student Info Display (shown during quiz) -->
     <div id="student-info-display" class="mb-6 p-4 rounded-lg hidden">
      <div class="flex justify-between items-center flex-wrap gap-2">
       <div>
        <span class="font-semibold">Name:</span> <span id="display-name"></span>
       </div>
       <div>
        <span class="font-semibold">Grade:</span> <span id="display-grade"></span>
       </div>
       <div>
        <span class="font-semibold">Section:</span> <span id="display-section"></span>
       </div>
      </div>
     </div><!-- Timer Display -->
     <div id="timer-display" class="mb-6 p-4 rounded-lg text-center font-bold text-2xl hidden">
      ⏱️ Time Remaining: <span id="timer-value">3:00</span>
     </div>
     <div id="quiz-container"></div>
     <div id="quiz-navigation" class="mt-8 flex justify-between items-center hidden"><button id="prev-button" class="px-6 py-3 rounded-lg font-semibold shadow-md hover:shadow-lg transition-all disabled:opacity-50 disabled:cursor-not-allowed"> ← Previous </button>
      <div id="question-counter" class="text-lg font-semibold"></div><button id="next-button" class="px-6 py-3 rounded-lg font-semibold shadow-md hover:shadow-lg transition-all"> Next → </button> <button id="submit-button" class="px-6 py-3 rounded-lg font-semibold shadow-md hover:shadow-lg transition-all hidden"> Submit Quiz </button>
     </div>
     <div id="quiz-results" class="mt-8 p-6 rounded-lg hidden">
      <div class="mb-4 p-4 rounded-lg">
       <div class="text-center mb-2">
        <p class="font-semibold">Student Information</p>
       </div>
       <div class="space-y-1 text-center">
        <p><span class="font-semibold">Name:</span> <span id="result-name"></span></p>
        <p><span class="font-semibold">Grade:</span> <span id="result-grade"></span></p>
        <p><span class="font-semibold">Section:</span> <span id="result-section"></span></p>
       </div>
      </div>
      <h3 class="text-2xl font-bold mb-4 text-center">Quiz Results</h3>
      <div class="text-center mb-6">
       <p class="text-5xl font-bold mb-2" id="score-display"></p>
       <p class="text-xl" id="score-message"></p>
      </div><button id="retry-button" class="w-full py-3 rounded-lg font-semibold shadow-md hover:shadow-lg transition-all"> Retry Quiz </button>
     </div>
    </div>
   </div>
  </div>
  <script>
    const defaultConfig = {
      background_color: '#f0f4f8',
      surface_color: '#ffffff',
      text_color: '#1e293b',
      primary_action_color: '#3b82f6',
      secondary_action_color: '#64748b',
      font_family: 'Inter',
      font_size: 16,
      site_title: 'ISTEPS-ICT SELF TUTORING EDUCATIONAL PLATFORMS',
      lesson_title: 'Lesson 4: Interactive Media',
      quiz_button_text: '📝 Take the Quiz',
      quiz_title: 'Interactive Media Quiz',
      footer_text: 'Research Study by JOEL P. RODRIGUEZ, LPT, MAVEd'
    };

    const quizQuestions = [
      {
        question: "What is Interactive Multimedia?",
        options: [
          "A printed textbook with images",
          "Any computer-delivered electronic system that allows user to control, combine, and manipulate different types of media",
          "A television broadcast",
          "A radio program"
        ],
        correct: 1
      },
      {
        question: "Which of the following is NOT a use of Interactive Multimedia?",
        options: [
          "Education",
          "Training",
          "Handwritten letters",
          "Games"
        ],
        correct: 2
      },
      {
        question: "Multimedia is a content that uses a combination of different content forms. Which is NOT mentioned as a multimedia content form?",
        options: [
          "Text",
          "Audio",
          "Smell",
          "Video"
        ],
        correct: 2
      },
      {
        question: "Which platform is mentioned as an example for sharing videos?",
        options: [
          "SoundCloud",
          "YouTube",
          "Spotify",
          "Netflix"
        ],
        correct: 1
      },
      {
        question: "What is SoundCloud used for?",
        options: [
          "Sharing videos",
          "Playing games",
          "Sharing sound bites and audio",
          "Online testing"
        ],
        correct: 2
      },
      {
        question: "What are browser-based games?",
        options: [
          "Games that require installation",
          "Games that run in most updated web browsers without installation",
          "Games only for mobile phones",
          "Games that require special hardware"
        ],
        correct: 1
      },
      {
        question: "Which of the following is an example of a browser-based game?",
        options: [
          "YouTube",
          "SoundCloud",
          "Candy Crush",
          "TED Talks"
        ],
        correct: 2
      },
      {
        question: "What are Online Tests in multimedia context?",
        options: [
          "Printed exams",
          "Online survey forms and tests that automatically display results when finished",
          "Video tutorials",
          "Audio lectures"
        ],
        correct: 1
      },
      {
        question: "What is Courseware?",
        options: [
          "Physical textbooks",
          "Online courses that simulate the classroom online",
          "Video games",
          "Music streaming"
        ],
        correct: 1
      },
      {
        question: "A Podcast is best described as:",
        options: [
          "A video series",
          "An episodic series of audio or text files streamed online",
          "A browser game",
          "An online test"
        ],
        correct: 1
      },
      {
        question: "Which is an example of a Podcast?",
        options: [
          "Candy Crush",
          "YouTube",
          "TED Talks",
          "Farmville"
        ],
        correct: 2
      },
      {
        question: "What is a Vodcast?",
        options: [
          "An audio-only podcast",
          "An episodic series of video streamed online",
          "An online test",
          "A browser game"
        ],
        correct: 1
      },
      {
        question: "Which is mentioned as an example of Vodcast content?",
        options: [
          "SoundCloud files",
          "Candy Crush",
          "Good Mythical Morning",
          "Online IQ tests"
        ],
        correct: 2
      },
      {
        question: "Interactive Multimedia is primarily about:",
        options: [
          "Using only text for communication",
          "Using multimedia to provide information or communicate with user control",
          "Watching television passively",
          "Reading printed books"
        ],
        correct: 1
      },
      {
        question: "Which of the following is NOT mentioned as a use of Interactive Multimedia?",
        options: [
          "Simulation",
          "Information Presentation",
          "Weather forecasting",
          "Corporate Presentation"
        ],
        correct: 2
      }
    ];

    let currentQuestion = 0;
    let userAnswers = new Array(quizQuestions.length).fill(null);
    let quizSubmitted = false;
    let studentInfo = {
      name: '',
      grade: '',
      section: ''
    };
    let timeRemaining = 180; // 3 minutes in seconds
    let timerInterval = null;
    let timeUsed = 0;

    async function onConfigChange(config) {
      const baseFontSize = config.font_size || defaultConfig.font_size;
      const customFont = config.font_family || defaultConfig.font_family;
      const fontStack = `${customFont}, Arial, sans-serif`;

      const backgroundColor = config.background_color || defaultConfig.background_color;
      const surfaceColor = config.surface_color || defaultConfig.surface_color;
      const textColor = config.text_color || defaultConfig.text_color;
      const primaryColor = config.primary_action_color || defaultConfig.primary_action_color;
      const secondaryColor = config.secondary_action_color || defaultConfig.secondary_action_color;

      document.getElementById('app-wrapper').style.backgroundColor = backgroundColor;
      document.getElementById('app-wrapper').style.color = textColor;
      
      document.querySelector('header').style.backgroundColor = surfaceColor;
      document.querySelector('header').style.color = textColor;
      document.querySelector('footer').style.backgroundColor = surfaceColor;
      document.querySelector('footer').style.color = textColor;

      const sections = document.querySelectorAll('section');
      sections.forEach(section => {
        section.style.backgroundColor = surfaceColor;
        section.style.color = textColor;
      });

      const contentDivs = document.querySelectorAll('section > div > div');
      contentDivs.forEach(div => {
        div.style.backgroundColor = backgroundColor;
      });

      document.getElementById('quiz-button').style.backgroundColor = primaryColor;
      document.getElementById('quiz-button').style.color = surfaceColor;

      const modal = document.querySelector('#quiz-modal > div:last-child');
      modal.style.backgroundColor = surfaceColor;
      modal.style.color = textColor;

      document.querySelector('#quiz-modal > div:first-child').style.backgroundColor = textColor;

      document.getElementById('close-quiz').style.color = textColor;

      document.getElementById('prev-button').style.backgroundColor = secondaryColor;
      document.getElementById('prev-button').style.color = surfaceColor;
      document.getElementById('next-button').style.backgroundColor = primaryColor;
      document.getElementById('next-button').style.color = surfaceColor;
      document.getElementById('submit-button').style.backgroundColor = primaryColor;
      document.getElementById('submit-button').style.color = surfaceColor;
      document.getElementById('start-quiz-button').style.backgroundColor = primaryColor;
      document.getElementById('start-quiz-button').style.color = surfaceColor;
      document.getElementById('retry-button').style.backgroundColor = primaryColor;
      document.getElementById('retry-button').style.color = surfaceColor;

      document.getElementById('quiz-results').style.backgroundColor = backgroundColor;
      document.getElementById('student-info-display').style.backgroundColor = backgroundColor;

      const inputFields = document.querySelectorAll('.input-field');
      inputFields.forEach(input => {
        input.style.backgroundColor = surfaceColor;
        input.style.borderColor = secondaryColor;
        input.style.color = textColor;
      });

      const labels = document.querySelectorAll('#student-info-form label');
      labels.forEach(label => {
        label.style.color = textColor;
        label.style.fontFamily = fontStack;
        label.style.fontSize = `${baseFontSize * 1.125}px`;
      });

      document.getElementById('site-title').textContent = config.site_title || defaultConfig.site_title;
      document.getElementById('lesson-title').textContent = config.lesson_title || defaultConfig.lesson_title;
      document.getElementById('quiz-button').textContent = config.quiz_button_text || defaultConfig.quiz_button_text;
      document.getElementById('quiz-title').textContent = config.quiz_title || defaultConfig.quiz_title;
      document.getElementById('footer-text').textContent = config.footer_text || defaultConfig.footer_text;

      document.getElementById('site-title').style.fontFamily = fontStack;
      document.getElementById('site-title').style.fontSize = `${baseFontSize * 2}px`;

      document.getElementById('lesson-title').style.fontFamily = fontStack;
      document.getElementById('lesson-title').style.fontSize = `${baseFontSize * 1.25}px`;

      document.getElementById('footer-text').style.fontFamily = fontStack;
      document.getElementById('footer-text').style.fontSize = `${baseFontSize}px`;

      const allHeadings = document.querySelectorAll('h2, h3');
      allHeadings.forEach(heading => {
        heading.style.fontFamily = fontStack;
        if (heading.tagName === 'H2') {
          heading.style.fontSize = `${baseFontSize * 1.5}px`;
        } else if (heading.tagName === 'H3') {
          heading.style.fontSize = `${baseFontSize * 1.25}px`;
        }
      });

      const allParagraphs = document.querySelectorAll('p, li');
      allParagraphs.forEach(p => {
        p.style.fontFamily = fontStack;
        p.style.fontSize = `${baseFontSize}px`;
      });

      document.getElementById('quiz-button').style.fontFamily = fontStack;
      document.getElementById('quiz-button').style.fontSize = `${baseFontSize * 1.25}px`;

      document.getElementById('quiz-title').style.fontFamily = fontStack;
      document.getElementById('quiz-title').style.fontSize = `${baseFontSize * 1.875}px`;

      document.getElementById('start-quiz-button').style.fontFamily = fontStack;
      document.getElementById('start-quiz-button').style.fontSize = `${baseFontSize}px`;

      updateQuizColors();
    }

    function updateTimer() {
      const minutes = Math.floor(timeRemaining / 60);
      const seconds = timeRemaining % 60;
      const timerValue = document.getElementById('timer-value');
      const timerDisplay = document.getElementById('timer-display');
      const config = window.elementSdk.config;
      const surfaceColor = config.surface_color || defaultConfig.surface_color;
      const textColor = config.text_color || defaultConfig.text_color;
      
      timerValue.textContent = `${minutes}:${seconds.toString().padStart(2, '0')}`;
      
      // Change color based on time remaining
      if (timeRemaining <= 30) {
        timerDisplay.style.backgroundColor = '#ef4444';
        timerDisplay.style.color = surfaceColor;
        timerDisplay.classList.add('timer-critical');
        timerDisplay.classList.remove('timer-warning');
      } else if (timeRemaining <= 60) {
        timerDisplay.style.backgroundColor = '#f59e0b';
        timerDisplay.style.color = surfaceColor;
        timerDisplay.classList.add('timer-warning');
        timerDisplay.classList.remove('timer-critical');
      } else {
        timerDisplay.style.backgroundColor = '#10b981';
        timerDisplay.style.color = surfaceColor;
        timerDisplay.classList.remove('timer-warning', 'timer-critical');
      }
    }

    function startTimer() {
      if (timerInterval) {
        clearInterval(timerInterval);
      }
      
      timerInterval = setInterval(() => {
        timeRemaining--;
        timeUsed++;
        updateTimer();
        
        if (timeRemaining <= 0) {
          clearInterval(timerInterval);
          autoSubmitQuiz();
        }
      }, 1000);
    }

    function stopTimer() {
      if (timerInterval) {
        clearInterval(timerInterval);
        timerInterval = null;
      }
    }

    function addBonusTime() {
      timeRemaining += 60; // Add 1 minute (60 seconds)
      updateTimer();
    }

    function autoSubmitQuiz() {
      if (!quizSubmitted) {
        const timerDisplay = document.getElementById('timer-display');
        timerDisplay.innerHTML = '⏰ <strong>Time\'s Up!</strong> Quiz auto-submitted.';
        
        setTimeout(() => {
          submitQuiz();
        }, 1500);
      }
    }

    function updateQuizColors() {
      const config = window.elementSdk.config;
      const backgroundColor = config.background_color || defaultConfig.background_color;
      const surfaceColor = config.surface_color || defaultConfig.surface_color;
      const textColor = config.text_color || defaultConfig.text_color;
      const primaryColor = config.primary_action_color || defaultConfig.primary_action_color;
      const secondaryColor = config.secondary_action_color || defaultConfig.secondary_action_color;

      const options = document.querySelectorAll('.quiz-option');
      options.forEach(option => {
        if (option.classList.contains('selected') && !quizSubmitted) {
          option.style.backgroundColor = primaryColor;
          option.style.borderColor = primaryColor;
          option.style.color = surfaceColor;
        } else if (option.classList.contains('correct')) {
          option.style.backgroundColor = '#10b981';
          option.style.borderColor = '#10b981';
          option.style.color = surfaceColor;
        } else if (option.classList.contains('incorrect')) {
          option.style.backgroundColor = '#ef4444';
          option.style.borderColor = '#ef4444';
          option.style.color = surfaceColor;
        } else {
          option.style.backgroundColor = surfaceColor;
          option.style.borderColor = secondaryColor;
          option.style.color = textColor;
        }
      });
    }

    function showQuestion(index) {
      const container = document.getElementById('quiz-container');
      const question = quizQuestions[index];
      const config = window.elementSdk.config;
      const baseFontSize = config.font_size || defaultConfig.font_size;
      const customFont = config.font_family || defaultConfig.font_family;
      const fontStack = `${customFont}, Arial, sans-serif`;
      const backgroundColor = config.background_color || defaultConfig.background_color;
      const surfaceColor = config.surface_color || defaultConfig.surface_color;
      const textColor = config.text_color || defaultConfig.text_color;
      const primaryColor = config.primary_action_color || defaultConfig.primary_action_color;
      const secondaryColor = config.secondary_action_color || defaultConfig.secondary_action_color;

      container.innerHTML = `
        <div class="fade-in">
          <h3 class="text-xl font-semibold mb-6" style="font-family: ${fontStack}; font-size: ${baseFontSize * 1.25}px; color: ${textColor};">
            Question ${index + 1}: ${question.question}
          </h3>
          <div class="space-y-3">
            ${question.options.map((option, i) => {
              let optionClass = 'quiz-option border-2 p-4 rounded-lg';
              let optionStyle = `font-family: ${fontStack}; font-size: ${baseFontSize}px; background-color: ${surfaceColor}; border-color: ${secondaryColor}; color: ${textColor};`;
              
              if (quizSubmitted) {
                if (i === question.correct) {
                  optionClass += ' correct';
                  optionStyle = `font-family: ${fontStack}; font-size: ${baseFontSize}px; background-color: #10b981; border-color: #10b981; color: ${surfaceColor};`;
                } else if (userAnswers[index] === i) {
                  optionClass += ' incorrect';
                  optionStyle = `font-family: ${fontStack}; font-size: ${baseFontSize}px; background-color: #ef4444; border-color: #ef4444; color: ${surfaceColor};`;
                }
              } else if (userAnswers[index] === i) {
                optionClass += ' selected';
                optionStyle = `font-family: ${fontStack}; font-size: ${baseFontSize}px; background-color: ${primaryColor}; border-color: ${primaryColor}; color: ${surfaceColor};`;
              }
              
              return `<div class="${optionClass}" data-option="${i}" style="${optionStyle}">${String.fromCharCode(65 + i)}. ${option}</div>`;
            }).join('')}
          </div>
        </div>
      `;

      if (!quizSubmitted) {
        container.querySelectorAll('.quiz-option').forEach(opt => {
          opt.addEventListener('click', function() {
            const optionIndex = parseInt(this.dataset.option);
            const wasAnswered = userAnswers[currentQuestion] !== null;
            const previousAnswer = userAnswers[currentQuestion];
            
            userAnswers[currentQuestion] = optionIndex;
            
            // Add bonus time only if this is a new correct answer
            if (!wasAnswered && optionIndex === question.correct) {
              addBonusTime();
              
              // Show bonus notification
              const timerDisplay = document.getElementById('timer-display');
              const originalContent = timerDisplay.innerHTML;
              timerDisplay.innerHTML = '🎉 <strong>+1 Minute Bonus!</strong> Correct answer!';
              timerDisplay.style.backgroundColor = '#10b981';
              
              setTimeout(() => {
                timerDisplay.innerHTML = originalContent;
                updateTimer();
              }, 2000);
            }
            
            showQuestion(currentQuestion);
          });
        });
      }

      updateNavigation();
    }

    function updateNavigation() {
      const prevButton = document.getElementById('prev-button');
      const nextButton = document.getElementById('next-button');
      const submitButton = document.getElementById('submit-button');
      const counter = document.getElementById('question-counter');
      const config = window.elementSdk.config;
      const baseFontSize = config.font_size || defaultConfig.font_size;
      const customFont = config.font_family || defaultConfig.font_family;
      const fontStack = `${customFont}, Arial, sans-serif`;
      const textColor = config.text_color || defaultConfig.text_color;

      counter.textContent = `${currentQuestion + 1} / ${quizQuestions.length}`;
      counter.style.fontFamily = fontStack;
      counter.style.fontSize = `${baseFontSize * 1.125}px`;
      counter.style.color = textColor;

      prevButton.disabled = currentQuestion === 0;

      if (currentQuestion === quizQuestions.length - 1) {
        nextButton.classList.add('hidden');
        if (!quizSubmitted) {
          submitButton.classList.remove('hidden');
        } else {
          submitButton.classList.add('hidden');
        }
      } else {
        nextButton.classList.remove('hidden');
        submitButton.classList.add('hidden');
      }

      prevButton.style.fontFamily = fontStack;
      prevButton.style.fontSize = `${baseFontSize}px`;
      nextButton.style.fontFamily = fontStack;
      nextButton.style.fontSize = `${baseFontSize}px`;
      submitButton.style.fontFamily = fontStack;
      submitButton.style.fontSize = `${baseFontSize}px`;
    }

    function startQuiz() {
      const name = document.getElementById('student-name').value.trim();
      const grade = document.getElementById('student-grade').value.trim();
      const section = document.getElementById('student-section').value.trim();

      if (!name || !grade || !section) {
        document.getElementById('info-error').classList.remove('hidden');
        return;
      }

      document.getElementById('info-error').classList.add('hidden');

      studentInfo = { name, grade, section };

      document.getElementById('display-name').textContent = name;
      document.getElementById('display-grade').textContent = grade;
      document.getElementById('display-section').textContent = section;

      document.getElementById('student-info-form').classList.add('hidden');
      document.getElementById('student-info-display').classList.remove('hidden');
      document.getElementById('timer-display').classList.remove('hidden');
      document.getElementById('quiz-navigation').classList.remove('hidden');

      // Start the timer
      timeRemaining = 180;
      timeUsed = 0;
      updateTimer();
      startTimer();

      showQuestion(currentQuestion);
    }

    function submitQuiz() {
      stopTimer();
      quizSubmitted = true;
      let score = 0;

      quizQuestions.forEach((question, index) => {
        if (userAnswers[index] === question.correct) {
          score++;
        }
      });

      const percentage = Math.round((score / quizQuestions.length) * 100);
      const config = window.elementSdk.config;
      const baseFontSize = config.font_size || defaultConfig.font_size;
      const customFont = config.font_family || defaultConfig.font_family;
      const fontStack = `${customFont}, Arial, sans-serif`;
      const textColor = config.text_color || defaultConfig.text_color;

      document.getElementById('result-name').textContent = studentInfo.name;
      document.getElementById('result-grade').textContent = studentInfo.grade;
      document.getElementById('result-section').textContent = studentInfo.section;

      const scoreDisplay = document.getElementById('score-display');
      const scoreMessage = document.getElementById('score-message');
      
      const timeMinutes = Math.floor(timeUsed / 60);
      const timeSeconds = timeUsed % 60;
      const timeString = `${timeMinutes}:${timeSeconds.toString().padStart(2, '0')}`;
      
      scoreDisplay.textContent = `${score}/${quizQuestions.length} (${percentage}%)`;
      scoreDisplay.style.fontFamily = fontStack;
      scoreDisplay.style.fontSize = `${baseFontSize * 3}px`;
      scoreDisplay.style.color = textColor;

      let message = '';
      if (percentage >= 90) {
        message = `Excellent! You have mastered this topic! 🎉 Time: ${timeString}`;
      } else if (percentage >= 75) {
        message = `Great job! You have a good understanding! 👏 Time: ${timeString}`;
      } else if (percentage >= 60) {
        message = `Good effort! Review the material for better results. 📚 Time: ${timeString}`;
      } else {
        message = `Keep studying! You can do better! 💪 Time: ${timeString}`;
      }

      scoreMessage.textContent = message;
      scoreMessage.style.fontFamily = fontStack;
      scoreMessage.style.fontSize = `${baseFontSize * 1.25}px`;
      scoreMessage.style.color = textColor;

      document.getElementById('quiz-results').classList.remove('hidden');
      document.getElementById('quiz-navigation').classList.add('hidden');
      document.getElementById('student-info-display').classList.add('hidden');
      document.getElementById('timer-display').classList.add('hidden');

      currentQuestion = 0;
      showQuestion(currentQuestion);
    }

    function resetQuiz() {
      stopTimer();
      currentQuestion = 0;
      userAnswers = new Array(quizQuestions.length).fill(null);
      quizSubmitted = false;
      timeRemaining = 180;
      timeUsed = 0;

      document.getElementById('student-name').value = '';
      document.getElementById('student-grade').value = '';
      document.getElementById('student-section').value = '';

      document.getElementById('quiz-results').classList.add('hidden');
      document.getElementById('student-info-display').classList.add('hidden');
      document.getElementById('quiz-navigation').classList.add('hidden');
      document.getElementById('timer-display').classList.add('hidden');
      document.getElementById('student-info-form').classList.remove('hidden');
      document.getElementById('info-error').classList.add('hidden');
    }

    document.getElementById('quiz-button').addEventListener('click', function() {
      document.getElementById('quiz-modal').classList.remove('hidden');
      resetQuiz();
    });

    document.getElementById('close-quiz').addEventListener('click', function() {
      document.getElementById('quiz-modal').classList.add('hidden');
    });

    document.getElementById('start-quiz-button').addEventListener('click', function() {
      startQuiz();
    });

    document.getElementById('prev-button').addEventListener('click', function() {
      if (currentQuestion > 0) {
        currentQuestion--;
        showQuestion(currentQuestion);
      }
    });

    document.getElementById('next-button').addEventListener('click', function() {
      if (currentQuestion < quizQuestions.length - 1) {
        currentQuestion++;
        showQuestion(currentQuestion);
      }
    });

    document.getElementById('submit-button').addEventListener('click', function() {
      submitQuiz();
    });

    document.getElementById('retry-button').addEventListener('click', function() {
      resetQuiz();
    });

    document.getElementById('quiz-modal').addEventListener('click', function(e) {
      if (e.target === this) {
        this.classList.add('hidden');
      }
    });

    document.getElementById('student-name').addEventListener('keypress', function(e) {
      if (e.key === 'Enter') {
        e.preventDefault();
        document.getElementById('student-grade').focus();
      }
    });

    document.getElementById('student-grade').addEventListener('keypress', function(e) {
      if (e.key === 'Enter') {
        e.preventDefault();
        document.getElementById('student-section').focus();
      }
    });

    document.getElementById('student-section').addEventListener('keypress', function(e) {
      if (e.key === 'Enter') {
        e.preventDefault();
        startQuiz();
      }
    });

    if (window.elementSdk) {
      window.elementSdk.init({
        defaultConfig,
        onConfigChange,
        mapToCapabilities: (config) => ({
          recolorables: [
            {
              get: () => config.background_color || defaultConfig.background_color,
              set: (value) => {
                config.background_color = value;
                window.elementSdk.setConfig({ background_color: value });
              }
            },
            {
              get: () => config.surface_color || defaultConfig.surface_color,
              set: (value) => {
                config.surface_color = value;
                window.elementSdk.setConfig({ surface_color: value });
              }
            },
            {
              get: () => config.text_color || defaultConfig.text_color,
              set: (value) => {
                config.text_color = value;
                window.elementSdk.setConfig({ text_color: value });
              }
            },
            {
              get: () => config.primary_action_color || defaultConfig.primary_action_color,
              set: (value) => {
                config.primary_action_color = value;
                window.elementSdk.setConfig({ primary_action_color: value });
              }
            },
            {
              get: () => config.secondary_action_color || defaultConfig.secondary_action_color,
              set: (value) => {
                config.secondary_action_color = value;
                window.elementSdk.setConfig({ secondary_action_color: value });
              }
            }
          ],
          borderables: [],
          fontEditable: {
            get: () => config.font_family || defaultConfig.font_family,
            set: (value) => {
              config.font_family = value;
              window.elementSdk.setConfig({ font_family: value });
            }
          },
          fontSizeable: {
            get: () => config.font_size || defaultConfig.font_size,
            set: (value) => {
              config.font_size = value;
              window.elementSdk.setConfig({ font_size: value });
            }
          }
        }),
        mapToEditPanelValues: (config) => new Map([
          ['site_title', config.site_title || defaultConfig.site_title],
          ['lesson_title', config.lesson_title || defaultConfig.lesson_title],
          ['quiz_button_text', config.quiz_button_text || defaultConfig.quiz_button_text],
          ['quiz_title', config.quiz_title || defaultConfig.quiz_title],
          ['footer_text', config.footer_text || defaultConfig.footer_text]
        ])
      });
    }

    onConfigChange(defaultConfig);
  </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9b9f530831e8043d',t:'MTc2Nzc0NTU5My4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
