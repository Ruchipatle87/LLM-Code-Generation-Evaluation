# LLM Code Generation Evaluation

## Performance Evaluation of Large Language
## Models for Code Generation using GPT-2,
## DialoGPT-medium and CodeGen-350M

---

## 📌 Project Overview

This project evaluates and compares three
Large Language Models for automatically
generating Python code from plain English
problem statements.

- **GPT-2** — General purpose model (OpenAI)
- **DialoGPT-medium** — Conversational model
  (Microsoft)
- **CodeGen-350M** — Code specialized model
  (Salesforce)

---

## 🎯 Evaluation Metrics

| Metric | Description |
|--------|-------------|
| Quality Score | Structural correctness (0.0 to 1.0) |
| Latency | Time taken to generate code (seconds) |
| Tokens Generated | Number of new tokens produced |
| Token Efficiency | Quality per token used |

---

## 🔍 Quality Checks

1. Correct function name (def solution)
2. No repetition of lines
3. No self keyword
4. Has return statement

---

## 📊 Results

| Model | Quality Score | Label |
|-------|--------------|-------|
| GPT-2 | 0.50 | Average |
| DialoGPT-medium | 0.75 | Good |
| CodeGen-350M | 1.00 | Excellent |

---

## 🛠️ Technologies Used

- Python
- Google Colab
- HuggingFace Transformers
- PyTorch
- Pandas
- Matplotlib
- HTML, CSS, JavaScript
- Chart.js

---

## 🚀 How To Run

```
Step 1 → Open Google Colab
         colab.research.google.com

Step 2 → Upload the notebook file
         LLM_Code_Generation_Evaluation.ipynb

Step 3 → Run all cells in order
         Cell 1 → Install libraries
         Cell 2 → Import modules
         Cell 3 → Load GPT-2
         Cell 4 → Load DialoGPT-medium
         Cell 5 → Load CodeGen-350M
         Cell 6 → Define generate_code function
         Cell 7 → Define plot and evaluate function
         Cell 8 → Run user input cell

Step 4 → In Cell 8 change my_problem variable
         to your own problem statement
         Example:
         my_problem = "Write a Python function
         that adds two numbers"

Step 5 → Run Cell 8 and wait for output

Step 6 → View quality breakdown and
         comparison table in Colab output

Step 7 → View 4 bar charts generated
         automatically

Step 8 → Click Open Dashboard button
         to open interactive HTML dashboard
         in new browser tab
```

## 📊 Sample Output

| Model           | Quality   | Score | Latency  | Tokens | Efficiency |
|-----------------|-----------|-------|----------|--------|------------|
| GPT-2           | Average   | 0.50  | 10.431s  | 150    | 3.33       |
| DialoGPT-medium | Good      | 0.75  | 47.030s  | 1      | 0.00       |
| CodeGen-350M    | Excellent | 1.00  | 22.013s  | 150    | 6.67       |

---

## 🔑 Key Findings

- CodeGen-350M consistently outperformed both
  general purpose models across all evaluated
  problems
- GPT-2 generated repetitive class style code
  using self keyword making it completely unusable
- DialoGPT-medium generated only 1 token proving
  conversational models cannot generate code at all
- Domain specific training on programming data is
  essential for high quality automated code
  generation

---

## 🔮 Future Scope

- Add execution based testing with automated
  test cases
- Include more models like StarCoder and CodeLlama
- Support multiple programming languages
  beyond Python
- Deploy as web application using Flask

