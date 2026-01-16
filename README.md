# Signal Processing: Noise Analysis & Removal (MAF + FFT) in MATLAB

This repository demonstrates signal denoising and analysis using:
- Moving Average Filtering (MAF) with configurable window lengths and passes
- FFT-based denoising using frequency-thresholding
- Evaluation using MSE and MAE
- Time-domain and frequency-domain visualizations

## Project Highlights
- **Signal analysis & segmentation**: time + frequency domain inspection and segmentation into homogeneous regions.
- **MAF denoising**: window sweep + multi-pass filtering; evaluated via MSE/MAE.
- **FFT denoising**: thresholding in the frequency domain to remove separable noise bands.
- **Custom MATLAB functions**: reusable filtering + FFT helpers.
- **Visualization**: plots to show improvements in both domains.
- **Comparison**: when MAF works best vs when FFT works best.

## Repository Structure
- `src/` reusable functions (filters, FFT utilities, metrics, plotting)
- `scripts/` reproducible experiments and comparisons
- `notebooks/` MATLAB Live Scripts (`.mlx`) with narrative + plots
- `data/` sample signals (`signals.mat`)
- `docs/` exported figures + report (optional)

## Quick Start
1. Open MATLAB in the repo root
2. Run:
   - `scripts/compare_maf_vs_fft.m`

## Key Functions
- `src/filters/MAF_filter.m` – Moving average filtering (window length, passes)
- `src/filters/FFTFilter.m` – FFT-based threshold denoising
- `src/metrics/MSE_MAE_Table.m` – compute MSE/MAE across configurations
- `src/viz/PlotFFT.m` – frequency-domain plotting helper

## Results
(Add exported figures in `docs/figures/` and embed them here.)

## Notes
- MATLAB version tested: (fill in)
- Data source: `data/signals.mat`

## License
MIT (or your preferred license)
