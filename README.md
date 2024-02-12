# duckdb-gnaf
Toy repository to test DuckDB speed on GNAF core dataset

To set up:
- Clone the repository
- Open the repository directory in your terminal
- `python -m venv .venv` (I used Python 3.11. Python 3.12 doesn't work with duckdb until v0.10.0, which is out in a few days)
- `source .venv/bin/activate` on Linux or `.venv/scripts/activate.ps1` on Windows
- `pip install -r requirements.txt`
- Put `GNAF_CORE.psv` in the `data` folder.

The notebook will read the .psv and write to Parquet in the first cell, then query the Parquet for the rest of the cells.