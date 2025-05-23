
# 🚀 RAG-Based Personalized Learning Path Recommender

A smart career guidance tool that uses **Retrieval-Augmented Generation (RAG)** to connect **existing user skills** with **technical learning recommendations** — guiding learners toward their dream job roles using real-world skill data.

## 🔍 Problem Statement

Many learners complete online courses without a clear idea of what to learn next. Companies offering these courses struggle to:
- Guide users effectively.
- Boost course engagement.
- Align learning with real job roles.

This tool solves that by:
> Matching a user’s **current skills** with **career paths**, and recommending what skills (and therefore courses) to learn next.

## 💡 What It Does

🧠 Uses a structured skills-role JSON dataset (**`compressed_RAG_data.json`**) as a **retrieval base**.  
🔎 Retrieves roles that match a student’s career goal.  
🧾 Compares known vs. required skills.  
🎯 Suggests targeted learning areas to bridge the gap.

## 📁 `compressed_RAG_data.json`

This file is the **heart of the RAG pipeline**. It contains job roles and their associated in-demand technical skills that are:
- **Hot Technologies**
- **Relevant in the industry**

It powers the system’s ability to personalize learning paths based on skill gaps.

## 🧪 Example Use Case

```python
user_skills = ["Python", "MATLAB", "Microsoft Excel"]
target_role = "Electrical Engineers"
```

### Output:
```
🎯 Target Role: Electrical Engineers

✅ Your Skills: python, matlab, microsoft excel

🧠 Skills You Need to Learn: c++, verilog, labview

📘 Recommended Learning Areas:
- Learn **C++** via relevant courses or platforms
- Learn **Verilog** via relevant courses or platforms
- Learn **Labview** via relevant courses or platforms
```

## 🧰 Tech Stack

| Component | Usage |
|----------|-------|
| 🐍 Python | Core logic |
| 📁 JSON | Role-skill data (retrieval base) |
| 📚 Pandas | Data processing |
| 🌐 Google Colab | Interactive execution |
| 🤖 Optional GPT | Future enhancement |

## 📂 File Structure

```plaintext
├── compressed_RAG_data.json   # 🔍 Retrieval data source for RAG pipeline
├── recommend_path.ipynb       # 🧠 Colab notebook (core logic)
└── README.md                  # 📘 Project overview and instructions
```

## 🛠 How To Use

1. Clone this repo or open the Colab notebook.
2. Upload `compressed_RAG_data.json` (already included in repo).
3. Provide:
   - A list of current skills.
   - A target job role.
4. Get personalized skill gap analysis + recommendations.


## 👩‍💻 Made For

- Q-Hackathon Problem Focused
- Developers exploring RAG + LLM applications

## 📣 Contribute

Ideas or improvements? Open an issue or PR — let’s build smarter learning tools together!