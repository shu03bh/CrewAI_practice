

```markdown
# 🤖 CrewAI Practice Projects – Multi-Agent Systems

This repository contains my practice implementations of multi-agent systems using **CrewAI**.

It includes two separate AI crews:

1. 📝 Research & Blog Writer Crew
2. 📊 Market Research Analyst Crew

Both projects demonstrate how multiple AI agents collaborate to complete structured tasks.

---

## 🧠 About CrewAI

CrewAI is a Python framework used to build multi-agent systems where:

- Each agent has a role and goal
- Tasks are assigned to specific agents
- Agents collaborate in structured workflows
- Execution is autonomous using `kickoff()`

---

# 📝 Project 1: Research & Blog Writer Crew

## 📌 Overview

This crew simulates a content creation pipeline where:

1. Research Agent gathers information
2. Writer Agent creates a blog post

### 🔹 Workflow

User Topic → Research Agent → Writer Agent → Final Blog Output

### 🔹 Process Type
Sequential execution

### 🔹 Features

- Goal-oriented agents
- Task-based workflow
- Structured output
- Dynamic topic input

---

# 📊 Project 2: Market Research Analyst Crew

## 📌 Overview

This crew simulates a market analysis workflow where agents:

1. Analyze a product idea
2. Perform competitor research
3. Generate a structured market report

### 🔹 Workflow

Product Idea → Market Research Agent → Analysis → Final Report

### 🔹 Features

- Analytical reasoning
- Structured reporting
- Tool usage 
- Goal-driven analysis

### Tools Used 

- SerperDevTool
- ScrapeWebsiteTool
- SeleniumScrapingTool

---

# 🏗 Architecture Overview

```

User Input
↓
Crew
↓
Agents
↓
Tasks
↓
Tools 
↓
Final Output

```

Both projects follow CrewAI’s core pillars:

- Agents
- Tasks
- Crew
- Execution (`kickoff()`)

---

# ⚙️ Tech Stack

- Python 3.10+
- CrewAI
- UV (Package Manager)
- YAML configuration
- OpenAI / Groq LLM

---

# 📁 Project Structure

```

crew-ai/
│
├── research_blog_writer/
│   ├── config/
│   ├── crew.py
│   ├── main.py
│
├── market_research_analyst/
│   ├── config/
│   ├── crew.py
│   ├── main.py
│
├── .env
└── README.md

```

---

# 🔧 Installation

### 1️⃣ Clone Repository

```

git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
cd your-repo-name

```

### 2️⃣ Install UV

```

pip install uv

```

### 3️⃣ Install CrewAI

```

uv tool install crewai

```

### 4️⃣ Add API Key

Create `.env` file:

```

OPENAI_API_KEY=your_api_key_here

```

---

# ▶️ Running the Projects

### Run Research & Blog Writer

```

cd research_blog_writer
python main.py

```

### Run Market Research Analyst

```

cd market_research_analyst
python main.py

```

---

# 📊 Example Outputs

## Blog Writer Crew Output:
- Topic-based blog article
- Structured sections
- SEO-friendly formatting

## Market Research Crew Output:
- Market overview
- Competitor analysis
- SWOT insights
- Final recommendation

---

# 📚 What I Learned

Through these projects, I practiced:

- Designing multi-agent systems
- Defining agent roles and goals
- Task orchestration
- YAML configuration
- Structured execution using `kickoff()`
- Tool integration

---

# 🚀 Future Improvements

- Add structured JSON output
- Add FastAPI API layer
- Add long-term memory (RAG)
- Add cost monitoring
- Add human-in-the-loop approval

---

# 🔐 Security

- API keys stored in `.env`
- `.env` excluded via `.gitignore`
- No sensitive data committed
```

