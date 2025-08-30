# 💻 HackTheTest – Console Based Exam System  

A simple **Java console application** that allows **Teachers** to upload questions and **Students** to take tests.  
This project simulates a real exam system where users can **register, login, upload Q&A, attempt tests, and view scores**.  

---

## 🚀 Features  

### 👩‍🏫 Teacher Side
- Register/Login as a Teacher  
- Add questions (MCQ, Fill-Ups, Statements)  
- View uploaded questions  

### 👨‍🎓 Student Side
- Register/Login as a Student  
- Attempt tests (randomly generated from the Question Bank)  
- Submit answers and view scores instantly  

### 🔐 Common
- Console-based interface → simple & portable  
- Modular design with clear class separation  
- Easy to expand (e.g., database, encryption, GUI in future)  

---

## ⚙️ How It Works  

1. **Registration/Login**  
   - Users sign up as either Teacher or Student  
   - Credentials stored in a simple in-memory DB (or file)  
   - Role-based menu shown after login  

2. **Teacher Flow**  
   - Choose question type (MCQ, FillUp, Statement)  
   - Enter question text, options, and correct answer  
   - Questions stored in the Question Bank  

3. **Student Flow**  
   - Login → choose **Take Test**  
   - System fetches random questions from Question Bank  
   - Student answers questions in console  
   - System evaluates answers and calculates score  

4. **Result Handling**  
   - Results shown immediately after submission  
   - Scores can be extended to file/DB storage  

---

## 🏗️ Project Structure  
src/
├── User.java # Base user class
├── Teacher.java # Teacher-specific methods
├── Student.java # Student-specific methods
├── Question.java # Question model (MCQ/FillUp/Statement)
├── Test.java # Test creation & evaluation logic
├── Database.java # Simulated DB (in-memory/file-based)
└── Main.java # Entry point with menus
