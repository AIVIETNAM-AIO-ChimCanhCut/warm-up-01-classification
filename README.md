# AIO-2026-WARMUP

A modular machine learning project designed for high-performance experimentation and reproducible research. This project leverages `uv` for dependency management, ensuring fast, deterministic builds and a clean development environment.

## 🚀 Getting Started

### Prerequisites
You will need [uv](https://github.com/astral-sh/uv) installed to manage the environment and dependencies.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd AIO-2026-WARMUP
    ```

2.  **Sync the environment:**
    This command creates a virtual environment (`.venv`), installs the required dependencies from `uv.lock`, and installs the project in editable mode[cite: 1].
    ```bash
    uv sync
    ```

## 📂 Project Structure

Following the modern **src-layout**, the project is organized as follows[cite: 1]:
```text
├── data/               # Local data storage (ignored by git)[cite: 1]
├── models/             # Saved model weights, checkpoints, and artifacts[cite: 1]
├── notebooks/          # Jupyter notebooks for EDA and prototyping[cite: 1]
├── src/                # Core logic and package source code[cite: 1]
├── tests/              # Unit and integration tests[cite: 1]
├── main.py             # Primary entry point for execution[cite: 1]
├── pyproject.toml      # Project configuration and dependencies[cite: 1]
├── uv.lock             # Deterministic dependency lockfile[cite: 1]
└── .python-version     # Specified Python version for the project[cite: 1]
```

## 🛠 Usage

### Running the Project
Execute the main script within the managed environment:
```bash
uv run main.py
```

### Development Workflow
*   **Add a dependency**: `uv add <package>`
*   **Remove a dependency**: `uv remove <package>`
*   **Interactive development**: Select the `.venv` directory as your interpreter/kernel in VS Code or Jupyter[cite: 1].