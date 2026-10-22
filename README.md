# Wealth, Longevity & Carbon

This project contains a Jupyter notebook analyzing the relationship between
wealth, longevity, and carbon emissions. The notebook includes the calculations
and charts behind the accompanying nine-slide presentation.

## Project files

- `Wealth_Longevity_Carbon_Concise.ipynb` — analysis notebook
- `worlddata.csv` — required data file; excluded from Git because it exceeds
  GitHub's 100 MB file limit
- `Wealth_Longevity_Carbon_Concise.pptx` — companion presentation
- `requirements.txt` — Python packages needed to run the notebook

## Run the notebook locally

You need Python 3.10 or newer and Git.

1. Clone the repository and enter its directory:

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Create and activate a virtual environment:

   **macOS/Linux**

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

   **Windows PowerShell**

   ```powershell
   py -m venv .venv
   .venv\Scripts\Activate.ps1
   ```

3. Install the dependencies and start JupyterLab:

   ```bash
   python -m pip install --upgrade pip
   python -m pip install -r requirements.txt
   jupyter lab
   ```

4. Open `Wealth_Longevity_Carbon_Concise.ipynb` in JupyterLab and choose
   **Run → Run All Cells**. Run it from the cloned project directory so the
   notebook can find `worlddata.csv`.

The data file is not included in the repository. Get `worlddata.csv` from the
project owner and place it in the project directory beside the notebook before
running it. A download link can be added here when available.

The notebook saves charts and analysis tables under
`outputs/concise_analysis/`. These files are generated when you run the
notebook.

Randomized analysis steps use the fixed seed `704`. This makes those steps
repeatable with the same data and software environment; exact numerical output
is not guaranteed across different Python, library, or platform versions.

## Run in Google Colab

Upload the notebook to Colab and run all cells. When prompted, upload
`worlddata.csv`; obtain the file from the project owner first.
