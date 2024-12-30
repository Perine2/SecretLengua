# SecretLengua
<section>
  <h2>Codes utilisés dans Secret Lengua</h2>
  <ul>
    <li><strong>Code 1:</<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Weather</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #fFfFfF.
            color: #333;
            margin: 20px;
            line-height: 1.6;
        }
        .content {
            max-width: 700px;
            margin: auto;
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 1);
        }
        .title {
            font-size: 24px;
            font-weight: bold;
            text-align: center;
            margin-bottom: 20px;
        }
        .paragraph {
            margin-bottom: 15px;
            text-align: justify;
        }
    </style>
</head>
<body>

<div class="content">
    <div class="title">Weather</div>

    <div class="paragraph">
Weather, or the state of atmospheric conditions during a given period, directly impacts individuals' mood, outdoor activities that can be enjoyed, and much more.
Sunny weather is, as most would guess, characterized by sunlight. Sunny days can be encountered during each of the four seasons, but are most common in summer and least common in spring (which is known for its "showers" or precipitation).
Cloudy weather is one that has a covered sky, or a gray and cloud-filled atmosphere, without sunlight. Cloudy weather can occur during all four seasons, but as it often precedes rain, it is most common in spring.   </div>
    <div class="paragraph">

Rainy weather is simply weather where it is raining. Rain can fall during each of the four seasons, but is most common in spring and least common in winter (as temperatures are so low that precipitation may turn into snow or sleet before reaching the ground).
Snowy weather occurs almost exclusively in winter, late autumn, and early spring, and is characterized by snow, or frozen, white, fluffy water that falls from the sky. Snow can fall gently on the ground, or reach the ground in the form of a snowstorm or blizzard, or episodes of powerful, windy, and potentially dangerous snowfall.
Ice is a slippery and potentially dangerous substance formed by water that freezes quickly when exposed to temperatures colder than 32 degrees Fahrenheit.   </div>
    <div class="paragraph">
Hail is a substance that falls from the sky in a state somewhere between snow and ice, meaning it has frozen fast enough to skip the snow stage but not fast enough to become full-fledged ice. Hail is seen almost exclusively in winter (although it can accompany spring precipitation).
Fog is a visible but untouchable vapor that limits visibility and can result from various factors, including humidity, temperature, elevation, and more.
A rainbow is a colorful collection of gases that forms in the sky, usually when rain is falling while the sun is still shining. This somewhat rare event is generally considered beautiful.      </div>                                                                                  
                        </div>
