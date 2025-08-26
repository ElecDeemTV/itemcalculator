---
title: "Items Earned Calculator"
description: "A modern web tool to calculate how many items you can earn over a given duration."
author: "ElecDeemTV"
date: 2025-08-26
tags: [calculator, items, web-tool, JavaScript, HTML, CSS]
license: MIT
live_demo: "https://elecdeemtv.github.io/itemcalculator/"
screenshot: "./screenshot.png"
badges:
  - "HTML: https://img.shields.io/badge/HTML5-%23E34F26.svg?style=flat&logo=html5&logoColor=white"
  - "CSS: https://img.shields.io/badge/CSS3-%231572B6.svg?style=flat&logo=css3&logoColor=white"
  - "JavaScript: https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=flat&logo=javascript&logoColor=black"
  - "License: https://img.shields.io/badge/License-MIT-green.svg"
---

# 🏆 Items Earned Calculator

![HTML](https://img.shields.io/badge/HTML5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-%231572B6.svg?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=flat&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green.svg)

A modern web tool to calculate how many items you can earn over a given duration. Enter a time, and see total items, rounded items, leftover seconds, and expected rare drop chances instantly.  

---

## 🔹 Features

- **Flexible Time Input** – supports:
  - `d`, `day(s)` – days  
  - `h`, `hour(s)` – hours  
  - `m`, `minute(s)` – minutes  
  - `s`, `second(s)` – seconds  
  - `HH:MM:SS` – standard time format  
- **Automatic Calculation** – 1 item per 10 seconds.  
- **Results Display** – shows:
  - Total seconds  
  - Exact items  
  - Rounded-down full items  
  - Leftover seconds  
- **Drop Chances** – expected values for rare items:
  - Grandmaster Sprinkler – 0.003%  
  - Level Up Lollipop – 0.003%  
- **Interactive Examples** – click example chips to auto-fill input.  

---

## ⚡ Usage

1. Enter a duration in the input field, for example:  
2. Click **Calculate** or press Enter.  
3. Results will appear in the corresponding tiles.  
4. Use **Clear** to reset inputs and outputs.  
5. Click on an example chip to automatically fill the input and calculate.  

---

## 💻 Installation / Local Usage

1. Clone the repository or download `index.html`.  
2. Open the file in your preferred web browser.  
3. Fully functional offline – no server or dependencies required.  

---

## 🛠️ Technologies

- **HTML5** – page structure  
- **CSS3** – modern gradients, shadows, and hover effects  
- **JavaScript** – parsing time input and calculating items dynamically  

---

## 📐 Formulas

```js
// Items earned
items = total_seconds / 10

// Full items (rounded down)
itemsFloor = Math.floor(items)

// Leftover seconds
leftover = total_seconds - (itemsFloor * 10)

// Expected rare drop (0.003%)
expected = items * 0.00003
