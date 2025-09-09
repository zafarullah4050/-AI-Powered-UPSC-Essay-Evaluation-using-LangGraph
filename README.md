# -AI-Powered-UPSC-Essay-Evaluation-using-LangGraph
📌 Overview

This project demonstrates how to use LangGraph to build an AI workflow for UPSC-style answer evaluation.
The workflow is designed as a graph, where each step evaluates different aspects of an answer (language, analysis, thought process), and finally produces a combined evaluation.

⚡ Workflow Design
Nodes in the Graph

Evaluate Language → Checks grammar, clarity, and structure of the answer.

Evaluate Analysis → Evaluates depth, factual correctness, and arguments.

Evaluate Thought Process → Measures originality, coherence, and flow of ideas.

Final Evaluation → Combines all three evaluations into a single report.

Graph Flow
START → evaluate_language → final_evaluation
START → evaluate_analysis → final_evaluation
START → evaluate_thought → final_evaluation
final_evaluation → END

🔧 Tech Stack

Python

LangGraph (stateful agentic AI workflows)

LangChain (LLM integration)

🚀 How to Run

Clone this repository

Install dependencies:

pip install langgraph langchain


Run the notebook:

jupyter notebook UPSC_Workflow.ipynb

🎯 Use Case

This project can be extended for:

Academic answer evaluation

Essay scoring

Interview preparation feedback

Automated report generation

🌟 Future Scope

Add memory to track multiple answers per candidate

Use RAG (Retrieval-Augmented Generation) for fact-checking answers

Deploy as a web app using Streamlit or FastAPI
