# DIP — Digital Image Processing Notebooks

This repository contains several interactive Jupyter notebooks demonstrating basic to intermediate digital image processing techniques using Python libraries such as Pillow, Mahotas, OpenCV, PyTorch and SciPy.

Contents
- `dip.ipynb`, `scipy.ipynb`, `scipy2.ipynb` — miscellaneous experiments and examples.
- `mahotas/` — notebooks that use the Mahotas library for image filtering and analysis.
- `pillow/` — Pillow (PIL) examples including `comp.ipynb` which compares Pillow and Mahotas results.
- `pytorch/` — PyTorch examples and experiments. Contains an `opencv/` subfolder with OpenCV-related notebooks and images.

Highlights
- `pillow/comp.ipynb` compares edge-detection, object counting and timing between Pillow and Mahotas.
- Notebooks are intended for interactive exploration — open them with Jupyter, run cells, tweak parameters and explore results.

Quick start
1. (Recommended) Create a virtual environment and activate it:

```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1
```

2. Install the required Python packages (example):

```powershell
pip install numpy matplotlib pillow mahotas scikit-image scipy jupyter
```

3. Launch Jupyter Notebook or Lab in the repository root and open the notebook you want to run:

```powershell
jupyter notebook
# or
jupyter lab
```

4. For `pillow/comp.ipynb` specifically:
- Replace the `image_path` variable inside the notebook with the path to an image on your machine (the notebook currently points to a local Downloads path). You can use JPEG/PNG files.
- Run all cells. The notebook will load the image via Pillow and Mahotas, run simple edge detection + thresholding, count connected components, and display comparison plots.

Dependencies
- Python 3.8+ recommended
- numpy
- matplotlib
- pillow
- mahotas
- scikit-image
- scipy

You can install them in one line:

```powershell
pip install numpy matplotlib pillow mahotas scikit-image scipy
```

Notes & troubleshooting
- If a notebook imports a library you don't have installed, install it into the active environment and re-run the kernel.
- Some notebooks read images from hard-coded paths. Update those paths to point to existing images on your machine.
- On Windows you may need to run PowerShell as Administrator to install packages system-wide; using a virtual environment avoids that.

License
This repository is provided as-is for learning and experimentation.

If you'd like a more formal CONTRIBUTING guide or CI setup, tell me what you'd like included and I can add it.