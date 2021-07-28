## Predicting bloodstream infection outcome using machine learning 
From the manuscript titled: [**Predicting bloodstream infection outcome using machine learning** by: Yazeed Zoabi, Orli Kehat, Dan Lahav, Ahuva Weiss-Meilek, Amos Adler, Noam Shomron](https://www.medrxiv.org/content/10.1101/2021.05.18.21257369v1), medRxiv; [doi:10.1101/2021.05.18.21257369](https://doi.org/10.1101/2021.05.18.21257369)

## Model Predictors and their respective units
* **RDW** - (%)
* **Albumin** - (g/L)
* **Age** - Age in years
* **Creatinine** - (mg/dL)
* **RBC** - (10e6/ϻL)
* **Surgery** - True = 1, False = 0
* **NRBC/100_WBC** - (%)
* **Mean_platelet_volume** - (fL)
* **AST** - (U/L)
* **HCT** - (%)
* **MCHC** - (g/dL)
* **Indirect_Bilirubin** - (mg/dL)
* **Cerebrovascular_disease** - True = 1, False = 0
* **Alkaline** - (U/L)
* **Platelet_Automated_Count** - (10e3/ϻL)
* **MCV** - (fL)
* **Catheterization** - True = 1, False = 0
* **Respiratory_diseases** - True = 1, False = 0
* **Direct_bilirubin** - (mg/dL)
* **ALT** - (U/L)
* **Sex** - Male=1, Female=0
* **Lymphocytes** - (10e3/ϻL)
* **Neutrophils** - (10e3/ϻL)
* **Infectious_background** - True = 1, False = 0
* **Insulin** - True = 1, False = 0


## Model Outcome
The probability of having the composite outcome as defined by the manuscript.


## Use
1. Import lgbm_compact_model.txt using LightGBM 2.3.1 on Python 3.6.

2. Predict using your data.

## Files in this repository

* **lgbm_compact_model.txt** - The compact model that uses 25 features
* **hyperparameters.txt** - The hyperparameters used by LightGBM to train the inclusive and the compact model
