# 🤖 MultiAgentic Chart Generator

![MultiAgent Banner](https://img.shields.io/badge/Powered%20By-LangGraph-blueviolet?style=for-the-badge)  
**MultiAgent** is an autonomous **multi-agent AI system** that collaborates to perform real-time research and generate charts — all via **self-coordinated agents** built on LangGraph & LangChain.

> Turn your natural language queries into fully automated data analysis and visualization!

---

## 🧩 Multi-Agent Workflow Overview

![🕸 MultiAgent Workflow Diagram](./images/workflow.png)

*Two specialized agents collaborate:*

- **Researcher Agent:** Performs web-based research using the Tavily Search Tool to gather concise, structured data.
- **Chart Generator Agent:** Takes the research data and generates charts by executing Python code (e.g., matplotlib).

*Agents take turns, reason independently, and collaborate to complete tasks end-to-end.*

---

## 🚀 Core Features

| Feature                     | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| 🧠 **LangGraph**           | Enables stateful multi-agent coordination                                    |
| 🤖 **LangChain React Agents** | Each agent reasons & selects tools to use intelligently                   |
| 🔍 **Tavily Search Tool**  | Web research tool to fetch real-time data                                   |
| 💻 **Python REPL Tool**    | Executes chart-generating Python code safely                                |
| 🎯 **Custom System Prompts** | Precisely defines agent behavior and handover logic                     |
| 🔁 **Autonomous Transitions** | Agents switch roles until `FINAL ANSWER` is found                      |

---

## 🛠️ Tech Stack & Tools

| Tool | Description | Icon |
|------|-------------|------|
| [LangGraph](https://github.com/langchain-ai/langgraph) | Graph-based multi-agent workflow engine | ![LangGraph](https://img.icons8.com/fluency/48/graph.png) |
| [LangChain](https://github.com/langchain-ai/langchain) | Framework for LLM agents and tool use | ![LangChain](https://img.icons8.com/external-tal-revivo-color-tal-revivo/48/langchain.png) |
| [Gemini 1.5 Flash](https://ai.google.dev) | LLM backend for fast & intelligent decisions | ![Gemini](https://img.icons8.com/color/48/artificial-intelligence.png) |
| [Tavily Search Tool](https://www.tavily.com/) | Real-time web search API | ![Search](https://img.icons8.com/color/48/web-search.png) |
| Python REPL Tool | Executes chart code in real-time | ![Python](https://img.icons8.com/color/48/python--v1.png) |

---
## 💡 Example Query

```txt
Get the UK's GDP over the past 3 years and then generate a line chart. Once the chart is ready, end the process.
```

---

## ⚙️ Installation & Running

1. Clone the repository and navigate to the `Agentic-2.0/langgraph` directory:
   ```bash
   git clone <repository-url>
   cd Agentic-2.0/langgraph
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements1.txt
   ```

3. Set up environment variables for API keys by creating a `.env` file in the root directory with:
   ```
   GROQ_API_KEY=your_groq_api_key_here
   GOOGLE_API_KEY=your_google_api_key_here
   TAVILY_API_KEY=your_tavily_api_key_here
   ```

4. Run the `MulriAgent.ipynb` notebook to start the multi-agent system.

---

## 📄 License

This project is licensed under the MIT License. See the LICENSE file for details.

---
