
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
https://feeds.soundcloud.com/perinemagne/lect28anglais-varieties-of-barbecue-sauce-c1"type="audio/mpeg">
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

       
