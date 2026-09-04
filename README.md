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

Example interaction

I am thinking of an animal.
Can you guess what animal it is?

Ask me a yes or no question: Does it have four legs?
Yes.

Ask me a yes or no question: Does it live in water?
No.

Ask me a yes or no question: Is it a dog?
Correct!

✨ Key Features
🐾 Random animal selection
🤖 AI-assisted question answering
💬 Natural-language user interaction
🔄 Continuous question-and-answer loop
🎯 Hidden target until the correct guess
🧩 Prompt-based response constraint
🐍 Python fundamentals applied to an interactive application

🔍 Technical Approach
The project combines basic program control flow with an AI reasoning component.
1. Hidden state
An animal is selected at the beginning of the game and stored as the target state.
2. Natural-language input
Instead of restricting the player to predefined questions, the program accepts free-form questions.
For example:
Does it live in water?
Can it fly?
Is it bigger than a dog?
Does it have fur?
3. Constrained AI response
The player's question is provided to the AI together with the hidden animal.
The prompt instructs the model to:
determine whether the question is true for the selected animal,
answer only with Yes or No,
avoid revealing the hidden animal.
This makes the AI component function as a controlled question-answering layer rather than simply generating unrestricted text.
4. Iterative interaction
A loop allows the player to continue asking questions until the correct animal is identified.

🗂️ Project Structure
guess-my-animal-stanford-code-in-place/
│
├── main.py
├── animal.py
└── README.md
main.py
Contains the main game logic, including:
animal selection
user interaction
question loop
AI interaction
termination condition
animal.py
Provides the random animal-selection functionality used by the game.

🛠️ Technologies & Concepts
Technology / Concept	Use
Python	Core implementation
AI / LLM	Natural-language question answering
Functions	Program organization
Loops	Repeated interaction
Conditionals	Game-state decisions
User Input	Interactive gameplay
Prompt Engineering	Constrained AI responses

💡 What I Learned
This project provided a practical introduction to combining conventional programming with generative AI.
In particular, it helped me practice:
designing an interactive program,
controlling program state,
handling repeated user interaction,
integrating an AI model into a deterministic workflow,
writing prompts with explicit behavioral constraints,
thinking about how AI-generated outputs can be constrained by program logic.
A key design idea was to separate the game state from the AI response layer: the program knows the hidden animal, while the AI is used to interpret the player's natural-language questions.

🎓 Context
Program: Stanford University — Code in Place × Section Leader
This project was developed as a hands-on programming exercise while learning Python and experimenting with AI-assisted interaction.
It is an individual learning project rather than an official Stanford software product.

🚀 Running the Project
The project was developed for the Code in Place environment and uses the provided project modules.
Clone the repository:
git clone https://github.com/rahulkiran2222/guess-my-animal-stanford-code-in-place.git
cd guess-my-animal-stanford-code-in-place
Then run:
python main.py
Note: The exact AI execution environment depends on the Code in Place setup used for the project.

🔮 Possible Extensions
The current implementation intentionally remains simple. Possible future improvements include:
📊 Tracking the number of questions asked
🧠 Maintaining a history of previous questions
🎯 Ranking candidate animals after each answer
🌳 Implementing a decision-tree baseline for comparison
📈 Comparing AI-based and rule-based guessing strategies
🧪 Evaluating the consistency of AI answers
🌍 Expanding the animal knowledge base
🖥️ Building a graphical/web interface

👨‍💻 Author
Rahul Kiran Gunti
AI/ML Practitioner · Independent Researcher
Research interests include LLM evaluation, foundation models, AI safety, multilingual NLP, and responsible AI.
<p align="center"> 🐾 <strong>Small project. Simple idea. First steps toward building interactive AI systems.</strong> </p> ```
