# code-scanner

[![CI](https://img.shields.io/github/actions/workflow/status/user/code-scanner/ci.yml?branch=main)]()
[![Python](https://img.shields.io/badge/python-3.11+-blue.svg)]()
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

Static code scanner for security vulnerabilities and anti-patterns — designed for production workloads with a focus on reliability and developer ergonomics.

## Features

- Minimal Dependencies: Only standard library dependencies for core features
- Async Support: Native asyncio integration with sync fallback
- Rich CLI: Interactive CLI with colored output and progress bars
- Plugin Architecture: Extensible design with entry-point based plugins

## Installation

```bash
pip install code-scanner
# or
pipx install code-scanner
```

## Quick Start

```python
from code_scanner import Client

client = Client(
    timeout=30,
    retries=3,
)

result = client.run()
print(result)
```

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
