# WREF Snag Detection — UNet Threshold Sweep Dashboard
 
Interactive results dashboard for a UNet-based snag detection threshold sweep across 123 models (3ch, 4ch, and 5ch variants) using CHM and intensity thresholds from 5–100%. Evaluated on n=58 validation chips from the Wind River Experimental Forest (WREF). Displays per-model SnagMAE, SnagR², RMSE, bias, and slope fit, with filtering and sorting by channel configuration.
 
> **Best performing model:** `4ch_rgb_chm_055` — SnagMAE 24.94, −22.7% vs baseline (4ch RGB+NIR)
 
---
 
## Model Variants
 
| Type | Description |
|------|-------------|
| `4ch RGB+CHM` | RGB + Canopy Height Model |
| `4ch RGB+INT` | RGB + Intensity |
| `4ch CIR+CHM` | Color Infrared + Canopy Height Model |
| `4ch CIR+INT` | Color Infrared + Intensity |
| `3ch RGB` | RGB only |
| `3ch CIR` | Color Infrared only |
| `4ch RGB+NIR` | RGB + Near Infrared (baseline) |
 
## Metrics
 
- **SnagMAE** — Mean Absolute Error on snag predictions (primary metric)
- **SnagR²** — R² score on snag predictions
- **SnagRMSE** — Root Mean Squared Error on snag predictions
- **SnagBias** — Signed bias on snag predictions
- **Slope** — Regression slope fit (ideal = 1.0)
---
 
*Part of ongoing research — not yet published.*
