# AIO-2026-WARMUP

A warm-up machine learning project for AIO2026, focusing on . This project leverages `uv` for dependency management.

## Getting Started

### Prerequisites
You will need [uv](https://github.com/astral-sh/uv) installed to manage the environment and dependencies.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd AIO-2026-WARMUP
    ```

2.  **Sync the environment:**
    This command creates a virtual environment (`.venv`), installs the required dependencies from `uv.lock`, and installs the project in editable mode.
    ```bash
    uv sync
    ```

## Project Structure

Following the modern **src-layout**, the project is organized as follows:
```text
├── data/               # Local data storage (ignored by git)
├── models/             # Saved model weights, checkpoints, and artifacts
├── notebooks/          # Jupyter notebooks for EDA and prototyping
├── src/                # Core logic and package source code
├── tests/              # Unit and integration tests
├── main.py             # Primary entry point for execution
├── pyproject.toml      # Project configuration and dependencies
├── uv.lock             # Deterministic dependency lockfile
└── .python-version     # Specified Python version for the project
```

## Usage

### Running the Project
Execute the main script within the managed environment:
```bash
uv run main.py
```

### Development Workflow
*   **Add a dependency**: `uv add <package>`
*   **Remove a dependency**: `uv remove <package>`
*   **Interactive development**: Select the `.venv` directory as your interpreter/kernel in VS Code or Jupyter.