# 🧮 Math Quiz Game — C++ Console Game

![C++](https://img.shields.io/badge/Language-C%2B%2B-blue?style=flat-square&logo=cplusplus)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey?style=flat-square&logo=windows)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

A console-based **Math Quiz Game** written in C++ that challenges the player with arithmetic questions across multiple difficulty levels and operation types. Track your score and see if you **Pass** or **Fail**!

---

## 📸 Preview

```
Question [1/5]

47
23 +
___________________
70
Correct Answer :-)

Question [2/5]

85
61 -
___________________
20
Wrong Answer :-(
Correct answer is : 24

_______________________________________

 Final Result is Pass :-)
_______________________________________

Number Of Questions    : 5
Questions Level        : Med
OpType                 : +
Number Of Right Answer : 3
Number Of Wrong Answer : 2
_______________________________________
```

---

## ✨ Features

- 🔢 **4 difficulty levels** — Easy (1–10), Medium (10–50), Hard (50–100), or Mix
- ➕➖✖️➗ **5 operation types** — Add, Subtract, Multiply, Divide, or Mix
- 🎯 **Custom quiz length** — choose between 1 and 10 questions
- ✅ **Instant feedback** — right or wrong shown after each answer with the correct solution
- 🎨 **Dynamic console colors** — green for correct, red for wrong
- 📊 **Final scoreboard** — full summary with pass/fail result
- 🔁 **Play again option** — replay without restarting the terminal
- ✔️ **Input validation** — no crashes from invalid input

---

## 🗂️ Project Structure

```
Math-Quiz-Game/
│
├── main.cpp       # Full game source code
└── README.md      # Project documentation
```

---

## 🧱 Code Architecture

The project uses **structured programming** with enums and structs for clean, readable logic:

| Component | Type | Description |
|---|---|---|
| `enQuestionLevel` | `enum` | Easy, Med, Hard, or Mix difficulty |
| `enOperationType` | `enum` | Add, Sub, Mul, Div, or MixOp |
| `stQuestion` | `struct` | Holds numbers, operation, correct answer, player answer, and result |
| `stQuizz` | `struct` | Holds all questions, score counters, level, op type, and pass/fail status |

### Key Functions

| Function | Description |
|---|---|
| `ReadHowManyQuestions()` | Validates and returns number of questions (1–10) |
| `ReadQuestionsLevel()` | Reads and validates difficulty level |
| `ReadOperationType()` | Reads and validates operation type |
| `GenerateQuestion()` | Creates a random question based on level and operation |
| `GenerateQuizzQuestions()` | Fills the quiz with generated questions |
| `SimpleCalculator()` | Computes the correct answer for any operation |
| `AskAndCorrectQuestionList()` | Displays questions, reads answers, and corrects them |
| `CorrectTheQuestionAnswer()` | Checks player answer and updates score counters |
| `PrintQuizzResult()` | Shows final summary with pass/fail verdict |
| `setColorBackground()` | Changes console color based on answer result |
| `PlayMathGame()` | Orchestrates a full quiz session |
| `StartGame()` | Entry point — handles play-again loop |

---

## 🚀 Getting Started

### Prerequisites

- A C++ compiler (e.g. **g++**, **MSVC**, **MinGW**)
- Windows OS *(uses `system("color")` and `system("cls")` — Windows only)*

### Compile & Run

**Using g++ (MinGW / terminal):**
```bash
g++ main.cpp -o MathQuizGame
./MathQuizGame
```

**Using Visual Studio:**
1. Create a new **Empty C++ Project**
2. Add `main.cpp` to the project
3. Press `Ctrl + F5` to build and run

---

## 🎮 How to Play

1. Run the program
2. Enter the number of questions **(1–10)**
3. Choose a difficulty level:
   - `1` → Easy &nbsp;&nbsp;*(numbers 1–10)*
   - `2` → Medium *(numbers 10–50)*
   - `3` → Hard &nbsp;&nbsp;*(numbers 50–100)*
   - `4` → Mix &nbsp;&nbsp;&nbsp;*(random level each question)*
4. Choose an operation type:
   - `1` → Add `+` &nbsp;&nbsp; `2` → Subtract `-`
   - `3` → Multiply `*` &nbsp; `4` → Divide `/`
   - `5` → Mix *(random operation each question)*
5. Answer each question — feedback is shown immediately
6. View your final score and **Pass / Fail** result
7. Choose to play again or exit

---

## 🧠 Pass / Fail Logic

```
Right Answers >= Wrong Answers  →  ✅ PASS
Right Answers <  Wrong Answers  →  ❌ FAIL
```

---

## 🛠️ Technologies Used

- **Language:** C++
- **Libraries:** `<iostream>`, `<cstdlib>`, `<ctime>`
- **Concepts:** Enums, Structs, Arrays, Functions, Loops, Input Validation, Randomization

---

## 🔮 Possible Improvements

- [ ] Add a **timer** per question
- [ ] Support **floating-point division** for more realistic results
- [ ] Save **high scores** to a file
- [ ] Add a **leaderboard** with player names
- [ ] Port to **cross-platform** (remove `system()` calls)

---

## 👨‍💻 Author

> Built with ❤️ as part of a C++ learning journey.

Feel free to fork, star ⭐, or contribute!

---

## 📄 License

This project is licensed under the **MIT License** — free to use and modify.
