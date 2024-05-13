
**🍷Prediction of Wine Quality via Dense Neural Network🍾**
------------------------------------------------------------------

Physiochemical components from various type of wine had been analyzed in order to find the correlation between each element with the wine's quality as the sensory output. It was found that Alcohol, Sulphates, Fixed Acidity, and Citric Acid correlates positively with the quality while Volatile Acidity, Total Sulfur Dioxides, Chlorides, and Density correlates negatively. Meanwhile, Residual Sugar, Free Sulfur Dioxides, and pH have little correlation with the quality.

However, using correlation matrix, it is speculated that despite the small correlation, these variables might be already represented with other components which they have in common, e.g. pH with Fixed Acidity.

--------------------------------------------------------------------

Data was preprocessed using SMOTE oversampling since the imbalance of data distribution. Model was built using Dense Neural Network from Tensorflow.Keras libraries with 5580 total trainable params. 

![model_preview](https://github.com/Andiko-K/Wine-Quality-Analysis/assets/114839796/a06e3e2c-eefd-4f27-a35b-63329fd5dd4c)

Model was trained for 1000 epochs with 64 batch size using ModelCheckpoint Callbacks. Model achieves 0.564 Validation Loss and 0.82 Validation Accuracy. 

--------------------------------------------------------------------

Model performance were later being analyzed using Confusion Matrix in which model was having a hard time in determining Level 4 and Level 7 quality due to the imbalance of data distribution. Despite so, it performed well in Level 3,5,6, and 8 with SMOTE oversampling.

Dataset acquired from <a href = https://www.kaggle.com/datasets/yasserh/wine-quality-dataset> Kaggle Wine Quality Dataset</a>


