# Project---Standard-Calculator
## js:
```
let display = document.getElementById('result');

function appendCharacter(character) {
    display.innerText += character;
}

function clearDisplay() {
    display.innerText = '';
}

function deleteLast() {
    display.innerText = display.innerText.slice(0, -1);
}

function calculateResult() {
    try {
        display.innerText = eval(display.innerText);
    } catch {
        display.innerText = 'Error';
    }
}
```
## html:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
    <div class="container">
        <div class="calculator">
            <div class="display">
                <div id="result"></div>
            </div>
            <div class="buttons">
                <button onclick="clearDisplay()">AC</button>
                <button onclick="deleteLast()">DEL</button>
                <button onclick="appendCharacter('/')">/</button>
                <button onclick="appendCharacter('')"></button>
                <button onclick="appendCharacter('7')">7</button>
                <button onclick="appendCharacter('8')">8</button>
                <button onclick="appendCharacter('9')">9</button>
                <button onclick="appendCharacter('-')">-</button>
                <button onclick="appendCharacter('4')">4</button>
                <button onclick="appendCharacter('5')">5</button>
                <button onclick="appendCharacter('6')">6</button>
                <button onclick="appendCharacter('+')">+</button>
                <button onclick="appendCharacter('1')">1</button>
                <button onclick="appendCharacter('2')">2</button>
                <button onclick="appendCharacter('3')">3</button>
                <button onclick="calculateResult()">=</button>
                <button onclick="appendCharacter('0')">0</button>
                <button onclick="appendCharacter('%')">%</button>
                <button onclick="appendCharacter('.')">.</button>
            </div><BR></BR>
            <div class="name">PRAGATHEESVARAN <ABbr></ABbr></div>
            <div class="id">212221240039</div>
        </div>
    </div>
    <script src="index.js"></script>
</body>
</html>
```
## css:
```
body {
    margin: 0;
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-image: url(download.jpg);
    background-size: cover;
}

.container {
    display: flex;
    justify-content: center;
    align-items: center;
}

.calculator {
    background-color: #fa6f6f;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
    text-align: center;
}

.display {
    margin-bottom: 20px;
}

.display .name {
    font-size: 1.2em;
    font-weight: bold;
}

.display .id {
    font-size: 1em;
    margin-bottom: 10px;
}

#result {
    font-size: 1.5em;
    margin-bottom: 20px;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

button {
    padding: 20px;
    font-size: 1.2em;
    border: none;
    border-radius: 5px;
    background-color: #ed4747;
    color: white;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
    cursor: pointer;
    transition: background-color 0.3s;
}

button:hover {
    background-color: #e34e4e;
}
```
## output:
![image](https://github.com/praga-16/Project---Standard-Calculator/assets/95266924/f4b7b200-62df-44cb-afa5-cfaf6a0c39ca)
![image](https://github.com/praga-16/Project---Standard-Calculator/assets/95266924/540bac33-ccb9-491f-83e9-626602313874)

