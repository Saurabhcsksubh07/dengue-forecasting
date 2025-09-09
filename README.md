# Dengue Outbreak Forecasting

This project was developed as **Project 3 under the GUVI – HCL Data Analytics Program**.  
It focuses on forecasting dengue cases using statistical models and climate variables.  
By predicting outbreaks in advance, health authorities can plan preventive measures and reduce the impact on communities.

---

**Objectives**

1. Collect and clean dengue and climate data.  
2. Convert daily records into weekly summaries for analysis.  
3. Study the relationship between rainfall, temperature, humidity, and dengue cases.  
4. Build an ARIMA model that leverages both past cases and climate factors.  
5. Forecast dengue cases for the upcoming weeks.  

---

**Data Sources**

- **Dengue data**: NVBDCP or IDSP reports.  
- **Climate data**: IMD or ERA5 datasets.  
- Data was preprocessed into weekly form for modeling.  

---

**Methodology**

1. Data collection and cleaning.  
2. Weekly aggregation of dengue and climate data.  
3. Correlation analysis between climate factors and dengue outbreaks.  
4. Model building using ARIMA with external climate inputs.  
5. Model validation using RMSE and MAE.  
6. Forecasting dengue cases for the next 12 weeks.  

---

**Repository Structure**



dengue-forecasting/
│
├── data\_raw/
├── data\_processed/
├── figures/
├── notebooks/
├── presentation/
│   └── dengue-outbreak-forecasting.pdf
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt

`

---

**How to Run**

1. Clone the repository:  
   bash
   git clone https://github.com/<your-username>/dengue-forecasting.git
`

2. Install dependencies:

   bash
   pip install -r requirements.txt
   

3. Open and run the notebook:

   bash
   jupyter notebook notebooks/Dengue_Forecasting.ipynb
   

4. Outputs generated after running:

   * `weekly_national_summary.csv`
   * `forecast_national.csv`
   * `forecast_plot.png`
   * `correlation_heatmap.png`

---

**Results**

* Validation RMSE: **10.07**
* Validation MAE: **7.96**
* Dengue cases increase during monsoon and post-monsoon weeks.
* Rainfall and humidity are strongly correlated with case surges.
* The ARIMA model provides reliable short-term forecasts.

---

**Limitations**

* Only historical case and climate data were considered.
* ARIMA may not capture sudden outbreaks triggered by external factors.
* District-level forecasting is still under development.

---

**Future Scope**

* Automating weekly updates with live data sources.
* Incorporating district-level forecasting.
* Developing an interactive dashboard for health departments.

---

## Conclusion

This project helped in understanding how **climate factors** influence dengue outbreaks.
By applying ARIMA with weather variables, short-term forecasts can be generated that may support public health decision-making.
Although improvements are possible, this project demonstrates a strong link between climate and dengue cases and provides a base for further research.

---

## Project Evaluation Note

This work was submitted as **Project 3 under GUVI – HCL program** for academic evaluation.
It reflects both the technical learning and practical application of forecasting methods in public health.

---

## Author

Saurabh Rai
B.Sc. Computer Science and Data Analytics
IIT Patna
