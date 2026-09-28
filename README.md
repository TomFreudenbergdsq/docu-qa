# docu-qa

Ask questions over my notes folder

Side project, maintained when I have time.

## Features

- Swap in any LLM for the answer step
- Prints sources with scores for transparency
- TF-IDF retrieval: zero external services needed
- Chunk markdown with overlap, keep source paths

## Getting started

```bash
pip install -r requirements.txt
```

## Examples

```bash
python rag.py ./notes "how do I rotate logs?"
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── workflows/
│       └── ci.yml
├── data/
│   └── sample.md
├── docs/
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── rag.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
