
# Blog Writer

A notebook-driven project for generating technical blog drafts using LangGraph and Groq.

## Overview

This project uses a notebook workflow to build a blog planning and writing pipeline:

- router decides if research is needed
- researcher gathers evidence when required
- orchestrator creates a blog outline
- worker writes each section in Markdown
- reducer merges the final output into a `.md` file

It is built around:
- `langgraph`
- `langchain-groq`
- `pydantic`
- `langchain-community` tools

## Files

- `new_file.ipynb` — main notebook with the blog planner pipeline
- `blog.html` — optional demo or output file

## Setup

Install the required Python packages:

```bash
pip install langchain langgraph langchain-groq langchain-community tavily-search python-dotenv pydantic
