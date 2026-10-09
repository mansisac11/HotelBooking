# Hotel Booking Analysis & Machine Learning
**From booking records to business questions, regression and classification.**

A portfolio project by **Mansi Sachar**, an enterprise technology professional with approximately 17 years of experience in technical investigation, SQL, automation and stakeholder communication, building practical data and AI capabilities.

## Project status
The hotel-booking learning project is **completed**, including regression and classification work, as reported by the author. This repository is its **documentation starter**: the original notebooks, dataset provenance, exact targets, model outputs and measured results have not yet been published here.

Completion of the learning work is distinct from reproducibility of this repository. There is currently no executable training pipeline or deployed model. All evidence fields below are deliberately unfilled rather than estimated.

## Business problem
Hotel teams need to understand booking patterns and plan for uncertain demand. This project connects exploratory analysis with two types of prediction:
- **Regression:** estimate a continuous booking-related outcome to support planning. The exact outcome used in the completed notebook must be recorded before publishing results.
- **Classification:** predict a booking-related category. Cancellation risk is a relevant business application, but the actual target and class definitions must be confirmed from the completed notebook.

Potential users include revenue, reservations and operations teams. Useful outputs would be interpretable patterns and evaluated predictions that inform decisions about capacity, booking policies or follow-up. These are intended applications, not demonstrated business impact.

## Dataset
| Item | Current documentation |
| --- | --- |
| Subject | Hotel-booking records |
| Original source and citation | **To add from the dataset actually used** |
| Source URL and access date | **To add** |
| Dataset version / file name | **To add** |
| Licence and redistribution permission | **To verify before uploading any data** |
| Rows, columns and observation period | **To add after checking the source file** |
| Unit of observation and field definitions | **To confirm from the data dictionary** |
| Regression target | **To confirm from the completed notebook** |
| Classification target / positive class | **To confirm from the completed notebook** |

No dataset is bundled. Do not substitute statistics from a similarly named public dataset. Record the actual source in [data/README.md](data/README.md); keep private data and identifiers out of the repository.

## Analysis summary
The project covers hotel-booking analysis alongside regression and classification. The published summary will be backed by notebook cells and figures once the original artifacts are added.

The following is the **reporting outline**, not a list of verified findings:
1. Profile the data: types, missing values, duplicate records and unusual values.
2. Describe booking patterns using fields present in the actual dataset, such as hotel category, arrival period, lead time, stay length or customer segment.
3. Examine how available predictors relate to the chosen continuous outcome and classification labels.
4. Explain preprocessing, feature selection and features excluded because they would be unavailable at prediction time.
5. Compare models with simple baselines and translate results into practical limitations.

Do not present correlations as causal effects or notebook performance as production impact.

## Completed modelling scope
| Workstream | Author-reported completed scope | Evidence to publish |
| --- | --- | --- |
| Regression | Linear regression | Target definition, features, preprocessing, split, baseline, coefficients and held-out metrics |
| Classification | Logistic regression | Target and class definitions, features, preprocessing, split, baseline, threshold and held-out metrics |

Logistic regression belongs to the classification workstream. Any additional algorithms should be listed only after checking the original notebooks.

### Evaluation evidence to document
- State when a prediction would be made and use only features available then.
- Identify the split strategy, random seed and any cross-validation. For a future-facing use case, evaluate whether a time-based split is more appropriate.
- Fit preprocessing on training data only; audit outcome/status fields and other potential target leakage.
- Report regression **MAE, RMSE and R²** against an appropriate simple baseline.
- Report classification **precision, recall, F1, ROC-AUC and a confusion matrix**; include class balance, a simple baseline and the chosen threshold. Consider PR-AUC for an imbalanced target.
- Keep the final test set separate from model and threshold selection.

These are evidence requirements for the portfolio; they are not claims that each check was performed in the original work.

## Results
**Not yet published.** Fill in values only from saved evaluation outputs.

| Task | Target | Baseline | Model | Test-set results | Evidence |
| --- | --- | --- | --- | --- | --- |
| Regression | To confirm | To document | Linear regression | MAE: pending; RMSE: pending; R²: pending | Notebook + metrics file pending |
| Classification | To confirm | To document | Logistic regression | Precision: pending; recall: pending; F1: pending; ROC-AUC: pending | Notebook + confusion matrix pending |

### Business findings to add
For each finding, include:
- **Observation:** what the data shows, with a figure or table.
- **Evidence:** population, period and calculation.
- **Decision relevance:** what a hotel team could consider.
- **Limitation:** uncertainty, missing context or scope restrictions.

No accuracy scores, savings or revenue improvements are claimed at this stage. The metric template is in [reports/results-template.md](reports/results-template.md).

## Repository structure
| Path | Purpose |
| --- | --- |
| `README.md` | Project overview, scope, evidence status and roadmap |
| `data/README.md` | Dataset provenance, acquisition and schema notes |
| `notebooks/README.md` | Suggested notebook sequence and publication checklist |
| `reports/results-template.md` | Structured results and interpretation template |
| `reports/figures/` | Exported EDA plots and evaluation figures |
| `models/README.md` | Model metadata and artifact documentation |
| `src/README.md` | Future reusable preprocessing and evaluation code |
| `.gitignore` | Exclude local data, model binaries, caches and secrets |

Folders currently contain guidance or placeholders. They do not imply that notebooks, models or reusable code have been uploaded.

## Technologies
Intended Python portfolio stack: **Python, pandas, NumPy, scikit-learn, Matplotlib, Seaborn and Jupyter Notebook**. The exact libraries and versions used in the completed work must be verified against its imports and environment before publishing a reproducibility claim.

Linear regression and logistic regression are the completed methods reported by the author. No framework-specific implementation is asserted yet. An environment file will be added once the actual notebook dependencies are known.

## How to explore
Start with this README and the documentation folders. There are no runnable notebooks or training commands yet.

Once the original notebooks are published:
1. Obtain the documented dataset under its permitted terms.
2. Install the verified dependencies in a clean environment.
3. Run the notebooks in the documented order.
4. Compare generated outputs with the saved metrics and figures.

## Realistic next steps
1. **Publish existing evidence:** add the completed EDA, regression and classification notebooks; confirm targets and remove private material.
2. **Make the work reproducible:** document provenance, dependencies, seeds, split strategy and preprocessing; rerun from a clean environment.
3. **Strengthen evaluation:** check leakage, compare baselines and examine errors across meaningful booking segments.
4. **Improve models selectively:** try a small number of justified alternatives, such as regularised regression or tree-based methods, using validation data.
5. **Improve decision usefulness:** if cancellation is the confirmed target, examine calibration and threshold trade-offs against the cost of missed cancellations and unnecessary follow-up.
6. **Communicate results:** add a concise visual findings report; consider a small dashboard only after the underlying results are verified.

## About the author
I bring an enterprise operations perspective to data and AI: understanding the business question, investigating evidence, checking assumptions and communicating usable conclusions. This project demonstrates my practical learning in analysis and predictive modelling; it does not represent professional production ML deployment.

[Mansi Sachar on LinkedIn](https://www.linkedin.com/in/mansi-sachar-a9bb71347)

## Use and attribution
This starter does not grant a software or dataset licence. Add an explicit code licence if intended, and retain the dataset's separate citation and usage terms.
