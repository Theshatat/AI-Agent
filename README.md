# Blog Agent

> <!-- TODO: one sentence. What does the agent produce, and for whom? Example: "An AI agent that researches a topic and writes a structured blog post draft." -->

Built with [Google Agent Development Kit (ADK)](https://google.github.io/adk-docs/) and Python.

<!-- TODO: add a screenshot or GIF of the agent running in the ADK web UI. A demo in the first screen of the README matters more than any other section. -->

---

## Features

<!-- TODO: replace with what agent.py actually does. Keep 3-5 bullets, each one verifiable in the code. -->

- <!-- e.g. Generates a blog outline from a topic -->
- <!-- e.g. Writes the full article in a chosen tone/length -->
- <!-- e.g. Uses tools (web search, etc.) -->

## How It Works

<!-- TODO: 3-5 lines describing the flow: input -> agent instructions -> model -> tools (if any) -> output.
     Mention the model used (e.g. gemini-2.x) and whether it is a single agent or multiple sub-agents. -->

## Tech Stack

| Layer | Technology |
|---|---|
| Language | Python 3.13 |
| Agent framework | Google ADK |
| LLM | <!-- TODO: model name --> |
| Session storage | SQLite (ADK session DB) |

## Project Structure

```
.
├── blog_agent/
│   ├── __init__.py
│   └── agent.py        # Agent definition (instructions, model, tools)
├── .env.example        # Required environment variables (no secrets)
├── .gitignore
└── README.md
```

## Getting Started

### Prerequisites

- Python 3.13 (<!-- TODO: confirm the minimum supported version -->)
- An API key for <!-- TODO: Google AI Studio / Vertex AI / other -->

### Installation

```bash
git clone https://github.com/Theshatat/AI-Agent.git
cd AI-Agent

python -m venv venv
# Windows
venv\Scripts\activate
# macOS / Linux
source venv/bin/activate

pip install google-adk
# TODO: add a requirements.txt (run `pip freeze > requirements.txt`) and use:
# pip install -r requirements.txt
```

### Configuration

Copy the example environment file and add your own key:

```bash
cp .env.example .env
```

```env
# TODO: confirm the exact variable names used by your agent
GOOGLE_API_KEY=your_key_here
```

> **Never commit `.env`.** It is listed in `.gitignore`.

### Run

Run these commands from the project root (the folder that contains `blog_agent/`):

```bash
# Web UI for chatting with the agent
adk web

# Or in the terminal
adk run blog_agent
```

## Usage Example

<!-- TODO: show one real input and a trimmed real output.

**Input**
> Write a blog post about ...

**Output**
> (first few lines of the generated post)
-->

## Design Decisions & Limitations

<!-- TODO: 3-4 honest bullets. Examples of what belongs here:
- Why ADK instead of LangChain/n8n
- Why this model
- Known limitations (no fact-checking, no citations, single-turn only, etc.)
This section is what separates a tutorial copy from an engineering project. -->

## Roadmap

- [ ] Add `requirements.txt`
- [ ] Add tests / evaluation cases for agent output
- [ ] <!-- TODO: your next real feature -->

## License

<!-- TODO: choose one (MIT is the common default) and add a LICENSE file. -->

## Author

**Ahmed Shatat** — [GitHub](https://github.com/Theshatat) · [LinkedIn](https://www.linkedin.com/in/ahmed-shatat-45ash50/)
