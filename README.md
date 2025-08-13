📌 Overview
Agentic Flow is a hands-on project demonstrating multi-step Large Language Model (LLM) prompt chaining, where the output from one LLM call becomes the input for the next.
It’s an early step toward Agentic AI — AI systems capable of reasoning, planning, and acting with minimal human intervention.

This implementation uses Python and the OpenAI API to:

Generate initial ideas or questions.

Expand and refine them through multiple chained LLM calls.

Converge on a final, actionable solution.

🛠️ Tech Stack
Python 3.12+

OpenAI API (gpt-4.1-nano & gpt-4.1-mini)

Jupyter Notebook

python-dotenv for environment variable management

IPython.display.Markdown for clean output formatting

📂 Project Structure

AgenticFlow/
│── 1_foundations/1_lab1.ipynb    # Main Jupyter Notebook
│── .env                          # API keys (excluded from repo)
│── requirements.txt              # Dependencies
│── assets/                       # Diagrams and visuals

🔄 Workflow Diagram

flowchart LR
    A[User Prompt: Pick Business Area] --> B[LLM Call 1: gpt-4.1-mini]
    B -->|Output: Industry| C[User Prompt: Identify Pain Point]
    C --> D[LLM Call 2: gpt-4.1-mini]
    D -->|Output: Challenge| E[User Prompt: Propose Agentic AI Solution]
    E --> F[LLM Call 3: gpt-4.1-mini]
    F -->|Final Solution| G[Markdown Display in Notebook]
    ![PromptCascade Flow](assets/PromptCascade_flow_svg.svg)

🧠 Example Flow
Step 1 – Select Business Area

"Please pick a business area worth exploring for Agentic AI."
LLM Output: Supply Chain Logistics Optimization

Step 2 – Identify Pain Point
"Please present a major pain point in Supply Chain Logistics Optimization."
LLM Output: Complexity and delays caused by real-time disruptions.

Step 3 – Propose Agentic AI Solution
"Please propose an Agentic AI solution to resolve the challenge."
LLM Output:
Autonomous agents that continuously monitor IoT, GPS, and weather data to proactively re-route shipments and coordinate across stakeholders in real-time.

📈 Learning Outcomes
From this project, I learned:

Designing multi-step LLM workflows for progressive reasoning.

Choosing between cost-effective and high-quality LLM models depending on task complexity.

Structuring AI outputs for human readability.

Laying groundwork for fully autonomous agentic systems.

📬 Connect
If you’re exploring LLM applications or Agentic AI:
💼 [LinkedIn – Divyani Audichya](https://www.linkedin.com/in/divyaniaudichya/)
