# A123-LFP-Battery-Multimodal-Electrochemical-Dataset

Multimodal electrochemical characterization raw dataset for 71 A123-type LiFePO₄ (LFP) batteries, covering charge–discharge cycling, cyclic voltammetry (CV), electrochemical impedance spectroscopy (EIS), incremental capacity analysis (ICA), and potentiostatic intermittent titration technique (PITT).

## Dataset Overview

| Item | Description |
|------|-------------|
| **Battery type** | A123-type LiFePO₄ (LFP) |
| **Number of cells** | 71 (Cell 1 – Cell 71) |
| **Test categories** | Charge–discharge, CV, EIS, ICA, PITT |
| **Summary file** | `Statistics.xlsx` |

## Directory Structure

```
raw_data/
├── Char-dis-data/          # Charge–discharge cycling data
│   ├── Char-dis-Cell1.xlsx
│   ├── Char-dis-Cell2.xlsx
│   └── ... (71 files, Cell 1–71)
├── Cyclic voltammetry/     # Cyclic voltammetry (CV) data
│   ├── A123-CV-1.txt
│   ├── A123-CV-2.txt
│   └── ... (71 files, Cell 1–71)
├── EIS/                    # Electrochemical impedance spectroscopy data
│   ├── A123-EIS-1.txt
│   ├── A123-EIS-2.txt
│   └── ... (71 files, Cell 1–71)
├── ICA/                    # Incremental capacity analysis data
│   ├── ICA-Cell1.xlsx
│   ├── ICA-Cell2.xlsx
│   └── ... (71 files, Cell 1–71)
├── PITT/                   # Potentiostatic intermittent titration technique data
│   ├── PITT-Cell1.xlsx
│   ├── PITT-Cell2.xlsx
│   └── ... (71 files, Cell 1–71)
├── Statistics.xlsx         # Summary performance metrics for all cells
└── README.md
```

## File Descriptions

### 1. Charge–Discharge Data (`Char-dis-data/`)

- **Format:** `.xlsx`
- **Naming:** `Char-dis-Cell{N}.xlsx` (N = 1–71)
- **Content:** Voltage, current, capacity, and time-series data recorded during galvanostatic charge–discharge cycling for each cell.

### 2. Cyclic Voltammetry (`Cyclic voltammetry/`)

- **Format:** `.txt`
- **Naming:** `A123-CV-{N}.txt` (N = 1–71)
- **Content:** Current–voltage profiles acquired by scanning the electrode potential at a controlled rate, used to identify redox peaks and electrochemical reaction kinetics.

### 3. Electrochemical Impedance Spectroscopy (`EIS/`)

- **Format:** `.txt`
- **Naming:** `A123-EIS-{N}.txt` (N = 1–71)
- **Content:** Impedance spectra (real and imaginary components) measured over a range of frequencies, used to characterize internal resistance and charge-transfer processes.

### 4. Incremental Capacity Analysis (`ICA/`)

- **Format:** `.xlsx`
- **Naming:** `ICA-Cell{N}.xlsx` (N = 1–71)
- **Content:** dQ/dV vs. voltage curves derived from charge–discharge data, used to track phase-transition peaks and diagnose degradation mechanisms.

### 5. Potentiostatic Intermittent Titration Technique (`PITT/`)

- **Format:** `.xlsx`
- **Naming:** `PITT-Cell{N}.xlsx` (N = 1–71)
- **Content:** Current transient responses to stepwise voltage pulses, used to determine lithium-ion diffusion coefficients within the electrode.

### 6. Statistics Summary (`Statistics.xlsx`)

- **Format:** `.xlsx`
- **Content:** Aggregated performance metrics for all 71 cells, including capacity, internal resistance, and open-circuit voltage (OCV).

## Usage Notes

- All 71 cells underwent the same set of electrochemical tests; each subfolder contains exactly one file per cell.
- `.xlsx` files can be opened with Microsoft Excel, LibreOffice Calc, or read programmatically via Python (`openpyxl`, `pandas`).
- `.txt` files are tab- or comma-delimited and can be loaded directly with `pandas.read_csv()` or similar tools.

## License

Please cite the associated publication if you use this dataset in your research.

## Contact

For questions regarding this dataset, please contact the corresponding author of the associated publication.
