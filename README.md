# Evaluating Re-identification Risk in De-identified Health datasets
## Project Overview
In the healthcare ecosystem, the ability to share data for research is often difficult due to the highly sensitive nature and HIPAA law to protect patient privacy. By simulating a Real-World Data (RWD) scenario, I evaluate how de-identification via multiplicative noise affects the validity of clinical interaction effects while measuring the mitigation of linkage attack risks.

## Tech Stack
- Programming/Scripting Languages: Python
- Python Libraries: SciPy, Statsmodels, Pandas, NumPy, Matplotlib
- IDE: PyCharm
- Documentation: Markdown via Jupyter Notebook (.ipynb)

## Methodology and Reproduction
The [initial_test_report.ipynb](initial_test_report.ipynb) notebook was designed to as a report to document the code and methodology for reproducibility.

## Professional Growth
- Identify probability distribution that match the simulated features, age and hospital length of stay.
- Explored additive and multiplicative noise differential privacy mechanisms to determine what logically matches the simulated features once the noise is applied.
- Researched differential privacy concepts.

## Future Insights
The project goal to simulate a "Real-World Data" (RWD) scenario to assess whether a de-identified health dataset remains statistically representative of the population while measuring the risk of a "linkage attack" (re-identification) was achieved. Positivity of features/attributes were preserved and bias towards zero was minimized by utilizing multiplicative noise instead of clipping additive noise. This project can be improved by simulating hospital length of stay data using Negative Binomial regression, zero-inflated Poisson (ZIP) or zero-inflated generalized Poisson (ZIGP). Additionally, this project can be expanded by simulating more sensitive features and exploring more differential privacy techniques. In summary, the dataset remained valid for secondary analysis and resistant to re-identification.

## Progress
### Completed
- [x] Simulate sensitive RWD (hospital length of stay and age)
- [x] Set up an initial A/B test (5 vs 7 day hospital length of stay)
- [x] Apply privacy noise to simulated patient data. 
- [x] Hypothesis testing: The statistical utility was preserved despite the privacy measures.
- [x] Evaluate the model against range of privacy levels to determine when a Type II error occurs.
- [x] Produce privacy vs utility trade-off visualization.
- [x] Simulate a linkage attack (re-identification risk) by uniqueness.
### In-Progress
- [ ] Set up an interesting A/B test (drug vs placebo) with simulated data.
### To-Do 
- [ ] Finalize documentation and results. 