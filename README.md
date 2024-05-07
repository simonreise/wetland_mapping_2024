# Data for *"Application of Machine Learning Techniques to Map Wetland Types in the Numto Nature Park (Western Siberia)"*

## Python code 

 The numto.ipynb file is the Jupyter Notebook with Python code that was used for data preprocessing, training the models and mapping the modeling results.

 ## Model checkpoints

This repository contains only joblib dumps of trained classical machine learing models. Model checkpoints for deep learning models are too large for GitHub and can be only provided by request.

| File         | Model                     |
|--------------|---------------------------|
| lr.joblib    | Linear regression         |
| rf.joblib    | Sklearn Random Forest     |
| xgbrf.joblib | XGBoost Random Forest     |
| xgb.joblib   | XGBoost Gradient Boosting |

## Maps

| File                  | Map                                      |
|-----------------------|------------------------------------------|
| map_nn.tif            | Modeling with DeepLabV3                  |
| map_nn_clip.tif       | Same, but clipped                        |
| map_nn_train.tif      | Same, but only for park area             |
| map_nn_train_clip.tif | Same, but only for park area and clipped |
| map_xgb.tif           | Modeling with Gradient Boosting          |
| map_xgb_train.tif     | Same, but only for park area             |

Map legend:
| Value | Class                           |
|-------|---------------------------------|
| 0     | No data                         |
| 1     | Lakes                           |
| 2     | Forests                         |
| 3     | Burnt areas                     |
| 4     | Palsa mires                     |
| 5     | Oligotrophic mires              |
| 6     | Eutrophic and mesotrophic mires |
| 7     | Built-up areas                  |
