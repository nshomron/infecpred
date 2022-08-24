## Predicting bloodstream infection outcome using machine learning 

[Scientific Reports](https://www.nature.com/articles/s41598-021-99105-2) | [medRxiv](https://www.medrxiv.org/content/10.1101/2021.05.18.21257369v1) | [PDF](https://www.nature.com/articles/s41598-021-99105-2.pdf)

[Yazeed Zoabi](https://yazeedzoabi.com)<sup>1,†</sup>, Orli Kehat<sup>2,†</sup>, [Dan Lahav](https://www.dlahav.com/)<sup>1</sup>, Ahuva Weiss-Meilik<sup>2,‡</sup>, Amos Adler<sup>2,‡</sup>, [Noam Shomron](https://nshomron.github.io/)<sup>1,‡</sup><br />
<sup>1</sup> Tel Aviv University<br>
<sup>2</sup> Tel-Aviv Sourasky Medical Center<br>
<sup>†</sup>These authors contributed equally<br>
<sup>‡</sup>These authors jointly supervised this work

*Among the implications of this work is implementation of the models as a basis for selective rapid microbiological identifcation, toward earlier administration of appropriate antibiotic therapy. Additionally, our models may help reduce the development of BSI and its associated adverse health
outcomes and complications.*

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
