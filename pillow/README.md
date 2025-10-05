# Pillow examples — DIP/pillow

This folder contains Jupyter notebooks that demonstrate image processing using the Pillow (PIL) library and comparisons with other libraries.

Files
- `comp.ipynb` — Compares Pillow and Mahotas for edge detection, binary thresholding, connected component counting, and timing. The notebook:
  - Loads an image using Pillow and Mahotas.
  - Applies an edge detection filter (Pillow's FIND_EDGES and Mahotas' sobel).
  - Uses Otsu thresholding to create a binary image.
  - Counts connected components and records execution time.
  - Plots a comparison matrix (number of objects, execution time, accuracy placeholder, and image sizes).

How to run
1. Open a terminal in the `pillow/` folder and start Jupyter Notebook or Jupyter Lab:

```powershell
jupyter notebook
# or
jupyter lab
```

2. Open `comp.ipynb` and edit the `image_path` variable near the bottom of the notebook to point to a valid local image. For example:

```python
image_path = r"C:\path\to\your\image.jpg"
```

3. Run the cells sequentially. The notebook will display bar charts comparing the two libraries.

Notes & improvements
- The notebook currently sets `accuracy_pillow` and `accuracy_mahotas` to 100 as placeholders. If you have ground-truth object counts, set these values to compute actual accuracy.
- The notebook expects grayscale images but will convert color images to grayscale where needed. If input images are already binary or single-channel, adjust preprocessing steps accordingly.
- Consider adding error handling for missing image files and invalid paths.

Dependencies
- pillow
- mahotas
- numpy
- matplotlib
- scipy
- scikit-image

Install them via pip if needed:

```powershell
pip install pillow mahotas numpy matplotlib scipy scikit-image
```

Contact
If you'd like help improving the notebook (e.g., add ground-truth evaluation, save plots to disk, or standardize inputs), tell me what you want and I can update the notebook.