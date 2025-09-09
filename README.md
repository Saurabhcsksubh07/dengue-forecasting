# Dengue Outbreak Forecasting

This is **Project 3 given by GUVI – HCL** as part of the Data Analytics learning program.
The project focuses on forecasting dengue cases using statistical models and climate variables.
By predicting dengue outbreaks in advance, health authorities can take preventive measures and reduce the impact on communities.

---

## Objectives

1. Collect and clean dengue and climate data.
2. Convert daily data into weekly summaries for better analysis.
3. Explore the relationship between rainfall, temperature, humidity, and dengue cases.
4. Build an ARIMA model that uses both past cases and climate factors.
5. Forecast dengue cases for the upcoming weeks.

---

## Data Sources

* **Dengue data**: NVBDCP or IDSP reports.
* **Climate data**: IMD or ERA5 datasets.
* Data was preprocessed into weekly form for modeling.

---

## Methodology

1. Data collection and cleaning.
2. Weekly aggregation of dengue and climate data.
3. Correlation study between weather and dengue outbreaks.
4. Model building using ARIMA with external climate inputs.
5. Model validation with RMSE and MAE.
6. Forecasting for the next 12 weeks.

---

## Repository Structure

```
dengue-forecasting/
│
├── data_raw/                        
├── data_processed/                  
├── figures/                         
├── notebooks/                       
├── presentation/                    
│   └── dengue-outbreak-forecasting.pdf
├── .gitignore                       
├── LICENSE                          
├── README.md                        
└── requirements.txt
---

## How to Run

1. Clone the repository:
   `git clone https://github.com/<your-username>/dengue-forecasting.git`

2. Install dependencies:
   `pip install -r requirements.txt`

3. Open and run the notebook:
   `jupyter notebook notebooks/Dengue_Forecasting.ipynb`

4. Outputs available after running:

   * weekly\_national\_summary.csv
   * forecast\_national.csv
   * forecast\_plot.png
   * correlation\_heatmap.png

---

## Results

* Validation RMSE: 10.07
* Validation MAE: 7.96
* Dengue cases rise during monsoon and post-monsoon weeks.
* Rainfall and humidity are strongly related to case surges.
* The ARIMA model provides reasonable short-term forecasts.

---

## Limitations

* Only historical case and climate data were used.
* ARIMA may not capture sudden outbreaks caused by external events.
* District-level granularity is still under development.

---

## Future Scope

* Automating weekly updates with live data.
* Adding district-wise forecasting.
* Creating a dashboard for real-time use by health departments.

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
