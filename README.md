# Machine-Learning-Driven-Prediction-of-Drug-Dissolution-in-Supercritical-CO2-A-Random-Forest-Approach
# About Dataset
This dataset was gathered specifically for my predictive modeling optimization project on drug dissolution in supercritical carbon dioxide (SCCO2). SCCO2 has been found to be the most commonly used supercritical fluid for various applications across scientific research and developments, most especially in Nano-technology. This project focuses on its application to drug formulation and extraction processes during pharmaceutical production. Estimating the solubility of a drug in SCCO2 helps to guide the formulation of the drug for improved drug delivery, especially for anticancer drugs. The dataset consist of experimental measured solubility of drugs over a diversified range of therapeutic classes.

drug - name of drug
temp - operating temperature (K)
press - operating pressure (bar)
mw_drug - molecular weight of drug (g/mole)
mp_drug - melting point of drug (K)
rho_scco2 - density of scco2 (kg/m3)
sol - equilibrium solubility (g/L)
sol_mol_frac - equilibrium solubility in mole fraction

============================================================================
#Introduction

The solubility of pharmaceutical compounds in supercritical fluids, particularly supercritical CO2 (SCCO2), plays a pivotal role in various industrial applications, including drug formulation and delivery. Accurate prediction of solubility, expressed as a mole fraction (sol_mol_frac), under varying thermodynamic conditions such as temperature (temp) and pressure (press), is essential for optimizing these processes. Traditional experimental methods, while reliable, can be time-consuming and resource-intensive.

Machine learning approaches, such as Random Forest Regression, offer a promising alternative by leveraging historical datasets to predict solubility under diverse conditions. In this study, a dataset comprising 2,134 observations of drug solubility, alongside features such as temperature, pressure, molecular weight (mw_drug), and CO2 density (rho_scco2), was analyzed to develop a predictive model for sol_mol_frac. The RandomForestRegressor was employed due to its robustness in handling non-linear relationships and complex interactions between variables.

The model demonstrated strong predictive capabilities, with an R² of 0.982 on the training set and 0.899 on the test set, indicating its effectiveness in capturing the solubility trends. These findings underscore the potential of machine learning to supplement experimental methods in advancing drug solubility research.

**Data Trends and Insights**
**Temperature (temp):**

Range: 303 K to 373.15 K, with a mean of 327.25 K.
Trend: The temperatures are concentrated around the median (328 K), with moderate variability (standard deviation: 14.28 K). This suggests experiments were conducted under typical supercritical CO2 conditions.
Pressure (press):

**Pressure**
Range: 80 bar to 500 bar, with a mean of 239.01 bar.
Trend: Pressure varies widely, indicating a diverse set of experimental conditions, but the median (243 bar) shows experiments tend to cluster around moderate pressures.
Molecular Weight of Drug (mw_drug):

**Moleular Weight**
Range: 96 to 853.91 g/mol, with a mean of 323.28 g/mol.
Trend: A broad range of molecular weights highlights the inclusion of a wide variety of drugs, with the median (289.38 g/mol) skewed slightly toward smaller molecules.
Melting Point of Drug (mp_drug):
**Melting Point**
Range: 115 K to 608.15 K, with a mean of 406.09 K.
Trend: Moderate variability (standard deviation: 105.28 K) suggests a mix of low and high-melting-point drugs, with many clustered around the median (431.15 K).
Density of SCCO2 (rho_scco2):

**Density**
Range: 3.46 kg/m³ to 992 kg/m³, with a mean of 743.58 kg/m³.
Trend: The density spans a large range, reflecting the impact of pressure and temperature on CO2 density. Most values are concentrated above 690 kg/m³, indicative of typical SCCO2 densities.
Solubility in mg/L (sol):
**Sol**
Range: 0 to 43.8 mg/L, with a mean of 2.07 mg/L.
Trend: Highly skewed distribution, as the 75th percentile (1.31 mg/L) is far below the maximum (43.8 mg/L). This suggests a few drugs exhibit exceptionally high solubility, while most remain at low solubility levels.
Solubility in Mole Fraction (sol_mol_frac):

**Mole fraction solubility**

Range: 0 to 0.021, with a mean of 0.000371.
Trend: Mole fraction solubility is extremely low across the dataset. The highly skewed data distribution (median: 0.000054) suggests that only a few instances reach higher solubility.

======================================================================================

**Conclusion**
This study highlights the utility of machine learning, specifically the RandomForestRegressor, in predicting drug solubility in SCCO2 systems. Using temperature and pressure as primary predictors, the model achieved high accuracy, as evidenced by an R² of 0.899 on the test set. The results suggest that this model can serve as a reliable tool for estimating sol_mol_frac, thereby reducing the dependency on exhaustive experimental procedures.

While the model performed well, the Mean Squared Error (MSE) on the test set (642.19) indicates potential areas for improvement, such as the inclusion of additional features (e.g., rho_scco2, mw_drug) or hyperparameter tuning. Future work could also explore the incorporation of advanced machine learning techniques and domain-specific feature engineering to further enhance predictive accuracy.

By leveraging machine learning, this research provides a framework for efficient solubility prediction, paving the way for optimized experimental designs and cost-effective drug formulation strategies.


