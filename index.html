<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ciclo Vitale</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: #f9f7f0;
            margin: 0;
            padding: 20px;
            background-image: radial-gradient(circle, #f0f8ff 20%, #e6f2ff 80%);
        }
        
        h1 {
            color: #4a7c59;
            margin-bottom: 15px;
            text-align: center;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
            font-size: 2.2em;
        }
        
        .instructions {
            margin-bottom: 25px;
            text-align: center;
            max-width: 650px;
            line-height: 1.6;
            background-color: rgba(255,255,255,0.8);
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .game-area {
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            margin-bottom: 20px;
        }
        
        .circle-container {
            position: relative;
            width: 550px;
            height: 550px;
            margin-bottom: 30px;
            background-color: rgba(255,255,255,0.3);
            border-radius: 50%;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
        }
        
        .center-text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 150px;
            text-align: center;
            z-index: 1;
            font-weight: bold;
            color: #4a7c59;
            font-size: 1.3em;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
            padding: 10px;
            background-color: rgba(255,255,255,0.7);
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        
        .section {
            position: absolute;
            width: 90px;
            height: 90px;
            background-color: #c8e6c9;
            border: 3px solid #4a7c59;
            border-radius: 50%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            font-size: 13px;
            cursor: pointer;
            transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
            z-index: 2;
            box-shadow: 0 3px 6px rgba(0,0,0,0.1);
        }
        
        .section-number {
            font-weight: bold;
            color: #2e7d32;
            margin-bottom: 3px;
            font-size: 15px;
            text-shadow: 0 1px 1px rgba(0,0,0,0.1);
        }
        
        .section.highlight {
            background-color: #ffcdd2;
            transform: scale(1.1);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .section.correct {
            background-color: #a5d6a7;
            box-shadow: 0 0 15px rgba(46, 125, 50, 0.5);
            animation: pulse 1.5s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }
        
        .word-container {
            position: relative;
            width: 100%;
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        
        .section-word {
            font-size: 12px;
            color: #1b5e20;
            font-weight: 500;
            max-width: 80%;
            word-wrap: break-word;
        }
        
        .words-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            width: 600px;
            margin-top: 20px;
            padding: 20px;
            background-color: rgba(255,255,255,0.7);
            border-radius: 15px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }
        
        .word {
            padding: 10px 15px;
            background-color: #d1c4e9;
            border: 2px solid #7e57c2;
            border-radius: 8px;
            cursor: move;
            user-select: none;
            transition: all 0.2s;
            font-weight: 500;
            color: #4527a0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .word:hover {
            background-color: #b39ddb;
            transform: translateY(-3px);
            box-shadow: 0 4px 8px rgba(0,0,0,0.15);
        }
        
        .word.dragging {
            opacity: 0.7;
            transform: scale(0.95);
            box-shadow: 0 0 10px rgba(126, 87, 194, 0.5);
        }
        
        .feedback {
            margin-top: 25px;
            padding: 18px 30px;
            border-radius: 10px;
            font-weight: bold;
            text-align: center;
            opacity: 0;
            transition: opacity 0.4s, transform 0.4s;
            max-width: 80%;
            transform: translateY(20px);
            font-size: 1.1em;
        }
        
        .feedback.show {
            opacity: 1;
            transform: translateY(0);
        }
        
        .positive {
            background-color: #c8e6c9;
            color: #1b5e20;
            border: 2px solid #4caf50;
            box-shadow: 0 3px 10px rgba(76, 175, 80, 0.3);
        }
        
        .negative {
            background-color: #ffcdd2;
            color: #c62828;
            border: 2px solid #f44336;
            box-shadow: 0 3px 10px rgba(244, 67, 54, 0.3);
        }
        
        .reset-btn {
            margin-top: 25px;
            padding: 14px 28px;
            background-color: #4a7c59;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 16px;
            transition: all 0.3s;
            font-weight: bold;
            letter-spacing: 0.5px;
            box-shadow: 0 3px 6px rgba(0,0,0,0.1);
        }
        
        .reset-btn:hover {
            background-color: #3a6a49;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .reset-btn:active {
            transform: translateY(1px);
        }
        
        svg.arrow-path {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 0;
        }
        
        .progress-container {
            width: 80%;
            max-width: 400px;
            height: 10px;
            background-color: #e0e0e0;
            border-radius: 5px;
            margin-top: 15px;
            overflow: hidden;
        }
        
        .progress-bar {
            height: 100%;
            background-color: #4a7c59;
            width: 0%;
            transition: width 0.5s;
        }
    </style>
</head>
<body>
    <h1>Ciclo Vitale</h1>
    <div class="instructions">
        <p>Trascina le parole nelle sezioni numerate per ricostruire il ciclo vitale corretto.</p>
        
    </div>
    
    <div class="game-area">
        <div class="circle-container" id="circleContainer">
            <div class="center-text">OGNI ESSERE VIVENTE</div>
            <svg class="arrow-path" id="arrowsSvg"></svg>
            <!-- Le sezioni verranno create dinamicamente -->
        </div>
        
        <div class="words-container" id="wordsContainer">
            <!-- Le parole verranno create dinamicamente -->
        </div>
    </div>
    
    <div class="progress-container">
        <div class="progress-bar" id="progressBar"></div>
    </div>
    
    <div class="feedback" id="feedback"></div>
    <button class="reset-btn" id="resetBtn">Ricomincia</button>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const circleContainer = document.getElementById('circleContainer');
            const arrowsSvg = document.getElementById('arrowsSvg');
            const wordsContainer = document.getElementById('wordsContainer');
            const feedback = document.getElementById('feedback');
            const resetBtn = document.getElementById('resetBtn');
            const progressBar = document.getElementById('progressBar');
            
            const correctOrder = ['nasce', 'si nutre', 'cresce', 'si muove', 'si riproduce', 'muore'];
            let words = [...correctOrder].sort(() => Math.random() - 0.5);
            
            let draggedWord = null;
            let placedWords = Array(6).fill(null);
            let sections = [];
            
            // Crea le sezioni disposte in cerchio con numerazione
            function createSections() {
                const radius = 200;
                const centerX = 275;
                const centerY = 275;
                const angleStep = (2 * Math.PI) / 6;
                
                // Pulisci il container
                while (circleContainer.firstChild) {
                    if (!circleContainer.firstChild.classList || 
                        (!circleContainer.firstChild.classList.contains('center-text') && 
                         !circleContainer.firstChild.classList.contains('arrow-path'))) {
                        circleContainer.removeChild(circleContainer.firstChild);
                    } else {
                        break;
                    }
                }
                
                sections = [];
                
                for (let i = 0; i < 6; i++) {
                    const section = document.createElement('div');
                    section.className = 'section';
                    section.dataset.index = i;
                    section.dataset.correctWord = correctOrder[i];
                    
                    const wordContainer = document.createElement('div');
                    wordContainer.className = 'word-container';
                    
                    // Aggiungi numero della sezione
                    const number = document.createElement('div');
                    number.className = 'section-number';
                    number.textContent = (i + 1) + '.';
                    wordContainer.appendChild(number);
                    
                    section.appendChild(wordContainer);
                    
                    const angle = i * angleStep - Math.PI / 2; // Inizia dall'alto
                    const x = centerX + radius * Math.cos(angle);
                    const y = centerY + radius * Math.sin(angle);
                    
                    section.style.left = `${x - 45}px`;
                    section.style.top = `${y - 45}px`;
                    
                    section.addEventListener('dragover', dragOver);
                    section.addEventListener('dragenter', dragEnter);
                    section.addEventListener('dragleave', dragLeave);
                    section.addEventListener('drop', drop);
                    
                    circleContainer.appendChild(section);
                    sections.push({
                        element: section,
                        x: x,
                        y: y,
                        wordContainer: wordContainer
                    });
                }
                
                drawArrows();
                updateProgress();
            }
            
            // Disegna le frecce curve tra le sezioni
            function drawArrows() {
                // Pulisci le frecce esistenti
                arrowsSvg.innerHTML = '';
                
                for (let i = 0; i < sections.length; i++) {
                    const nextIdx = (i + 1) % sections.length;
                    const start = sections[i];
                    const end = sections[nextIdx];
                    
                    // Calcola punti di controllo per la curva
                    const centerX = 275;
                    const centerY = 275;
                    const controlRadius = 240;
                    const controlAngle = (i * (2 * Math.PI / 6) - Math.PI / 2 + (Math.PI / 6));
                    
                    const controlX = centerX + controlRadius * Math.cos(controlAngle);
                    const controlY = centerY + controlRadius * Math.sin(controlAngle);
                    
                    // Crea il percorso curvo
                    const path = document.createElementNS('http://www.w3.org/2000/svg', 'path');
                    path.setAttribute('d', `M ${start.x} ${start.y} Q ${controlX} ${controlY} ${end.x} ${end.y}`);
                    path.setAttribute('stroke', '#4a7c59');
                    path.setAttribute('stroke-width', '3');
                    path.setAttribute('fill', 'none');
                    path.setAttribute('marker-end', 'url(#arrowhead)');
                    path.setAttribute('opacity', '0.7');
                    
                    arrowsSvg.appendChild(path);
                }
                
                // Aggiungi la definizione della punta della freccia
                const defs = document.createElementNS('http://www.w3.org/2000/svg', 'defs');
                const marker = document.createElementNS('http://www.w3.org/2000/svg', 'marker');
                marker.setAttribute('id', 'arrowhead');
                marker.setAttribute('markerWidth', '10');
                marker.setAttribute('markerHeight', '7');
                marker.setAttribute('refX', '9');
                marker.setAttribute('refY', '3.5');
                marker.setAttribute('orient', 'auto');
                
                const arrow = document.createElementNS('http://www.w3.org/2000/svg', 'polygon');
                arrow.setAttribute('points', '0 0, 10 3.5, 0 7');
                arrow.setAttribute('fill', '#4a7c59');
                
                marker.appendChild(arrow);
                defs.appendChild(marker);
                arrowsSvg.appendChild(defs);
            }
            
            // Crea le parole nel contenitore sotto il cerchio
            function createWords() {
                wordsContainer.innerHTML = '';
                
                words.forEach(word => {
                    const wordElement = document.createElement('div');
                    wordElement.className = 'word';
                    wordElement.textContent = word;
                    wordElement.draggable = true;
                    wordElement.dataset.word = word;
                    
                    wordElement.addEventListener('dragstart', dragStart);
                    wordElement.addEventListener('dragend', dragEnd);
                    
                    wordsContainer.appendChild(wordElement);
                });
            }
            
            // Funzioni per il drag and drop
            function dragStart(e) {
                draggedWord = e.target;
                e.target.classList.add('dragging');
                e.dataTransfer.setData('text/plain', e.target.dataset.word);
                e.dataTransfer.effectAllowed = 'move';
            }
            
            function dragEnd(e) {
                e.target.classList.remove('dragging');
            }
            
            function dragOver(e) {
                e.preventDefault();
                e.dataTransfer.dropEffect = 'move';
            }
            
            function dragEnter(e) {
                e.preventDefault();
                let section = e.target;
                while (section && !section.classList.contains('section')) {
                    section = section.parentElement;
                }
                
                if (section) {
                    section.classList.add('highlight');
                }
            }
            
            function dragLeave(e) {
                let section = e.target;
                while (section && !section.classList.contains('section')) {
                    section = section.parentElement;
                }
                
                if (section) {
                    section.classList.remove('highlight');
                }
            }
            
            function drop(e) {
                e.preventDefault();
                
                // Trova l'elemento sezione
                let section = e.target;
                while (section && !section.classList.contains('section')) {
                    section = section.parentElement;
                }
                
                if (!section) return;
                
                section.classList.remove('highlight');
                
                const sectionIndex = parseInt(section.dataset.index);
                const word = e.dataTransfer.getData('text/plain');
                
                // Se la sezione è già occupata (oltre al numero), non fare nulla
                const wordContainer = section.querySelector('.word-container');
                if (wordContainer.children.length > 1) return;
                
                // Posiziona la parola nella sezione
                const wordElement = document.createElement('div');
                wordElement.className = 'section-word';
                wordElement.textContent = word;
                wordContainer.appendChild(wordElement);
                
                placedWords[sectionIndex] = word;
                draggedWord.style.display = 'none';
                
                // Controlla l'ordine
                checkOrder();
                updateProgress();
            }
            
            // Aggiorna la barra di progresso
            function updateProgress() {
                const placedCount = placedWords.filter(word => word !== null).length;
                const progress = (placedCount / 6) * 100;
                progressBar.style.width = `${progress}%`;
            }
            
            // Controlla se l'ordine è corretto
            function checkOrder() {
                // Rimuovi i valori null dall'array
                const currentWords = placedWords.filter(word => word !== null);
                
                // Se tutte le parole sono state piazzate
                if (currentWords.length === 6) {
                    let isCorrect = true;
                    
                    for (let i = 0; i < 6; i++) {
                        if (currentWords[i] !== correctOrder[i]) {
                            isCorrect = false;
                            break;
                        }
                    }
                    
                    if (isCorrect) {
                        showFeedback('Fantastico! Hai ricostruito correttamente il ciclo vitale!', 'positive');
                        
                        // Evidenzia le sezioni
                        document.querySelectorAll('.section').forEach(section => {
                            section.classList.add('correct');
                        });
                    } else {
                        showFeedback('Attenzione! Alcune fasi non sono nell\'ordine corretto.', 'negative');
                        
                        // Riporta le parole nel contenitore dopo un breve ritardo
                        setTimeout(() => {
                            resetWords();
                        }, 1500);
                    }
                }
            }
            
            function showFeedback(message, type) {
                feedback.textContent = message;
                feedback.className = 'feedback';
                feedback.classList.add(type, 'show');
                
                // Nascondi il feedback dopo 3 secondi se è negativo
                if (type === 'negative') {
                    setTimeout(() => {
                        feedback.classList.remove('show');
                    }, 3000);
                }
            }
            
            // Riporta le parole nel contenitore
            function resetWords() {
                placedWords = Array(6).fill(null);
                
                // Ripristina le parole
                Array.from(wordsContainer.children).forEach(word => {
                    word.style.display = 'block';
                });
                
                // Svuota le sezioni (mantenendo solo i numeri)
                document.querySelectorAll('.word-container').forEach(container => {
                    // Rimuovi tutti i figli tranne il numero
                    while (container.children.length > 1) {
                        container.removeChild(container.lastChild);
                    }
                });
                
                document.querySelectorAll('.section').forEach(section => {
                    section.classList.remove('correct', 'highlight');
                });
                
                feedback.classList.remove('show', 'positive', 'negative');
                updateProgress();
            }
            
            // Resetta tutto il gioco
            function resetGame() {
                // Mescola le parole
                words = [...correctOrder].sort(() => Math.random() - 0.5);
                resetWords();
                createSections();
                createWords();
            }
            
            resetBtn.addEventListener('click', resetGame);
            
            // Inizializza il gioco
            createSections();
            createWords();
        });
    </script>
</body>
</html>
