# AI Agents with CrewAI

Multi-agent workflows built with CrewAI demonstrating data quality automation
and autonomous research reporting.

## Notebooks

**data_quality_crews.ipynb** - 4-agent pipeline that profiles a SQLite table,
flags issues, writes and executes SQL fixes, and produces a report. Uses Claude
Haiku. Two-stage design with a human review checkpoint before fixes are applied.

**data_scientist_or_agent.ipynb** - 3-agent research crew that takes any topic,
searches the web, extracts insights, and produces an executive summary. Runs on
Llama 3.2 locally via Ollama.

## Setup

```bash
pip install crewai crewai-tools
```

Set `ANTHROPIC_API_KEY` and `SERPER_API_KEY` in your environment. For the
research notebook, install [Ollama](https://ollama.com) and run `ollama pull llama3.2`.