</body>
</html>> [Texte]</li>
    
    <li><strong>Code 2:</<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Questions de Compréhension</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffffff;
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        .container {
            width: 100%;
            max-width: 600px;
            background-color: white;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .question-box {
            background-color: #f0000F;
            color: WHITE;
            font-weight: bold;
            padding: 5px;
            border-radius: 5px;
            margin-bottom: 10px;
            text-align: center;
            width: 150px;
            margin-left: 0;
        }
        .question {
            font-size: 14px;
            margin-bottom: 10px;
            text-align: left;
        }
        .options {
            display: flex;
            flex-direction: column;
            gap: 5px;
        }
        .options label {
            font-size: 12px;
            color: #333;
            display: flex;
            align-items: center;
        }
        input[type="radio"] {
            margin-right: 10px;
        }
        .correct .circle {
            width: 15px;
            height: 15px;
            background-color: green;
            border-radius: 50%;
            margin-left: 10px;
            display: inline-block;
        }
        .incorrect {
            color: red;
            font-weight: bold;
            text-decoration: line-through;
        }
        .result {
            margin-top: 20px;
            padding: 10px;
            background-color: #ffccd5;
            text-align: center;
            border-radius: 5px;
            display: none;
        }
        .score-circle {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-top: 20px;
            font-weight: bold;
            font-size: 18px;
        }
        .low-score {
            background-color: red;
        }
        .mid-score {
            background-color: pink;
        }
        .high-score {
            background-color: green;
        }
    </style>
</head>
<body>
    <div class="container">
        <div id="quiz">
     <!-- Question 1 -->
            <div class="question-box">Question 1</div>
            <div class="question">She is ___ tired after the long journey. (très)</div>
            <div class="options">
                <label><input type="radio" name="q1" value="a" onclick="verifierReponse(this, 'b')"> a) slightly</label>
                <label><input type="radio" name="q1" value="b" onclick="verifierReponse(this, 'b')"> b) very</label>
                <label><input type="radio" name="q1" value="c" onclick="verifierReponse(this, 'b')"> c) hardly</label>
            </div>

            <!-- Question 2 -->
            <div class="question-box">Question 2</div>
            <div class="question">He was ___ pleased with the results. (extrêmement)</div>
            <div class="options">
                <label><input type="radio" name="q2" value="a" onclick="verifierReponse(this, 'a')"> a) extremely</label>
                <label><input type="radio" name="q2" value="b" onclick="verifierReponse(this, 'a')"> b) just</label>
                <label><input type="radio" name="q2" value="c" onclick="verifierReponse(this, 'a')"> c) slightly</label>
            </div>

            <!-- Question 3 -->
            <div class="question-box">Question 3</div>
            <div class="question">They were ___ happy about the news. (absolument)</div>
            <div class="options">
                <label><input type="radio" name="q3" value="a" onclick="verifierReponse(this, 'a')"> a) absolutely</label>
                <label><input type="radio" name="q3" value="b" onclick="verifierReponse(this, 'a')"> b) just</label>
                <label><input type="radio" name="q3" value="c" onclick="verifierReponse(this, 'a')"> c) slightly</label>
            </div>

            <!-- Question 4 -->
            <div class="question-box">Question 4</div>
            <div class="question">The movie was ___ interesting. (assez)</div>
            <div class="options">
                <label><input type="radio" name="q4" value="a" onclick="verifierReponse(this, 'b')"> a) almost</label>
                <label><input type="radio" name="q4" value="b" onclick="verifierReponse(this, 'b')"> b) quite</label>
                <label><input type="radio" name="q4" value="c" onclick="verifierReponse(this, 'b')"> c) just</label>
            </div>

            <!-- Question 5 -->
            <div class="question-box">Question 5</div>
            <div class="question">She is ___ better now. (beaucoup)</div>
            <div class="options">
                <label><input type="radio" name="q5" value="a" onclick="verifierReponse(this, 'a')"> a) much</label>
                <label><input type="radio" name="q5" value="b" onclick="verifierReponse(this, 'a')"> b) slightly</label>
                <label><input type="radio" name="q5" value="c" onclick="verifierReponse(this, 'a')"> c) hardly</label>
            </div>

            <!-- Question 6 -->
            <div class="question-box">Question 6</div>
            <div class="question">He is ___ the best player on the team. (probablement)</div>
            <div class="options">
                <label><input type="radio" name="q6" value="a" onclick="verifierReponse(this, 'c')"> a) absolutely</label>
                <label><input type="radio" name="q6" value="b" onclick="verifierReponse(this, 'c')"> b) nearly</label>
                <label><input type="radio" name="q6" value="c" onclick="verifierReponse(this, 'c')"> c) probably</label>
            </div>

            <!-- Question 7 -->
            <div class="question-box">Question 7</div>
            <div class="question">The weather is ___ good today. (plutôt)</div>
            <div class="options">
                <label><input type="radio" name="q7" value="a" onclick="verifierReponse(this, 'b')"> a) very</label>
                <label><input type="radio" name="q7" value="b" onclick="verifierReponse(this, 'b')"> b) rather</label>
                <label><input type="radio" name="q7" value="c" onclick="verifierReponse(this, 'b')"> c) just</label>
            </div>

            <!-- Question 8 -->
            <div class="question-box">Question 8</div>
            <div class="question">She was ___ surprised by the gift. (agréablement)</div>
            <div class="options">
                <label><input type="radio" name="q8" value="a" onclick="verifierReponse(this, 'c')"> a) very</label>
                <label><input type="radio" name="q8" value="b" onclick="verifierReponse(this, 'c')"> b) almost</label>
                <label><input type="radio" name="q8" value="c" onclick="verifierReponse(this, 'c')"> c) pleasantly</label>
            </div>

            <!-- Question 9 -->
            <div class="question-box">Question 9</div>
            <div class="question">The book is ___ interesting. (extrêmement)</div>
            <div class="options">
                <label><input type="radio" name="q9" value="a" onclick="verifierReponse(this, 'a')"> a) extremely</label>
                <label><input type="radio" name="q9" value="b" onclick="verifierReponse(this, 'a')"> b) hardly</label>
                <label><input type="radio" name="q9" value="c" onclick="verifierReponse(this, 'a')"> c) almost</label>
            </div>

            <!-- Question 10 -->
            <div class="question-box">Question 10</div>
            <div class="question">He is ___ ready for the exam. (presque)</div>
            <div class="options">
                <label><input type="radio" name="q10" value="a" onclick="verifierReponse(this, 'c')"> a) just</label>
                <label><input type="radio" name="q10" value="b" onclick="verifierReponse(this, 'c')"> b) very</label>
                <label><input type="radio" name="q10" value="c" onclick="verifierReponse(this, 'c')"> c) almost</label>
            </div>
            <!-- Résultat -->
            <div id="result" class="result"></div>
            <!-- Score circle -->
            <div id="scoreCircle" class="score-circle" style="display: none;"></div>
        </div>
    </div>

    <script>
        let correctAnswers = 0;
        let totalQuestions = 10;

        function verifierReponse(element, bonneReponse) {
            const userChoice = element.value;
            const parentLabel = element.parentElement;

            if (userChoice === bonneReponse) {
                parentLabel.classList.add('correct');
                correctAnswers++;
                ajouterCercleVert(parentLabel);
            } else {
                parentLabel.classList.add('incorrect');
                const correctOption = parentLabel.parentElement.querySelector(`input[value="${bonneReponse}"]`);
                correctOption.parentElement.classList.add('correct');
                ajouterCercleVert(correctOption.parentElement);
            }

            const options = parentLabel.parentElement.querySelectorAll('input');
            options.forEach(opt => opt.disabled = true);

            if (document.querySelectorAll('input:checked').length === totalQuestions) {
                afficherScore();
            }
        }

        function ajouterCercleVert(parentLabel) {
            const circle = document.createElement('span');
            circle.classList.add('circle');
            parentLabel.appendChild(circle);
        }

        function afficherScore() {
            let score = Math.round((correctAnswers / totalQuestions) * 100);
            const scoreCircle = document.getElementById('scoreCircle');
            const result = document.getElementById('result');

            scoreCircle.style.display = 'flex';
            scoreCircle.textContent = score + '%';

            if (score < 50) {
                scoreCircle.classList.add('low-score');
                result.textContent = "Score faible : essayez encore!";
            } else if (score >= 50 && score <= 80) {
                scoreCircle.classList.add('mid-score');
                result.textContent = "Score moyen : bien joué !";
            } else {
                scoreCircle.classList.add('high-score');
                result.textContent = "Excellent score ! Félicitations !";
            }

            result.style.display = 'block';
        }
    </script>
