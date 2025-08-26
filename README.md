# Items Earned Calculator

![HTML](https://img.shields.io/badge/HTML5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-%231572B6.svg?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=flat&logo=javascript&logoColor=black)

**Items Earned Calculator** is a simple web tool to calculate how many items you can earn over a given duration. The tool converts the user input into seconds, divides it by 10, and shows both the exact and rounded-down number of items you can earn.  

---

## Features

- Supports multiple time formats:
  - `d`, `day(s)` – days  
  - `h`, `hour(s)` – hours  
  - `m`, `minute(s)` – minutes  
  - `s`, `second(s)` – seconds  
  - `HH:MM:SS` – standard time format  
- Automatic item calculation: 1 item per 10 seconds  
- Displays:
  - Total seconds  
  - Exact items  
  - Rounded-down full items  
  - Leftover seconds  
- Expected rare drop chances:
  - Grandmaster Sprinkler – 0.003%  
  - Level Up Lollipop – 0.003%  
- Interactive example chips for quick calculations  

---

## Usage

1. Enter a duration in the input field, e.g.:  
   - `10 h`  
   - `1h 30m`  
   - `540s`  
   - `1:30:00`  
   - `2 days 5 hours`  
2. Click **Calculate** or press Enter.  
3. Results will appear in the tiles.  
4. Use **Clear** to reset.  
5. Click an example chip to auto-fill and calculate.  

---

## Installation / Local Usage

1. Download `index.html`.  
2. Open the file in your browser.  
3. Fully functional offline, no server needed.  

---

## Technologies

- **HTML5** – structure  
- **CSS3** – modern design with gradients and shadows  
- **JavaScript** – time parsing & item calculation logic  

---

## Formulas

```js
// Items earned
items = total_seconds / 10

// Full items
itemsFloor = Math.floor(items)

// Leftover seconds
leftover = total_seconds - (itemsFloor * 10)

// Expected drop (0.003% chance)
expected = items * 0.00003
