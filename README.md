# Lightweight Agentic AI: Research Assistant Agent 

This project implements a lightweight LLM-based research agent that automates the process of researching a topic, exploring subtopics, gathering online information, summarizing findings, and refining results through critique.

The agent uses modular AI tools in a structured workflow, designed to simulate an early form of agentic behavior — combining tool usage, reasoning, and reflection.

## 🚀Features
Topic Breakdown Tool
Breaks down a broad research topic into smaller, focused subtopics using a language model.

Query Expansion Tool
Expands subtopics by generating related keywords, synonyms, and additional phrases to enhance search breadth.

Search Tool
Retrieves information from the internet using the Brave Search API, with caching mechanisms to optimize API usage.

Summarizer Tool
Synthesizes collected information into a coherent and concise summary.

Critique Tool
Reviews the generated summary, provides suggestions for improvement, and proposes additional areas for exploration.

## Workflow Overview
1. The agent receives a research topic from the user.

2. It uses the Topic Breakdown Tool to split the topic into manageable subtopics or queries.

3. The Query Expansion Tool enhances these subqueries with related terms and phrases.

4. The Search Tool fetches relevant information from online sources based on the expanded queries.

5. The Summarizer Tool compiles a short, meaningful summary from the gathered information.

6. The Critique Tool reviews the summary and suggests improvements or further refinements.

7. The agent delivers the final refined summary to the user.

## 🛠Tech Stack
- Python

- Serverless LLM APIs (TogetherAI, OpenAI, Anthropic, Fireworks, or Groq)

- You API (for search queries)

- Jupyter Notebook (for modular, step-by-step development)

## Key Design Highlights
**Tool-as-Function Approach:**
Each agent capability is modularized as a separate Python function for reusability and clarity.

**Modular Agent Workflow:**
The workflow follows a clean, linear progression but leaves room for adding loops, retries, and dynamic planning.

**Caching Search Results:**
Optional caching is implemented to store and reuse search results, minimizing redundant API calls.coded

## 📚 Future Improvements
Introduce dynamic planning where the agent chooses tools based on intermediate results.

Implement self-correction loops after critique feedback.

Extend to multi-agent collaboration (separate agents for search, summarization, critique).

Integrate semantic search or vector databases for deeper context retrieval.

## 🧑‍💻 Author
- Anvitha Hiriadka
- ![LinkedIn](https://www.linkedin.com/in/anvitha-hiriadka-b68817118/)
