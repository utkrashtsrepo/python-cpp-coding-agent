# Python C++ Coding Agent

A command-line coding agent that uses an LLM to interpret bug reports, locate relevant C++ code, propose targeted edits, and verify fixes through compilation and tests.

## Features

- Interprets natural-language bug reports.
- Searches project files and locates relevant code with line numbers.
- Applies targeted edits instead of rewriting entire files.
- Compiles and tests proposed fixes.
- Limits repair attempts and rolls back changes if verification fails.

## Tech Stack

- Python
- LLM API
- C++
- Tool Calling
- Compiler and test-based verification

## How It Works

1. The user provides a bug report in natural language.
2. The agent searches the codebase for relevant files and code.
3. The LLM proposes a targeted code change.
4. The agent applies the change and runs compilation or tests.
5. If verification fails, it retries within a bounded limit and restores the original code if necessary.

## Setup

Clone the repository:

```bash
git clone https://github.com/your-username/python-cpp-coding-agent.git
cd python-cpp-coding-agent
