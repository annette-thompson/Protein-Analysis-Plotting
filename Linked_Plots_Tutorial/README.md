# Linked plots: click a point, see the structure

Examples of interactive analysis plots for MD trajectories. Each plot sits next to a 3D viewer, and clicking a
point jumps the viewer to that frame and highlights the atoms behind it. The examples cover time series, 2D
scatter, event rasters, an UpSet plot, a Ramachandran plot, a free-energy landscape, cluster bars, per-residue
bars and a heatmap. Analysis uses MDAnalysis, plots use plotly, and the viewer is nglview.

The example system (a kinase with a bound peptide, ATP and Mg²⁺) is only there to have something to look at. The
end of the notebook explains how to adapt it and gives a prompt for asking Claude to build the same kind of
notebook for a different project.

## Setup

```
conda env create -f environment.yml
```

Open `tutorial.ipynb` with the `viztutorial` kernel (VS Code or JupyterLab). Clicks need a live kernel.

## Files

| File | What it is |
|---|---|
| `tutorial.ipynb` | The examples |
| `data/md.tpr`, `data/md_full.xtc` | Example topology and trajectory (all atoms, 200 frames, 1.5 ns apart, 33 MB) |
| `environment.yml` | Conda environment |
