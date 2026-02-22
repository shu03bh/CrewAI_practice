```markdown
# 🤖 CrewAI Practice Projects – Multi-Agent Systems

This repository contains my practice implementations of multi-agent systems using **CrewAI**.

It includes two separate AI crews:

1. 📝 Research & Blog Writer Crew  
2. 📊 Market Research Analyst Crew  

Both projects demonstrate how multiple AI agents collaborate in structured workflows using roles, goals, tasks, and tools.

---

## 🧠 About CrewAI

CrewAI is a Python framework for building multi-agent systems.  
It allows developers to:

- Define specialized agents with roles and goals
- Assign tasks to specific agents
- Control workflow execution (Sequential / Hierarchical)
- Run autonomous multi-agent pipelines using `kickoff()`

---

# 📝 Project 1: Research & Blog Writer Crew

## 📌 Overview

This project simulates a structured content creation pipeline.

### Workflow

```

User Topic
↓
Research Agent
↓
Writer Agent
↓
Final Blog Output

```

### Description

- The **Research Agent** gathers and structures information about the given topic.
- The **Writer Agent** converts research into a formatted blog post.

### Process Type

Sequential execution.

### Features

- Goal-driven agents
- Clear task separation
- Dynamic topic input
- Structured multi-step workflow

---

# 📊 Project 2: Market Research Analyst Crew

## 📌 Overview

This project simulates a product market analysis workflow using multiple agents.

### Workflow

```

Product Idea
↓
Market Research Agent
↓
Competitor Analysis
↓
Final Market Report

```

### Description

- The agent performs market research on a given product idea.
- It gathers online insights using tools.
- It generates a structured analytical report including recommendations.

### Tools Used

- `SerperDevTool`
- `ScrapeWebsiteTool`
- `SeleniumScrapingTool`

### Features

- Tool-integrated agent execution
- Structured report generation
- Market reasoning workflow
- Autonomous task execution

---

# 🏗 Overall Architecture

Both projects follow CrewAI’s four core components:

```

User Input
↓
Crew (Multi-Agent System)
↓
Agents (Specialized Roles)
↓
Tasks (Defined Work Units)
↓
Tools (Optional External Actions)
↓
Final Output

```

Core pillars used:

- Agents
- Tasks
- Crew
- Execution (`kickoff()`)

---

# ⚙️ Tech Stack

- Python 3.10+
- CrewAI
- UV (Package Manager)
- YAML Configuration
- OpenAI / Groq LLM

---

# 📁 Project Structure

```

crew-ai/
│
├── research_blog_writer/
│   ├── config/
│   │   ├── agents.yml
│   │   ├── tasks.yml
│   ├── crew.py
│   ├── main.py
│
├── market_research_analyst/
│   ├── config/
│   │   ├── agents.yml
│   │   ├── tasks.yml
│   ├── crew.py
│   ├── main.py
│
├── .env
└── README.md

```

---

# 🔧 Installation

## 1️⃣ Clone Repository

```

git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
cd your-repo-name

```

## 2️⃣ Install UV

```

pip install uv

```

## 3️⃣ Install CrewAI

```

uv tool install crewai

```

## 4️⃣ Add API Key

Create a `.env` file in the root directory:

```

OPENAI_API_KEY=your_api_key_here

```

Make sure `.env` is included in `.gitignore`.

---

# ▶️ Running the Projects

## Run Research & Blog Writer

```

cd research_blog_writer
python main.py

```

## Run Market Research Analyst

```

cd market_research_analyst
python main.py

```

---

# 📊 Example Outputs

## Blog Writer Crew

- Topic-based blog article
- Structured headings
- Organized sections

## Market Research Crew

- Market overview
- Competitor insights
- SWOT analysis
- Final recommendations

---

# 📚 What I Learned

Through these projects, I practiced:

- Designing multi-agent systems
- Defining agent roles and goals
- Task orchestration
- YAML-based configuration
- Tool integration
- Structured execution using `kickoff()`

---
