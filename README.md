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

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-%23E34F26.svg?style=flat&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-%231572B6.svg?style=flat&logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=flat&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/License-MIT-green.svg" />
</p>

# 🏆 Items Earned Calculator

<div align="center">

A modern web tool to calculate how many items you can earn over a given duration. Enter a time, and see total items, rounded items, leftover seconds, and expected rare drop chances instantly.

</div>

---

## 🔹 Features

- **Flexible Time Input** – supports: d, h, m, s, and HH:MM:SS format  
- **Automatic Calculation** – 1 item per 10 seconds  
- **Results Display** – total seconds, exact items, full items, leftover seconds  
- **Drop Chances** – expected values for rare items (0.003% chance each)  
- **Interactive Examples** – click chips to auto-fill input  

---

## ⚡ Usage

1. Enter a duration (e.g., `10 h`, `1h 30m`, `540s`, `1:30:00`, `2 days 5 hours`)  
2. Click **Calculate** or press Enter  
3. Results will appear in tiles  
4. Use **Clear** to reset  
5. Click example chips to auto-fill input  

---

## 💻 Installation / Local Usage

1. Clone repo or download `index.html`  
2. Open in a browser  
3. Works offline – no server or dependencies required  

---

## 🛠️ Technologies

<div align="center">
  <img src="https://img.shields.io/badge/HTML5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black" />
</div>

---

## 📐 Formulas

```js
items = total_seconds / 10
itemsFloor = Math.floor(items)
leftover = total_seconds - (itemsFloor * 10)
expected = items * 0.00003
```
🌐 Live Demo
<div align="center"> [🔗 Try it Live](https://elecdeemtv.github.io/itemcalculator/) </div>

