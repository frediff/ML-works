## XGBoost vs SVM ##
We use the attached dataset `S_n_I_A_N_P_An_Io_noaa2.txt`. The dataset contains 870 rows × 7 columns in a space separated manner. The columns are ‘SAM’, ‘nino’, ‘ISMR’, ‘AMO’, ‘NAO’, ‘PDO’, ‘At-nino’, ’IOD’. Here ISMR is mean monthly rainfall in Indian region. Other columns denote potential causal drivers for ISMR, which are climatic conditions in other parts of the world. The rows contain monthly data for the months ‘May’, ‘June’, ‘July’, ‘Aug’, ‘Sep’, ‘Oct’ for the years 1871-2015 (145x6=870).  E.g., The first row contains the data for May, 1871. Ignore the column "SAM".

ISMR can be predicted using the potential drivers, but the lags can be different. E.g., If rainfall of July is caused by the driver values of May, then the lag value will be 2. That means the predictor values of 2 months back causes the rainfall of the current month. We use ***Xgboost regresssor*** to predict ISMR for different lag values of the drivers and print the true and predicted values of the ISMR for different lags in a tabular form.

Then we plot the true values vs predicted values of ISMR in scatter plots for different lags separately. We try to find out which lag is statistically showing best results.

We repeat the experiment for ***SVM*** with different kernel values to find the best performing one. We use grid search method to find the best performance.

- `model_XGBOOST.ipynb` contains the experiment using XGBOOST
- `model_SVM.ipynb` contains the experiment using SVM
