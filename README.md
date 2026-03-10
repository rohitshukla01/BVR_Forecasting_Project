<p align="left">
<img alt="License" src="https://img.shields.io/badge/License-MIT-blue.svg">
<img alt="Python" src="https://img.shields.io/badge/Python-3.9%2B-blueviolet">
<img alt="Models" src="https://img.shields.io/badge/Model-XGBoost-4285F4">
<img alt="Framework" src="https://img.shields.io/badge/Framework-Scikit--learn-orange">
<img alt="Framework" src="https://img.shields.io/badge/Visulisation-Matplotlib-green">
<img alt="RStudio" src="https://img.shields.io/badge/RStudio-4285F4?style=flat&logo=rstudio&logoColor=white">
</p>



# Multi-horizon Chlorophyll-a forecasting with XGBoost and SHAP-based explainability for Beaverdam Reservoir (BVR), Virginia.

---

## 📖 About

This project develops a machine learning (ML) framework to **forecast Chlorophyll-a concentrations at 1–7 day horizons** in Beaverdam Reservoir, Virginia, USA. It uses Explainable AI (SHAP) to identify the key environmental drivers at each forecast horizon, and Bootstrap Ensemble methods (evaluated with CRPS) to quantify prediction uncertainty. By combining high-frequency sensor data with meteorological observations, the model uncovers hidden patterns driving phytoplankton dynamics, offering insights for both **water quality management** and **ecological research**.

> *Note: The title will be updated with the publication name upon acceptance.*
---

## 🚀 Getting Started

### Option A: Run on Google Colab (Recommended)

1. Open the colab: https://colab.google/
2. Add the notebook `BVR_Forecasting_XAI_UQ_Review.ipynb`
3. Upload the CSV data file (`BVR_BIO_CHEM_MET_DAILY_2020_2024.csv`) or mount Google Drive
4. Run the notebook cells sequentially

>*Note: It will install the optuna package. Make sure it is uncommented.*

### Option B: Run Locally

```bash
# Clone the repository
git clone https://github.com/rohitshukla01/BVR_Forecasting_Project.git
cd BVR_Forecasting_Project

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate        # Mac/Linux
venv\Scripts\activate           # Windows

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
pip install jupyter
jupyter notebook
```

Open `BVR_Forecasting_review.ipynb` and run all cells sequentially.

---

## 📊 Data Access

The processed daily-averaged dataset is included in this repository as a CSV file `BVR_BIO_CHEM_MET_DAILY_2020_2024.csv`.

To regenerate the data directly from [EDI Repository](https://portal.edirepository.org/nis/home.jsp), run the R script:

**R Script:** [Daily_avg_RS.R](https://github.com/CareyLabVT/Reservoirs/blob/master/Scripts/Daily_avg_RS.R)

This script fetches data packages from the EDI API, processes the variables, and outputs the final CSV.

> *Note: The R script may take several minutes and require substantial memory depending on your system.*

### Data Citations

- Carey, C. C., & Breef-Pilz, A. (2025). Time series of high-frequency meteorological data at Falling Creek Reservoir, Virginia, USA, 2015–2024 (ver. 9). Environmental Data Initiative. https://doi.org/10.6073/pasta/0389840ddcb39ec5526869ac898ddb5d

- Carey, C. C., & Breef-Pilz, A. (2025). Time series of high-frequency sensor data measuring water temperature, dissolved oxygen, conductivity, specific conductance, total dissolved solids, chlorophyll a, phycocyanin, fluorescent dissolved organic matter, and turbidity at discrete depths, and water level in Beaverdam Reservoir, Virginia, USA, 2009–2024 (ver. 5). Environmental Data Initiative. https://doi.org/10.6073/pasta/8f666b34c120aa5d2242964cf3147f90

---


## ✅ Citation & Data Access

📑 If you use this code/data in a publication, please cite this repository/paper and data accordingly. 









