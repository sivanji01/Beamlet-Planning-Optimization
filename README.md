# Radiotherapy Beamlet Planning with Constrained Optimization

A compact Python project exploring constrained optimization in a simplified radiotherapy beamlet model.

## Project overview

Two non-negative beamlet intensities are selected to meet a target-dose requirement while respecting dose limits for two nearby organs at risk (OARs). The notebook compares:

- A strictly convex quadratic objective solved with SciPy SLSQP.
- A linear objective solved with SciPy's HiGHS linear-programming solver.
- Feasibility checks and 2D/3D visualizations of the solution.

## Files

- `beamlet_planning_optimization.ipynb` — complete, executable notebook with explanations, code, results and plots.
- `requirements.txt` — Python dependencies.
- `.gitignore` — excludes common temporary files.

## Run locally

Python 3.10+ is recommended.

```bash
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt
jupyter notebook
```

Open `beamlet_planning_optimization.ipynb` and run all cells.

## Model and safety note

This is a synthetic, educational two-beamlet optimization example with arbitrary dose units and fixed coefficients. It is **not** a clinical radiotherapy planning system and must not be used to make treatment decisions.

## Concepts demonstrated

Convexity, Hessians, feasible regions, constrained nonlinear optimization, linear programming, dose constraints, numerical validation, and visualization.

## Acknowledgement

The project develops mathematical optimization concepts encountered in biomedical engineering coursework into a standalone learning example. The notebook is independently organized and documented; it is not the original university exercise template.
