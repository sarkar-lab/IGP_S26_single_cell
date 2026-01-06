# IGP S26 Single-Cell Quick Start

This repository contains teaching materials for an introductory single-cell RNA-seq (scRNA-seq) practical, built around a quick-start workflow in **Scanpy**.

The main notebook is:

- `week_1/1_Quick_Start_Single_Cell.ipynb`

It is designed so that students can either run it locally (Jupyter/Lab) or directly in **Google Colab**.

## Folder Structure

- `week_1/` – quick-start notebook(s) for Week 1
  - `1_Quick_Start_Single_Cell.ipynb` – primary teaching notebook
- `data/` – (optional) local data files used by the notebooks

Large `.h5ad` and similar data files are ignored by Git via `.gitignore`; students are expected to download data within the notebook or use shared data paths as instructed.

## Running on Google Colab

1. Push this repository to GitHub.
2. Open `week_1/1_Quick_Start_Single_Cell.ipynb` on GitHub and copy its URL.
3. Construct a Colab URL using the pattern:

	`https://colab.research.google.com/github/USERNAME/REPO/blob/main/week_1/1_Quick_Start_Single_Cell.ipynb`

4. Open that URL in your browser. Colab will load the notebook.
5. In the notebook, follow **Step 2** to install required packages, then run cells from top to bottom.

## Running Locally

1. Clone this repository:

	`git clone https://github.com/USERNAME/IGP_S26_single_cell.git`

2. Create and activate a Python environment (e.g. via `conda` or `venv`). For example, with **conda**:

	`conda create -n igp_scenv python=3.10`

	`conda activate igp_scenv`

3. Install packages similar to those used in the teaching environment.

	**Option A (conda-forge preferred):**

	`conda install -c conda-forge scanpy anndata umap-learn python-igraph leidenalg seaborn`

	**Option B (pip):**

	`pip install scanpy anndata umap-learn leidenalg python-igraph gseapy seaborn`

4. Launch Jupyter Lab/Notebook in this directory and open:

	`week_1/1_Quick_Start_Single_Cell.ipynb`

5. Run the notebook from top to bottom, following the numbered steps inside.

## Contributing / Updating

- Edit the notebooks in `week_1/` and re-run them to ensure all cells execute cleanly.
- Avoid committing large `.h5ad` files; instead, add download commands inside the notebooks or document shared paths.
- After changes, commit and push as usual:

  `git add .`

  `git commit -m "Update quick-start notebook"`

  `git push`
