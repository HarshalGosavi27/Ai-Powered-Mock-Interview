# 🎯 Mock Interview Web App

> 💡 An AI-powered mock interview system that simulates real interview scenarios using webcam, microphone, speech-to-text, and Gemini AI evaluation — built with HTML, CSS, JavaScript, PHP & MySQL.

---

## 🚀 Features

- 🎯 **Role-based AI Interview Questions**  
  Select a job role and dynamically generate questions using **Gemini API**
  
- 🎤 **Voice Input with Speech-to-Text**  
  Record answers via **microphone** using **Web Speech API**

- 🎥 **Live Webcam Preview & Face Detection**  
  Real-time **presence monitoring** with 3-strike rule

- 🧠 **AI-based Answer Evaluation**  
  Uses **Gemini AI** with custom prompts to rate and provide feedback

- 📊 **Ratings & Feedback Storage**  
  Feedback is stored per question for detailed analysis

- 📁 **Secure Session Handling**  
  Built using **PHP + MySQL** with local storage via **XAMPP**

- 💾 **Code Editor for Coding Rounds**  
  Integrates **Monaco Editor** for real-time code input and validation

---

## 🧱 Tech Stack

| Layer        | Tech Used                               |
|--------------|------------------------------------------|
| Frontend     | HTML, CSS, JavaScript                    |
| Backend      | PHP (No Composer)                        |
| Database     | MySQL (via XAMPP)                        |
| AI & APIs    | Gemini 2.0 Flash API, Web Speech API     |
| Tools        | Webcam JS, Monaco Editor, XAMPP Server   |

---

## 🗃️ Database Structure

- 🗂️ **`interviews`**  
  Stores generated mock questions & job role details.

- 🗂️ **`userAnswer`**  
  Stores user answers, AI rating, and feedback per question.

---

## 📸 Interview Experience Flow

- ✅ Webcam preview activates on start  
- 🧍 Face detection with a **3-strike rule** if the user goes out of frame  
- 🔁 One-by-one question navigation  
- 🎙️ Answer via mic — validated automatically (minimum 10 words)  
- 📈 AI generates rating + feedback stored in database

---

## 📦 How to Run Locally

> You’ll need [XAMPP](https://www.apachefriends.org/index.html) and a Gemini API key

```bash
1. Clone the repository
2. Place the project in your XAMPP `htdocs` folder
3. Import the provided SQL schema into phpMyAdmin
4. Add your Gemini API key in the respective PHP files
5. Start Apache & MySQL servers from XAMPP
6. Navigate to `http://localhost/mock-interview/` in your browser
