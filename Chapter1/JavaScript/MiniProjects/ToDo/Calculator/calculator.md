🧮 Mini Project: Calculator (Step-by-Step)
🎯 Objective

Build a working calculator:

Display numbers
Perform operations (+, -, *, /)
Show result
🟢 Step 1: UI (Start Simple)
📄 HTML
<input type="text" id="display" disabled>

<br><br>

<button>1</button>
<button>2</button>
<button>3</button>
<button>+</button>

<br>

<button>4</button>
<button>5</button>
<button>6</button>
<button>-</button>

<br>

<button>7</button>
<button>8</button>
<button>9</button>
<button>*</button>

<br>

<button>0</button>
<button>C</button>
<button>=</button>
<button>/</button>

🟡 Step 2: Basic Functionality
🎯 Task 1:

👉 When number button clicked → show in display

🧠 Hint:
Use querySelectorAll("button")
Add event to each button
Append value
🔧 Example logic:
display.value += button.innerText;
🟠 Step 3: Clear Button

🎯 Task 2:

👉 When C clicked:

display.value = "";
🔴 Step 4: Calculate Result

🎯 Task 3:

👉 When = clicked:

Evaluate expression
⚠️ Simple way (for now):
display.value = eval(display.value);

👉 Yes, eval is not recommended in real apps — but fine for learning

🧠 Full Logic Flow
Button	Action
Number	append
Operator	append
C	clear
=	evaluate
🔥 Example Core JS Structure
let display = document.getElementById('display');
let buttons = document.querySelectorAll('button');

buttons.forEach(function(button){
    button.addEventListener('click', function(){

        let value = button.innerText;

        if(value === "C"){
            display.value = "";
        }
        else if(value === "="){
            display.value = eval(display.value);
        }
        else{
            display.value += value;
        }

    });
});

🟡 Step 5: Edge Cases (IMPORTANT)

Try handling:

++ (invalid input)
divide by zero
empty input
🔥 Bonus Upgrades

If you want to level up:

✅ 1. Backspace button
⌫
✅ 2. Keyboard input support
✅ 3. Styling (grid layout)

🧠 What This Project Teaches
Skill	Why it matters
Event delegation	many buttons
State handling	display value
Condition branching	button types
String evaluation	expressions