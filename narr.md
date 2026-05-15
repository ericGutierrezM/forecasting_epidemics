# Forecasting Epidemic Outbreaks

## Introduction
Motivation: we want to predict epidemic outbreaks for effective resource mobilization and death prevention.

(Motivate further with some numbers on deaths.)

## Data
- Target ($y$): epidemic outbreaks (0/1). We generate onset / incidence variables. Month-level data.
- Regressors ($X$):
  - (BASELINE) Lags of the dependent variable (history) -- (we have to check whether it is persistent or if there are epidemic traps, similarly to what happens in conflict)
  - (BASELINE) Health indicators
  - (BASELINE) Socioeconomic indicators
  - (TEXT-ENRICHED MODEL) Text features, maybe _topics.csv_, Google Trends, or GDELT. 

## Methodology
- Describe how the onset / incidence variables are generated.
- Describe the data pre-processing / feature engineering in the regressors.
- Pseudo-out-of-sample cross-validation.
- Use Random Forest (Classifier), for example.
- (BONUS) Adapt cost functions:
  - FP: resources mobilized, non-assistance in some other region.
  - FN: deaths, disease spread.

## Results
- Confussion matrix across folds for each model (BASELINE, BASELINE + TEXT).
- Feature importance (for each model) -- it can be interesting.
- ROC and PR curves + rigorous interpretation.
- (BONUS) Adapt cost

## Conclusion
