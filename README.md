# Optical Flow for Scratch Wound Analysis

An image processing pipeline that uses optical flow to analyse scratch wound (wound healing) assays from microscopy time series. It extracts cell boundaries, tracks their movement over time, and quantifies how cells migrate into the wound area.

## What it measures

- Speed of cell movement
- Directionality of movement
- Persistence of movement over time

Together these give a quantitative picture of cell migration dynamics during wound closure, instead of a single end point measurement of wound area.

## Contents

- `optical_flow_scratch_wound_analysis.ipynb` - the main notebook: the full pipeline from time series images to migration measurements
- `motion_analysis.py` - motion tracking over the image sequence
- `magnitude_analysis.py` - magnitude of movement
- `orientation_analysis.py` - orientation and directionality analysis
- `polar_plots.py` - polar plots of movement direction and distribution

## How to run

Open the notebook in Jupyter and run it against your own scratch assay time series images. The four Python modules are imported by the analysis code and can also be used individually.

Requirements: Python with NumPy, OpenCV, and Matplotlib (with Jupyter for the notebook).

## Notes

- No microscopy data is included in this repository.
- These modules are the cleaned up versions of analysis code developed during postdoctoral bioimaging work at Durham University.
