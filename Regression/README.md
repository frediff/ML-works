The `data.csv` file containing 294 rows and 10 columns
(`?` refers to not available value)
The features that need to be considered are:

- **age**: age in years
- **sex**: sex (1 = male; 0 = female)
- **cp**: chest pain type
  - 1: typical angina
  - 2: atypical angina
  - 3: non-anginal pain
  - 4: asymptomatic
- **trestbps**: resting blood pressure (in mm Hg on admission to the hospital)
- **chol**: serum cholesterol in mg/dl
- **fbs**: (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
- **restecg**: resting electrocardiographic results
  - 0: normal
  - 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
  - 2: showing probable or definite left ventricular hypertrophy by Estes’ criteria
- **thalach**: maximum heart rate achieved
- **exang**: exercise-induced angina (1 = yes; 0 = no)
- **oldpeak**: ST depression induced by exercise relative to rest

*(Rows and columns that are not useful are dropped)*

Using this data we implement (`model_RGRSS.ipynb`) the following regression techniques from scratch:
- ***Linear Regression***
- ***Lasso Regression***
- ***Ridge Regression***

Finally we give the comparative analysis of all these regression techniques.
