# Contraceptive Methods Analysis

This is a project that explores the relationship between different personal and socio-economic factors of users and the contraceptive plans they follow. The aim of this study is to aid healthcare organizations and policymakers in understanding how different factors affect contraception, such as which age-group or socio-economic class of the society to introduce subsidized contraceptive plans for.


## Dataset

The [dataset](https://archive.ics.uci.edu/ml/datasets/Contraceptive+Method+Choice) used in this project is a subset of the 1987 National Indonesia Contraceptive Prevalence Survey, obtained from the [UCI Machine Learning repository](https://archive.ics.uci.edu/ml/index.php). The data consists of personal and socio-economic attributes of married women who were either not pregnant or do not know if they were at the time of interview, and the contraceptive method they are currently using.

## Dependencies

The projeect is developed with following dependencies
 - R version 3.6.3 or later
 - RStudio version 1.3 or later
 - altair==4.2.0
 - numpy=1.23.3
 - ipykernel
 - scikit-learn==1.1.2
 - pandas=1.4.4
 - matplotlib>=3.5.3
 - glmnet>=4.1
 - tidyverse
 - VGAM>=1.1

## Usage

If you would like run the analysis yourself, please make sure you have all the dependencies installed, and then follow the following steps, in order:

1. Clone the repository by typing this on your terminal:
``` git clone https://github.com/qurat-azim/contraceptive_methods_analysis```
2. Run the notebook [Preliminary_EDA](https://github.com/qurat-azim/contraceptive_methods_analysis/blob/main/src/Preliminary_EDA.ipynb) in your ipykernel for performing exploratory data analyis.
3. Run the notebook [multinomial_inference](https://github.com/qurat-azim/contraceptive_methods_analysis/blob/main/src/multinomial_inference.ipynb) in R kernel for inferential analyis.
4. Run the notebook [train_yest_split](https://github.com/qurat-azim/contraceptive_methods_analysis/blob/main/src/train_test_split.ipynb) in ipykernel for train test split.
5. Run the notebook [ML_models](https://github.com/qurat-azim/contraceptive_methods_analysis/blob/main/src/ML_models.ipynb) in ipykernel for performing predictive analysis.


## Analysis

In this project, we conducted an inferential analysis using a generalized linear model with multinomial logistic regression to study the association between personal and socio-economic factors of users and the contraceptive plans they follow. We also conducted multi-class classification predictive analysis to predict a user's contraceptive strategy using their personal and socio-economic attributes. We found that gradient boosting methods perform really well. However, we improved the logistic regression model (due to its interpretability) with hyperparameter optimization and achieved a weighted average f1 score of 0.54 on the test set.

## Results

The final report of the project is available [here](https://github.com/qurat-azim/contraceptive_methods_analysis/blob/main/doc/report.md). It includes the exploratory data analysis, inferential analysis, and predictive analysis, as well as the results and interpretations of the analyses.

## Future improvements

This project is under active development, and we are working on many more areas of improvement for whoever wants to use the analysis. We are working on:
- scripting the files
- making and environment file for installing all dependencies at once
- automating the running of project through `make`
- possibly Docker containerization for complete automation

## Contributing to the project

Interested in contributing? Check out the contributing guidelines [here](https://github.com/qurat-azim/contraceptive_methods_analysis/blob/main/CONTRIBUTING.md). Please note that this project is released with a [Code of Conduct](https://github.com/qurat-azim/contraceptive_methods_analysis/blob/main/CODE_OF_CONDUCT.md). By contributing to this project, you agree to abide by its terms.

## References

The dataset used in this project is the [dataset](https://archive.ics.uci.edu/ml/datasets/Contraceptive+Method+Choice) we use is obtained from [UCI Machine Learning repository](https://archive.ics.uci.edu/ml/index.php).

Please refer to the original data sources for more information on how the data was collected and processed.

## License

`contraceptive-methods_analysis` was created by [Qurat-ul-Ain Azim](https://github.com/qurat-azim). The materials of this project are licensed under the [MIT license](https://github.com/qurat-azim/contraceptive_methods_analysis/blob/main/LICENSE). If re-using/re-mixing please provide attribution and link to this webpage.
