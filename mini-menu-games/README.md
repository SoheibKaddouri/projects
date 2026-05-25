# Mini Menu Games Platform

A lightweight, dependency-free single-page web application featuring isolated mathematical engine and game state environments: an arbitrary-precision Factorial Calculator and an interactive Number Guessing Game. The architecture relies completely on native web standards to deliver high-performance client-side logic.

## 🛠️ Tech Stack & Focus Areas
* **Frontend Core:** Semantic HTML5 / Modular CSS3 / Vanilla JavaScript (ES6+)
* **Engineering Standards:** Arbitrary-Precision Arithmetic ($BigInt$), Client-Side State Isolation, Robust Input Validation

## 📈 Core Business Value & Engineering Impact
* **Arbitrary-Precision Computation:** Utilizes JavaScript's native `BigInt` primitives to calculate factorials beyond $20!$ (up to $100!$). This bypasses standard IEEE 754 floating-point limitations, preventing numerical overflow and ensuring absolute precision for massive calculations.
* **Zero-Dependency Architecture:** Eliminates third-party overhead and vulnerabilities by implementing pure vanilla modules, resulting in near-instant layout rendering and negligible asset weight.
* **Defensive Input Handling:** Features rigorous boundary checks and real-time input sanitization to catch negative numbers, empty states, and upper limit breaks before execution blocks can crash.

## 📁 Platform Architecture Breakdown
The application is decoupled into independent user modules:
1. **Central Dashboard:** A clean navigation UI allowing seamless hot-swapping between the active utility engines without full page reloads.
2. **Factorial Computational Engine:** A dedicated computational loop optimized to scale large integer allocations safely within the browser call stack.
3. **Stateful Guessing Simulator:** A randomized game tracking environment running automated state resets, precise attempt counters, and intuitive high/low evaluation indicators.

## 🌐 Live Interactive Demo
* To see the application code structure and frontend execution assets in real-time within an interactive repository environment, check out the project codebase here: **[Mini Menu Games Code Repository](https://github.com/SoheibKaddouri/mini-menu-games)**
