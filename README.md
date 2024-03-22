# DeepACE
The implementation of the paper
## Requirements
The majoy dependencies used in this project are as following:
```
Python 3.9.18
fair-esm 2.0.0
pandas 1.3.5
numpy 1.21.6
scikit-learn 1.0.2
torch 1.13.0+cu116
tensorflow 2.6.0
keras 2.6.0
```
If other libraries are missing, you can install them yourself using the command `pip install package_name==2.0.0`
## t-SNE plot of the dataset
![t-SNE plot](https://github.com/Joker-A7/Pep-CapsuleGAN/blob/main/image/t-SNE.png)
## Model performance
![ROC curve](https://github.com/Joker-A7/Pep-CapsuleGAN/blob/main/image/Pep_ROC_Ind.png)
![PR curve](https://github.com/Joker-A7/Pep-CapsuleGAN/blob/main/image/Pep_PR_Ind.png)
## Usage
Note: The dataset uses 0 and 1 to represent high activity and low/no activity respectively.  
### Extract features
In the __iFeature_exteactor__ file, traditional feature extraction methods are provided, which can be modified according to your own needs. The __ESM and PortT5__ file provides extraction methods for ESM-2 and PortT5 features, and you can extract them according to your needs.
### Feature processing
The feature processing method is in the __extra_features__ folder, which includes feature fusion and feature selection. You can process the extracted features according to your own needs.
### Model prediction
In the __fusion_features__ folder, there are a variety of machine learning models and deep learning models. Such as: LR, SVM, MLP, CNN, DNN, etc. Models can be trained and tested by uploading your own data sets.
## Further adjustments and modifications
Feel free to personalize it. Just scroll down to the model architecture section and modify it to suit your expectations.
