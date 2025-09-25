<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Retro Calculator with History</title>
<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@700&family=Bungee&display=swap" rel="stylesheet">
<style>
  body {
    display: flex;
    justify-content: center;
    padding: 20px;
    font-family: 'Courier New', Courier, monospace;
    background: #111;
    color: #fff;
  }

  .calculator-wrapper {
    display: flex;
    align-items: flex-start;
    gap: 20px;
  }

  .calculator-box {
    display: flex;
    flex-direction: column;
  }

  /* Heading shifted 1cm to the right */
  h1 {
    font-family: 'Bungee', cursive;
    font-size: 3rem;
    margin: 0 0 20px 0;
    padding-left: 1cm; /* Moves heading 1 cm to the right */
    color: #fff;
    text-align: left;
    text-shadow: none;
  }

  .calculator {
    border-radius: 12px;
    width: 360px;
    padding: 20px;
    transition: all 0.3s ease;
  }
  .display {
    font-size: 2rem;
    text-align: right;
    padding: 15px;
    margin-bottom: 20px;
    overflow-x: auto;
    white-space: nowrap;
  }
  .buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
  }
  .bottom-row {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
    margin-top: 10px;
  }
  button {
    padding: 15px;
    font-size: 1.2rem;
    cursor: pointer;
    border-radius: 6px;
    border: 1px solid;
    transition: all 0.2s ease;
  }
  button:hover { opacity: 0.9; }
  button:active { transform: scale(0.95); }

  .side-panel {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-top: 60px;
  }

  #themeSelector, #clearHistory {
    padding: 10px;
    font-size: 1rem;
    border-radius: 6px;
    cursor: pointer;
  }

  /* Themes */
  body.light { background: #b0b0b0; color: #000; }
  body.light .calculator { background: #d3d3d3; border: 3px solid #7a7a7a; box-shadow: 0 0 10px #888; }
  body.light .display { background: #222; color: #fff; border: 2px inset #555; }
  body.light button { background: #f0f0f0; border-color: #666; color: #000; }
  body.light button.operator { background: orange; color: #fff; }
  body.light #clear { background: red; color: white; }
  body.light #backspace { background: #5c6ac4; color: white; }
  body.light #history { background: #4caf50; color: white; }
  body.light #equals { background: black; color: white; font-weight: bold; }

  body.dark { background: linear-gradient(135deg, #0f0f0f, #1a1a2e); color: #fff; }
  body.dark .calculator { background: #111; border: 3px solid #00ffcc; box-shadow: 0 0 20px #00ffcc; }
  body.dark .display { background: #000; color: #0ff; border: 2px inset #00ffcc; text-shadow: 0 0 8px #0ff, 0 0 12px #0ff; }
  body.dark button { background: #1a1a2e; border-color: #00ffcc; color: #fff; box-shadow: 0 0 8px #00ffcc inset; }
  body.dark button.operator { background: #ff007f; border-color: #ff66b2; }
  body.dark #clear { background: #e60000; border-color: #ff3333; }
  body.dark #backspace { background: #5c6ac4; border-color: #8892ff; }
  body.dark #history { background: #00cc44; border-color: #33ff77; }
  body.dark #equals { background: #222; color: #0ff; font-weight: bold; border-color: #00ffcc; }
  body.dark #clearHistory { background: crimson; color: white; }

  body.lcd { background: #444; color: #000; }
  body.lcd .calculator { background: #d6d1a6; border: 3px solid #333; box-shadow: 0 0 10px #666; }
  body.lcd .display { background: #b4c292; color: #1a2; border: 2px inset #333; font-family: "Digital-7", monospace; text-shadow: 0 0 3px #0f0; }
  body.lcd button { background: #e2dfc7; border-color: #333; color: #000; font-weight: bold; }
  body.lcd button.operator { background: #c9c490; }
  body.lcd #clear { background: #d9534f; color: white; }
  body.lcd #backspace { background: #337ab7; color: white; }
  body.lcd #history { background: #5cb85c; color: white; }
  body.lcd #equals { background: #222; color: #0f0; font-weight: bold; }
  body.lcd #clearHistory { background: crimson; color: white; }

  #historyPanel { display: none; border-radius: 6px; padding: 10px; width: 180px; }
  #historyList { max-height: 300px; overflow-y: auto; font-size: 1rem; }
  #historyList div { border-bottom: 1px dotted #444; padding: 4px 0; cursor: pointer; }
  #historyList div:hover { background: rgba(255,255,255,0.1); }
</style>
</head>
<body class="dark">
  <div class="calculator-wrapper">
    <div class="calculator-box">
      <h1>CALCULATOR</h1>
      <div class="calculator">
        <div class="display" id="display">0</div>
        
        <div class="buttons">
          <button>(</button><button>)</button><button class="operator">/</button><button class="operator">*</button>
          <button>7</button><button>8</button><button>9</button><button class="operator">-</button>
          <button>4</button><button>5</button><button>6</button><button class="operator">+</button>
          <button>1</button><button>2</button><button>3</button><button>0</button>
          <!-- Advanced functions -->
          <button class="func">√</button>
          <button class="func">x²</button>
          <button class="func">x³</button>
          <button class="func">exp</button>
          <button class="func">sin</button>
          <button class="func">cos</button>
          <button class="func">tan</button>
          <button class="func">log</button>
        </div>

        <div class="bottom-row">
          <button id="clear">C</button>
          <button id="backspace">Del</button>
          <button id="equals">=</button>
          <button id="history">History</button>
        </div>
      </div>
    </div>

    <div class="side-panel">
      <button id="clearHistory">Clear History</button>
      <select id="themeSelector">
        <option value="dark">Neon Dark</option>
        <option value="light">Light</option>
        <option value="lcd">Retro LCD</option>
      </select>
      <div id="historyPanel">
        <div id="historyList"></div>
      </div>
    </div>
  </div>

<script>
const display = document.getElementById("display");
const historyPanel = document.getElementById("historyPanel");
const historyList = document.getElementById("historyList");
const themeSelector = document.getElementById("themeSelector");
const clearHistoryBtn = document.getElementById("clearHistory");
let currentInput = "";
let history = JSON.parse(localStorage.getItem("calcHistory")) || [];

function setDisplay(value) { display.textContent = value || "0"; }

function updateHistory() {
  historyList.innerHTML = history.map((item, i) =>
    `<div class="history-item" data-index="${i}">${item}</div>`).join('');
  document.querySelectorAll(".history-item").forEach(el => {
    el.addEventListener("click", () => {
      const expr = history[el.dataset.index].split(" = ")[0];
      currentInput = expr;
      setDisplay(currentInput);
    });
  });
  localStorage.setItem("calcHistory", JSON.stringify(history));
}

const operators = ['+', '-', '*', '/'];

document.querySelectorAll("button").forEach(btn => {
  btn.addEventListener("click", () => {
    const value = btn.textContent;
    if (btn.id === "clear") { currentInput=""; setDisplay("0"); }
    else if (btn.id === "backspace") { currentInput=currentInput.slice(0,-1); setDisplay(currentInput); }
    else if (btn.id === "equals") {
      try {
        let expr = currentInput.replace(/√/g,"Math.sqrt").replace(/x²/g,"**2").replace(/x³/g,"**3")
          .replace(/sin/g,"Math.sin").replace(/cos/g,"Math.cos").replace(/tan/g,"Math.tan")
          .replace(/log/g,"Math.log").replace(/exp/g,"Math.exp");
        let result = Function(`"use strict";return (${expr})`)();
        if(typeof result==='number' && !Number.isInteger(result)) result=parseFloat(result.toFixed(6));
        history.push(`${currentInput} = ${result}`);
        currentInput = result.toString(); setDisplay(currentInput); updateHistory();
      } catch { currentInput=""; setDisplay("Error"); }
    } else if (btn.id==="history") { historyPanel.style.display = historyPanel.style.display==="none"?"block":"none"; updateHistory(); }
    else if (btn.id==="clearHistory") { history=[]; updateHistory(); localStorage.removeItem("calcHistory"); }
    else if (operators.includes(value)) { if (!operators.includes(currentInput.slice(-1)) && currentInput!=="") { currentInput+=value; setDisplay(currentInput); } }
    else if (value===".") { const last = currentInput.split(/[\+\-\*\/]/).pop(); if(!last.includes(".")) { currentInput+=value; setDisplay(currentInput); } }
    else if (btn.classList.contains("func")) { currentInput+=value==="√"?"√(":value+"("; setDisplay(currentInput); }
    else if (btn.id!=="themeSelector") { currentInput+=value; setDisplay(currentInput); }
  });
});

themeSelector.addEventListener("change", () => { document.body.className = themeSelector.value; localStorage.setItem("theme", themeSelector.value); });
const savedTheme = localStorage.getItem("theme") || "dark";
document.body.className = savedTheme;
themeSelector.value = savedTheme;
updateHistory();

document.addEventListener("keydown", e => {
  if ((/\d/).test(e.key) || operators.includes(e.key) || e.key==="." || e.key==="("|| e.key===")") { currentInput+=e.key; setDisplay(currentInput); }
  else if(e.key==="Enter") document.getElementById("equals").click();
  else if(e.key==="Backspace") document.getElementById("backspace").click();
  else if(e.key.toLowerCase()==="c") document.getElementById("clear").click();
  else if(e.key.toLowerCase()==="h") document.getElementById("history").click();
});
</script>
</body>
</html>
