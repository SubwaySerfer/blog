# FastAPI Blog with HTMX

A simple and modern blog application built with FastAPI and HTMX. This project demonstrates how to build dynamic web applications with minimal JavaScript using server-side rendering and HTMX for interactivity.

## Features

- Server-side rendered blog posts
- Real-time search with HTMX
- Dynamic content updates without page reloads
- Markdown support for blog posts
- Clean and minimal UI

## Tech Stack

- **FastAPI** - Modern Python web framework
- **HTMX** - Dynamic HTML without JavaScript
- **Jinja2** - Template engine
- **UV** - Fast Python package installer and resolver

## Local Development Setup

1. Clone the repository
```bash
git clone <your-repo-url>
cd fastapi-blog
```

2. Create and activate virtual environment with UV
```bash
uv venv
source .venv/bin/activate  # On Windows use: .venv\Scripts\activate
```

3. Install dependencies
```bash
uv pip install -e ".[dev]"
```

4. Install pre-commit hooks
```bash
pre-commit install
```

5. Run the development server
```bash
uvicorn app.main:app --reload
```

The application will be available at `http://localhost:8000`

## Project Structure
```
blog/
├── app/
│   ├── api/          # Route handlers
│   ├── core/         # Configuration
│   ├── models/       # Pydantic models
│   ├── storage/      # Data storage
│   ├── templates/    # Jinja2 templates
│   └── static/       # CSS and other static files
└── tests/            # Test suite
```

## Testing

Run the test suite:
```bash
pytest
```

## Code Quality

This project uses several tools to maintain code quality:

- **Black** - Code formatting
- **Flake8** - Style guide enforcement
- **MyPy** - Static type checking

These checks run automatically on commit via pre-commit hooks.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes (following our commit message convention)
4. Push to your branch
5. Create a Pull Request

## License

MIT
