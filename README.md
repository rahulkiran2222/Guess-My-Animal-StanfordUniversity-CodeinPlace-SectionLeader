# 🐾 Guess My Animal

### Stanford University · Code in Place × Section Leader

<p align="center">
  <strong>An interactive AI-powered guessing game built with Python.</strong>
</p>

<p align="center">
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  </a>
  <img src="https://img.shields.io/badge/AI-LLM-8B5CF6?style=for-the-badge" alt="AI">
  <img src="https://img.shields.io/badge/Stanford-Code%20in%20Place-8C1515?style=for-the-badge" alt="Stanford Code in Place">
  <img src="https://img.shields.io/badge/Status-Complete-16A34A?style=for-the-badge" alt="Project Status">
</p>

---

## 🧩 What is this?

**Guess My Animal** is a command-line game that combines fundamental Python programming with an AI model.

The program secretly chooses an animal. Instead of selecting from predefined questions, the player can ask questions in natural language and use the AI's **Yes/No responses** to narrow down the possibilities.

The goal is simple:

> **Can you figure out the animal before you run out of questions? 🐾**

This project was developed as part of **Stanford University's Code in Place × Section Leader** learning experience.

---

## 🎮 The Experience


                    🐾 START
                       │
                       ▼
              ┌─────────────────┐
              │  Random Animal  │
              │    Selected     │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Ask a Question  │
              │  in Plain Text  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │    🤖 AI Model  │
              │ Evaluates Query │
              └────────┬────────┘
                       │
                       ▼
                 ┌───────────┐
                 │ YES / NO  │
                 └─────┬─────┘
                       │
                       ▼
              ┌─────────────────┐
              │  Make a Guess  │
              └────────┬────────┘
                       │
                ┌──────┴──────┐
                │             │
              ❌ Wrong      ✅ Correct
                │             │
                ▼             ▼
             Continue       🎉 WIN

---

## 💬 Example

I am thinking of an animal.
Can you guess what animal it is?

Ask me a yes or no question: Does it have four legs?
Yes.

Ask me a yes or no question: Does it live in water?
No.

Ask me a yes or no question: Does it bark?
Yes.

Ask me a yes or no question: Is it a dog?
Correct!


The interesting part is that the player is **not limited to a fixed question list**.

Questions can be expressed naturally:

Does it fly?
Does it have fur?
Can it swim?
Is it larger than a dog?
Does it usually live in forests?


---

## 🧠 How the AI is Used

The AI is used as a constrained question-answering component.

The game maintains the hidden animal as part of the program state. When the player asks a question, the AI receives the relevant context and is instructed to:

* evaluate the question against the hidden animal,
* respond with **Yes** or **No**,
* avoid directly revealing the animal.

Conceptually:

Player Question
      │
      ▼
┌──────────────────┐
│ Hidden Animal    │
│ + User Question  │
└────────┬─────────┘
         │
         ▼
    🤖 AI Model
         │
         ▼
   "Yes" / "No"
         │
         ▼
   Player continues

This creates a simple hybrid system:

**deterministic program state + natural-language AI interaction**

---

## 🔍 Core Programming Concepts

Although the game is small, it brings together several fundamental programming ideas:

| Concept         | Application                            |
| --------------- | -------------------------------------- |
| `input()`       | Accepting natural-language questions   |
| Variables       | Maintaining the selected animal        |
| Functions       | Organizing program behavior            |
| `while` loop    | Maintaining the interactive game loop  |
| Conditionals    | Checking guesses and controlling state |
| String handling | Comparing user input and responses     |
| AI prompting    | Constraining model behavior            |

---

## 📁 Project Structure


Guess-My-Animal-StanfordUniversity-CodeinPlace-SectionLeader/
│
├── main.py
├── animal.py
└── README.md


### `main.py`

The main application logic.

It handles:

* selecting the animal,
* interacting with the player,
* receiving questions,
* communicating with the AI,
* checking the player's guess,
* controlling the game loop.

### `animal.py`

Provides the animal-selection functionality used by the game.

---

## ⚙️ Running the Project

Clone the repository:

git clone https://github.com/rahulkiran2222/Guess-My-Animal-StanfordUniversity-CodeinPlace-SectionLeader.git

Move into the project:


cd Guess-My-Animal-StanfordUniversity-CodeinPlace-SectionLeader


Run the program:


python main.py


> **Note:** The AI functionality relies on the environment and AI interface provided for the Code in Place project. The repository therefore preserves the original learning-project structure rather than introducing an independent API setup.

---

## 🧪 Design Perspective

A small design decision in this project is the separation between **game logic** and **AI interaction**.

The Python program remains responsible for:


State
 ↓
Control Flow
 ↓
User Interaction
 ↓
Termination


while the AI is used for:


Natural-language question
          ↓
      Interpretation
          ↓
       Yes / No


This separation keeps the application simple while demonstrating how an AI component can be incorporated into a conventional program.

---

## 🚀 Possible Extensions

The current implementation intentionally focuses on the core interaction.

Natural extensions could include:

* 📊 tracking the number of questions required to solve each game,
* 🧠 maintaining question history,
* 🎯 ranking likely animals after each response,
* 🌳 comparing the AI approach with a decision-tree baseline,
* 🧪 testing consistency across repeated AI responses,
* 📈 evaluating how question strategy affects success rate,
* 🌍 expanding the underlying animal set,
* 🖥️ building a graphical or web-based interface.

These extensions would turn the game from a programming exercise into a small **AI evaluation experiment**.

---

## 🎓 Learning Context

**Stanford University — Code in Place × Section Leader**

This project was created as part of a hands-on programming experience focused on learning Python and experimenting with AI-assisted interaction.

It is an **individual learning project** and is not an official Stanford software product.

---

## 📚 What This Project Represents

This repository is intentionally a small project.

Its value is not the complexity of the game itself, but the exercise of combining:

**Python fundamentals → program state → user interaction → constrained AI behavior**

It represents an early practical step toward building and evaluating interactive AI systems.

---

## 👨‍💻 Author

### Rahul Kiran Gunti

**AI/ML Practitioner · Independent Researcher**

Research interests include:

`LLM Evaluation` · `Foundation Models` · `AI Safety` · `Multilingual NLP` · `Responsible AI`

---

<p align="center">
  <br>
  🐾
  <br>
  <strong>Ask better questions. Think like the animal.</strong>
  <br><br>
  Built with Python + AI
  <br>
</p>
```