</body>
</html>> [questoions]</li>

    <li><strong>Code 3:</<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lecteur Audio Vertical</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #fFfFfF;
            padding: 10px;
        }
        .audio-container {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        .audio-player {
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: white;
            padding: 8px;
            border-radius: 12px;
            border: 1px solid pink;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            width: 150px;
        }
        .audio-player img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-bottom: 6px;
        }
        audio {
            width: 100%;
            height: 30px;
            -webkit-appearance: none;
            border: none;
            border-radius: 8px;
            background-color: #f3f3f3;
        }
        .control-buttons {
            display: flex;
            justify-content: space-between;
            width: 100%;
            margin-top: 3px;
        }
        button {
            padding: 2px 6px;
            background-color: pink;
            border: none;
            color: white;
            font-weight: bold;
            font-size: 10px;
            cursor: pointer;
            border-radius: 4px;
        }
        button:hover {
            background-color: #ff8ab0;
        }
    </style>
</head>
<body>
    <div class="audio-container">
        <!-- Premier lecteur audio avec image de Miranne -->
        <div class="audio-player">
            <img src="https://via.placeholder.com/50/FF69B4/FFFFFF?text=Monique" alt="Miranne">
            <audio id="audio1" controls>
                <source src="
https://feeds.soundcloud.com/stream/1863928806-perinemagne-lect28anglais-varieties-of-barbecue-sauce-c1"type="audio/mpeg">
                Votre navigateur ne supporte pas l'élément audio.
            </audio>
            <div class="control-buttons">
                <button onclick="changeSpeed('audio1', 0.75)">-</button>
                <button onclick="changeSpeed('audio1', 1.25)">+</button>
            </div>
        </div>

        <!-- Deuxième lecteur audio avec image de Paul -->
        <div class="audio-player">
            <img src="https://via.placeholder.com/50/1E90FF/FFFFFF?text=Emmanuel" alt="Paul">
            <audio id="audio2" controls>
                <source src="
https://feeds.soundcloud.com/stream/1863929352-perinemagne-lect28anglais-weather-c1h"type="audio/mpeg">
                Votre navigateur ne supporte pas l'élément audio.
            </audio>
            <div class="control-buttons">
                <button onclick="changeSpeed('audio2', 0.75)">-</button>
                <button onclick="changeSpeed('audio2', 1.25)">+</button>
            </div>
        </div>
    </div>

    <script>
        function changeSpeed(audioId, speed) {
            const audio = document.getElementById(audioId);
            audio.playbackRate = speed;
        }
    </script>
