# mcp-notes-server

MCP server template I base new tools on

## Highlights

- Includes Claude Desktop config snippet
- Three tools: add / get / list notes
- State persisted to a JSON file in the home dir
- FastMCP style: decorators, zero boilerplate

## Usage

```bash
# claude_desktop_config.json
# {
#   "mcpServers": {
#     "notes-box": {"command": "python", "args": ["server.py"]}
#   }
# }
python server.py
```

## Install

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   ├── dependabot.yml
│   └── pull_request_template.md
├── docs/
│   ├── configuration.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── Makefile
├── requirements.txt
└── server.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT. Do whatever you want.
