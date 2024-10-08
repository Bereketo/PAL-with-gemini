# PAL (Program-aided Language) using Gemini 1.5**

This project leverages **Google's Generative AI Model (Gemini 1.5)** in conjunction with **Program-aided Language (PAL)** prompt engineering to automatically generate and execute Python code based on user-provided problem descriptions. The PAL methodology plays a pivotal role in improving the quality, relevance, and precision of code generation by framing the problem for the AI in a structured way that leads to more accurate code outputs.

---

## **Table of Contents**

- [Overview](#overview)
- [Why PAL?](#why-pal)
- [Installation](#installation)
- [Usage](#usage)


---

## 📖 **Overview**

In this project, I use **Google's Gemini 1.5** to generate Python code based on problem statements provided by the user. I employ the **Program-aided Language (PAL)** method to ensure that the prompts sent to the AI are structured in such a way that they effectively guide the AI to produce useful, executable Python code.



---

## **Why PAL?**

**Program-aided Language models (PAL)** approach uses large language models (LLMs) to read natural language problems and generate programs as intermediate reasoning steps. However, PAL offloads the actual solution step to a runtime environment, such as a Python interpreter. This methodology is especially useful when the problem-solving process is complex and requires both logical reasoning and computational steps.

In this project, PAL is critical for the following reasons:

- **Intermediate Reasoning**: The PAL approach generates Python code that serves as an intermediate reasoning step to solve the natural language problem. The actual solution is executed by the Python interpreter at runtime, not just by the AI model.
- **Problem Structuring**: PAL helps break down complex problem descriptions into a structured format, making it easier for the AI to generate accurate Python code.
- **High-Quality Outputs**: PAL guides the AI to produce relevant and well-formatted code, minimizing the need for additional edits or corrections.
- **Prompt Engineering**: The PAL method allows us to seamlessly integrate a prompt like "generate a python code" directly within the user-provided problem description, ensuring clarity and alignment with the task.


---

## ️ **Installation**

### 1. **Clone the Repository**
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. **Install required packages**
```bash
pip install -r requirements.txt
```
### 3. **Set up your API key**
This project uses Google's Gemini 1.5 model, and an API key is required to access it. Make sure your API key is set as an environment variable:
```bash
export GEMINI_API_KEY='your-gemini-api-key'
```
## **Usage**
### 1. **Start jupyter notebook**
### 2. **run the notebook**
- The notebook will prompt you for a problem description. You can either provide a custom problem or press Enter to use the default prompt.
- If no prompt is entered, a default prompt will be used.
- Gemini 1.5 will generate Python code based on the provided prompt and execute it directly within the notebook and the executed result is returned.

### **Default prompt example**
if no prompt is provided this default prompt will be used 
```bash
Liam spent the morning on three tasks:
He worked on a project for 2 hours and 15 minutes.
After a 25-minute break, he reviewed his emails for 45 minutes.
Then, he attended a 1-hour 30-minute meeting.
In the afternoon, he:
Spent 1 hour 45 minutes writing a report.
Took a 20-minute coffee break and then worked for another 2 hours.
How much time did Liam spend working in total? 
Generate a Python code to solve the problem.
```

### Execution 
The code is executed in the notebook and the result is displayed

**sample output**
```bash
Executing the generated code...
Liam spent 8 hours and 15 minutes working in total.
```
> **please refer to the notebook for detail code and examples**
