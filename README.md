# Machine Learning: Weekly Challenges

Solutions to the weekly challenges from the **Machine Learning** course (code 81610) at the [University of Bologna](https://www.unibo.it), taught by Prof. Davide Maltoni, academic year 2026/2027.

📚 [Course page](https://www.unibo.it/it/studiare/insegnamenti-competenze-trasversali-moocs/insegnamenti/insegnamento/2026/559021)

## Repository structure

Each week's challenge has its own folder:

```
.
├── Week1Chall/
│   ├── <notebook>.ipynb    # Challenge solution
│   └── <dataset files>     # Dataset, when provided
├── Week2Chall/
│   └── ...
├── ...
├── requirements.txt        # Python dependencies
└── README.md
```

- **`Week<N>Chall/`**: one folder per weekly challenge.
- **Notebook**: a Jupyter notebook with the solution to that week's challenge.
- **Dataset**: usually included in the folder next to the notebook.
- **`requirements.txt`**: all packages needed to run the notebooks (Jupyter kernel and ML libraries).

## Environment setup

### Prerequisites

- Python 3.10 or newer
- `git`

### 1. Clone the repository

```bash
git clone <repository-url>
cd <repository-folder>
```

### 2. Create a virtual environment

**Linux / macOS**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

**Windows (PowerShell)**
```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Register the Jupyter kernel (optional)

This makes the environment selectable from VS Code, JupyterLab, etc.

```bash
python -m ipykernel install --user --name ml-course --display-name "Python (ml-course)"
```

### 5. Launch Jupyter

```bash
jupyter lab
# or
jupyter notebook
```

Open a notebook from one of the `Week<N>Chall/` folders and select the **Python (ml-course)** kernel.

> **Tip:** Run notebooks from within their own folder so relative dataset paths resolve correctly.

Or in vsCode via the jupyter extension.

### Using conda instead

```bash
conda create -n ml-course python=3.11
conda activate ml-course
pip install -r requirements.txt
```

## Running a challenge

1. Activate the environment (`source .venv/bin/activate`).
2. Start Jupyter and open `Week<N>Chall/<notebook>.ipynb`.
3. Run all cells (**Kernel → Restart & Run All**).

## Course topics

Supervised and unsupervised learning, classification and regression (Bayes, k-NN, SVM, ensembles), clustering (K-means, EM), dimensionality reduction (PCA, DA), neural networks, deep learning, CNNs, RNNs, Transformers and LLMs, and reinforcement learning.

Course tools: scikit-learn, TensorFlow, PyTorch.

## Notes

Course materials and exercise texts are available on the instructor's page: <http://bias.csr.unibo.it/maltoni/ml>