</body>
</html>> [audio]</li>
    
    <li><strong>Code 4:</<!DOCTYPE html> 
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dictée Interactive</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: flex-start;
            align-items: center;
            flex-direction: column;
            min-height: 100vh;
            background-color: #FB5AFB;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            width: 100%;
            text-align: center;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            display: flex;
            flex-direction: column;
            justify-content: flex-start;
            align-items: center;
        }
        h2 {
            font-size: 1.5em;
            margin-bottom: 10px;
        }
        textarea {
            width: 100%;
            font-size: 16px;
            margin-bottom: 10px;
            padding: 10px;
            border-radius: 5px;
            border: 1px solid #ddd;
            box-sizing: border-box;
            height: 120px;
        }
        .result-container {
            margin-top: 15px;
            padding: 15px;
            background-color: #fafafa;
            border-radius: 8px;
            border: 1px solid #ddd;
            text-align: left;
            width: 100%;
        }
        .missed {
            text-decoration: underline;
            color: black;
        }
        .incorrect {
            color: red;
            text-decoration: underline;
        }
        .fixed {
            color: #FB5AFB; /* Rose pour les corrections */
        }
        .correct {
            color: green;
        }
        button {
            margin-top: 10px;
            padding: 10px 20px;
            background-color: pink;
            color: white;
            font-weight: bold;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            width: 100%;
        }
        button:hover {
            background-color: #FF8AB0;
        }
        #score-circle {
            margin-top: 20px;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-weight: bold;
            font-size: 16px;
            color: white;
        }
        .red {
            background-color: red;
        }
        .pink {
            background-color: #FF8AB0;
        }
        .green {
            background-color: green;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Dictation</h2>
        <textarea id="userInput" rows="6" placeholder="Écrivez ici ce que vous entendez..."></textarea>
        <button id="submitBtn" onclick="corrigerDictee()" disabled>Soumettre</button>

        <div id="result" class="result-container"></div>
        <div id="score-circle" class="pink"></div>
    </div>

    <script>
        let texteCorrect = ""; // Initialement vide pour charger dynamiquement le texte correct

        // Fonction pour définir le texte de référence en fonction de la dictée choisie
        function setTexteCorrect(nouveauTexte) {
            texteCorrect = nouveauTexte;
            document.getElementById('result').innerHTML = ''; // Effacer les résultats précédents
            document.getElementById('userInput').value = ''; // Effacer la zone de saisie
            document.getElementById('score-circle').innerHTML = ''; // Effacer le score
            document.getElementById('submitBtn').disabled = true;
        }

        const submitBtn = document.getElementById('submitBtn');
        const userInput = document.getElementById('userInput');

        // Activer le bouton "Soumettre" si l'utilisateur a écrit au moins 10 mots
        userInput.addEventListener('input', () => {
            const wordCount = userInput.value.trim().split(/\s+/).length;
            submitBtn.disabled = wordCount < 10;
        });

        function corrigerDictee() {
            const userInputValue = userInput.value.trim();
            const userWords = userInputValue.split(/\s+/);
            const correctWords = texteCorrect.split(/\s+/);
            let correctCount = 0;
            let htmlResult = '';
            
            userWords.forEach((userWord) => {
                if (correctWords.includes(userWord)) {
                    htmlResult += `<span class="correct">${userWord}</span> `;
                    correctCount++;
                } else {
                    const correctWord = correctWords[userWords.indexOf(userWord)] || ''; 
                    htmlResult += `<span class="incorrect">${userWord}</span> <span class="fixed">(${correctWord})</span> `;
                }
            });

            // Afficher la correction complète en noir et souligné
            htmlResult += `<div class="missed">${texteCorrect}</div>`;

            const totalWords = correctWords.length;
            const score = Math.round((correctCount / totalWords) * 100);
            document.getElementById('result').innerHTML = htmlResult;

            const scoreCircle = document.getElementById('score-circle');
            scoreCircle.innerHTML = score;

            if (score < 50) {
                scoreCircle.className = "red";
            } else if (score < 75) {
                scoreCircle.className = "pink";
            } else {
                scoreCircle.className = "green";
            }

            submitBtn.disabled = true;
            userInput.disabled = true;
        }

        // Exemple : définir un texte en français (mais cela peut être remplacé par un texte dans toute autre langue)
        setTexteCorrect("Butterflies often flutter gracefully through the air, collecting nectar from colorful flowers to nourish themselves. They dance lightly over the flower meadows and spread a cheerful atmosphere in the summer. Their delicate wings shimmer in the sun and create a beautiful image in nature.");
    </script>
</body>
</html>> [Dictee]</li>
  </ul>
</section>
