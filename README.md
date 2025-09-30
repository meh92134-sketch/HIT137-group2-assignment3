# HIT137 Group Assignment 3 — Group 2  
**Group Members:**  
- lakshikadhonchak@gmail.com  
- aryankadiyan90@gmail.com  
- princerozera98@gmail.com  
- arpitgholia1234@gmail.com  

---

## 📌 Project Overview
This project demonstrates the integration of **Hugging Face AI models** into a **Tkinter GUI** while applying key **Object-Oriented Programming (OOP) concepts**.  
The application allows users to:
- Select between **two AI models from different categories**.  
- Provide input (text or image).  
- Run the selected model and view the results.  
- View **OOP concept explanations** and **model information** directly inside the GUI.  

---

## 📂 Project Structure
HIT137_Project_Group2/
├── main.py              # App entrypoint
├── gui.py               # Tkinter GUI (layout, menus, logic)
├── models.py            # AI model classes (SummarizationModel, ZeroShotModel, base AIModel)
├── oop_examples.py      # LoggerMixin, OOPExplanationMixin
├── utils.py             # Decorators (log_decorator, timeit_decorator) + helpers
├── requirements.txt     # Dependencies
├── github_link.txt      # Repository URL
└── outputs/             # Example screenshots & results

---

## 🤖 Hugging Face Models Used
1. **Summarization**  
   - Model: sshleifer/distilbart-cnn-12-6  
   - Task: Text Summarization  
   - Purpose: Converts long input text into concise summaries.  

2. **Zero-Shot Classification**  
   - Model: facebook/bart-large-mnli  
   - Task: Zero-Shot Text Classification  
   - Purpose: Classifies text into arbitrary labels without retraining.  

---

## 🧩 OOP Concepts Demonstrated
- **Encapsulation:** Private attributes like _model_name and _pipeline in AIModel.  
- **Polymorphism:** run_any_model() accepts any AIModel subclass and calls run().  
- **Method Overriding:** Child classes (SummarizationModel, ZeroShotModel) override run().  
- **Multiple Inheritance:** App inherits from tk.Tk, LoggerMixin, and OOPExplanationMixin.  
- **Multiple Decorators:** @log_decorator and @timeit_decorator stacked on run() methods.  

---

## 🖥️ GUI Workflow
1. Start the application: python main.py  
2. Select a model from the dropdown (Summarization or Zero-Shot).  
3. Choose input type (Text or Image).  
4. Enter text or browse an image file.  
5. Click Run Model to execute.  
6. View:
   - Model output in the output display.  
   - Model info (name, task, short description).  
   - OOP explanations of applied concepts.  

---

## ⚙️ Installation & Running
1. Clone the repository:
   git clone https://github.com/<your-group2-repo>.git
   cd HIT137_Project_Group2

2. Create & activate a virtual environment:
   python -m venv venv
   venv\Scripts\activate       

3. Install dependencies:
   pip install -r requirements.txt

4. Run the GUI:
   python main.py

---

## 📊 Example Results
- **Summarization Example:**  
  Input:  
  > “Artificial Intelligence is transforming industries such as healthcare, education, and transportation...”  
  Output:  
  > “AI is transforming industries by automating tasks and enabling efficiency.”  

- **Zero-Shot Classification Example:**  
  Input:  
  The new smartphone has excellent battery life and display. ||| technology, sports, politics  
  Output:  
  {"labels": ["technology"], "scores": [0.92], "sequence": "The new smartphone..."}

Screenshots of results are included in the outputs/ folder.  

---

## 📎 Submission Notes
- Repository link saved in github_link.txt.  
- Submission ZIP includes: all code files, requirements.txt, outputs, and github_link.txt.  
- All contributions tracked on GitHub with commits from group members.  

---

## 📚 References
- Hugging Face — Models & Transformers Documentation  
- Python — Tkinter Documentation  
- GitHub — Collaboration Guide  
