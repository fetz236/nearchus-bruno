# nearchus-bruno

Bruno Collection :D

## Setup

This project uses [uv](https://github.com/astral-sh/uv) for package management.

### Installation

1. Install uv (if not already installed):

   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

2. Sync dependencies (creates virtual environment and installs all dependencies):

   ```bash
   uv sync
   ```

   This will automatically:

   - Create a virtual environment (if it doesn't exist)
   - Install the project and all development dependencies
   - Generate a lock file (`uv.lock`)

### Development

You can run commands using `uv run` (which automatically uses the project's virtual environment):

- Run tests:

  ```bash
  uv run pytest
  ```

- Format code:

  ```bash
  uv run ruff format .
  ```

- Lint code:

  ```bash
  uv run ruff check .
  ```

- Run the package:
  ```bash
  uv run python -m nearchus_bruno
  ```

Alternatively, you can activate the virtual environment manually:

```bash
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```
