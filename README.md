# Evaluating Business Process Feedback using LLM and DMN

This repository presents the implementation and evaluation of a novel **DMN-guided prompting framework** for controlling Large Language Models (LLMs) in automated feedback generation. The work is based on the thesis:

📄 **DMN-Guided Prompting: A Low-Code Framework for Controlling LLM Behavior**  
🧑‍🎓 Master’s Thesis, Politecnico di Torino  
👨‍🏫 Supervised by Dr. Amin Jalali, Stockholm University

---
## 🔍 Overview

LLMs like GPT-4 offer powerful capabilities for natural language reasoning, but lack structure, transparency, and maintainability when used with traditional prompt engineering. This project proposes a **low-code approach** that uses **Decision Model and Notation (DMN)** to modularize and guide LLM behavior, enabling:

- **Structured, rule-based prompting** using DMN elements.
- **Automated feedback generation** for process modeling tasks.
- **Improved precision, interpretability, and scalability** over ad hoc prompts.

The approach is demonstrated using a loan approval process scenario and example feedback texts.
---

## 🚀 Key Features

✅ **Modular Prompting**  
Breaks down decision logic into triples: input fields, decision table, and literal expression.

✅ **Low-Code Framework**  
Users define or modify decision rules in DMN, with no need to edit complex LLM prompts.

✅ **Educational Case Study**  
Applied in a graduate-level course to evaluate Petri net models and generate feedback.

---
## 📁 Repository Structure

The repository is organized as follows:
```
├── README.md                         # Project documentation
├── requirements.txt                  # Python libraries required
├── src/                              # Source code and related files
│   └── process_feedback/             
│       ├── loan_approval.ipynb       # Main notebook: LLM + DMN evaluation
│       ├── loan_approval.dmn         # DMN file for decision logic
│       └── feedback_examples/        # Sample natural language inputs
│           ├── loan_approval_test1.txt
│           ├── loan_approval_test2.txt
│           └── loan_approval_test3.txt
└── utils/                            
    └── convert_pnml_to_text.ipynb    # Converts PNML to text descriptions
```
## 🧪 How It Works

1. **User Input**: A process description in plain English (e.g., student assignment).
2. **Decision Logic**: Encoded in a DMN model with rules and feedback messages.
3. **Prompt Framework**:
   - Parses the DMN into triples.
   - Guides the LLM to extract inputs, evaluate rules, and generate responses.
4. **Output**: A decision-specific feedback message.

No manual prompt tweaking is needed; just modify the DMN file.

---

## 🚀 Getting Started

### Requirements

* Python 3.8 or higher
* openai
* Jupyter Lab or Jupyter Notebook
* An API key for the Large Language Model you are using (e.g., OpenAI).

### Installation

```bash
git clone https://github.com/Shaghayegh-Abedi/DMN-prompting-project
cd dmn-guided-prompting
pip install -r requirements.txt
```

---

## License

This project is licensed under the MIT License.

## Citation


---
