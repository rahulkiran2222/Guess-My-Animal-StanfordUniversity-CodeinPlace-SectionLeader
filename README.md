# 🐾 Guess My Animal
### Stanford University — Code in Place × Section Leader

<p align="center">
  <strong>An interactive AI-powered animal guessing game built with Python.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/AI-Powered-purple" alt="AI Powered">
  <img src="https://img.shields.io/badge/Stanford-Code%20in%20Place-red" alt="Stanford Code in Place">
  <img src="https://img.shields.io/badge/Project-Interactive-green" alt="Interactive Project">
</p>

---

## 🧠 Overview

**Guess My Animal** is a small interactive Python project that explores how a traditional guessing game can be extended with an AI model.

The program secretly selects an animal and allows the player to ask **yes/no questions** to narrow down the possibilities. An AI model interprets each question and provides a constrained response without revealing the hidden animal.

The project was developed as part of **Stanford University's Code in Place × Section Leader** learning experience.

---

## 🎮 How It Works

```text
┌──────────────────────┐
│  🎲 Select an Animal │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   ❓ Player Question │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   🤖 AI Interprets   │
│      the Question    │
└──────────┬───────────┘
           │
           ▼
      ┌───────────┐
      │ Yes / No  │
      └─────┬─────┘
            │
            ▼
     ┌───────────────┐
     │ Guess Animal? │
     └───────┬───────┘
             │
       ┌─────┴─────┐
       │           │
      No          Yes
       │           │
       ▼           ▼
    Continue    🎉 Correct!
