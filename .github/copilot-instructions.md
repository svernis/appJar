# Copilot Instructions for appJar

## Project Overview
**appJar** is a Python tkinter GUI wrapper library designed to simplify GUI development, especially for educational use. It wraps tkinter widgets and provides a simpler, more consistent API.

- **Main module**: `appJar/appjar.py`
- **Language**: Python 2.7 / Python 3.x compatible
- **License**: Apache 2.0

## Code Style
- Follow PEP 8 for Python code.
- Maintain Python 2.7 and Python 3 compatibility (avoid Python 3-only syntax unless the codebase has already dropped Python 2 support).
- Use camelCase for method names to stay consistent with the existing appJar API convention.
- Keep public API methods simple and beginner-friendly — this library targets classroom/educational use.

## Architecture
- All GUI widgets and logic live in `appJar/appjar.py`.
- Helper/utility libraries are in `appJar/lib/`.
- Tests are in `tests/`.
- Examples are in `appJar/examples/` and `examples/`.

## Testing
- Run tests with: `python -m pytest tests/` or `python -m unittest discover tests/`
- Keep test coverage high; new features should include tests.

## Key Conventions
- Widget add/set/get methods follow the pattern: `addWidget(title, ...)`, `setWidget(title, value)`, `getWidget(title)`.
- Always check for tkinter availability and handle import errors gracefully for headless environments.
- Do not introduce new third-party dependencies without a strong justification.
