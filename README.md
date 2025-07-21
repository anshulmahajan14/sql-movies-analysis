# IMDB Movies SQL Analysis

Explore and analyze the top 250 IMDB movies using SQL with DuckDB and Python. Results are presented in an interactive report using Quarto and [itables](https://mwouts.github.io/itables/).

## Features

- SQL-based data analysis with DuckDB
- Interactive tables using `itables`
- Report built with Quarto (`.qmd`)
- Lightweight and reproducible environment setup

## Installation

1. Clone the repository:

```bash
git clone https://github.com/anshulmahajan14/sql-movies-analysis
cd imdb-sql-analysis
```

2. Create a virtual environment and install dependencies using [`uv`]
```bash
uv venv
source .venv/bin/activate  # or .venv\Scripts\activate on Windows
uv pip install -r pyproject.toml
```

## Usage

To render the Quarto notebook as HTML:

```bash
quarto render notebook.qmd
```

Or open it interactively in Jupyter:

```bash
quarto preview notebook.qmd
```

## Dataset

The SQLite database `movies.db` should be placed inside the `data/` folder. It must contain a `movies` table with the following columns:

title, director, year, rating, genres,runtime, country, language,imdb_score, imdb_votes, metacritic_score
## License

MIT License
