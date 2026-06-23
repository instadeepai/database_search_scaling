# Comparative Framework Database Search

This project provides an interactive scaling analysis for proteomics database search strategies. It uses [marimo](https://marimo.io/) to create a notebook-style web app for exploring how hardware performance and search parameters affect estimated runtimes and memory requirements.

[View the interactive notebook online!](https://molab.marimo.io/github/instadeepai/database_search_scaling/blob/main/database_search_scaling.py)

## Features

- Interactive sliders and input boxes for hardware and search parameters
- Visualizations of asymptotic scaling, memory overhead, and runtime heatmaps
- Figures update automatically as parameters change

## Requirements

- Python 3.12 or newer (see [.python-version](.python-version))
- [marimo](https://marimo.io/) >= 0.15.5
- [matplotlib](https://matplotlib.org/) >= 3.10.6
- [numpy](https://numpy.org/) >= 2.3.3

Dependencies are listed in [pyproject.toml](pyproject.toml).

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/instadeepai/database_search_scaling.git
   cd database_search_scaling
   ```

2. **Install `uv`**

Follow the [official instructions](https://docs.astral.sh/uv/getting-started/installation/).

3. **Create and activate a Python 3.12 environment:**
   ```sh
   uv venv --python 3.12
   source .venv/bin/activate
   ```

4. **Install dependencies with uv:**
   ```sh
   uv sync
   ```

## Running the Interactive App

To launch the interactive notebook, run:

```sh
marimo run database_search_scaling.py
```

This will start a local web server and open the app in your browser. You can adjust parameters and view updated figures interactively.

## Project Structure

- `database_search_scaling.py`: Main marimo app with all interactive cells and visualizations.
- `pyproject.toml`: Project metadata and dependencies.
- `.python-version`: Specifies required Python version.

## License

[Apache 2.0](LICENSE.md)

---

For more details on marimo, see the [marimo documentation](https://marimo.io/docs/).
