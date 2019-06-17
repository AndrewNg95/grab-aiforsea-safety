# AIForSea - Grab - Safety

This repo is for AIForSea - Grab Competition. The challenge taken up is to classify a particular driver is a save or dangerous driver based on the telematics data given.

## Setting up
1. `brew install pipenv`
2. Run `pipenv install` to install the required packages.
3. Run `pipenv run notebook` to run notebooks with the required packages installed.
4. Do not run commented codes unless required. The files weren't added into the repo due its massive file size. The features was combined using the commented codes and was grouped by using their bookingID and aggregated according to their respective median (to account for outliers). Only run the commented codes if you know what you doing.

## Notebooks
1. Kindly find the notebooks as your perusal in the notebook directory. The models would be created and it would be in a separate notebook accordingly.

# Best model - Random Forest Classifier
`rfc = RandomForestClassifier(criterion='gini',n_estimators = 18,max_depth = 18, max_features = 2,min_samples_leaf = 1,min_samples_split=4,random_state = 0)` with AUC scoring of 0.6112312749439615.