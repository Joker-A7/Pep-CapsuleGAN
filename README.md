# DeepACE
Angiotensin-I converting enzyme (ACE) plays an important role in maintaining the balance of the angiotensin system and regulating blood pressure in the body. Due to its importance, ACE has also become the target of many drugs to treat hypertension and cardiovascular diseases. Among them, the strength of ACE inhibitory activity will affect the effect of the drug. How to accurately identify peptides with strong ACE inhibitory activity from ACE inhibitory peptides is of great significance.
this study proposes a novel and high-accuracy prediction model (DeepACE) developed using generative adversarial capsule network (CapsuleGAN), to accurately identify peptides with strong ACE inhibitory activity. For DeepACE, we first utilized a wide range of feature encoding schemes derived with two main types of feature encoding strategies, including hand-crafted feature encodings and pre-trained protein language models, to extract the hidden interrelated information embedding in ACE inhibitory peptides. Subsequently, these extracted features were fused and used to develop a predictor based on the CapsuleGAN model for identifying peptides with strong ACE inhibitory activity. Finally, to enhance the model performance we performed the dimensionality reduction on the fused features using the principal component analysis (PCA) method. Comparative analysis results show that in independent tests, DeepACE's prediction performance is significant, with a balanced accuracy of 0.984 ± 0.039, an MCC of 0.968 ± 0.079, and an AUC of 0.995 ± 0.014, which are significantly better than existing methods. In addition, DeepACE was able to attain a superior prediction performance compared with well-known machine learning-based and deep learning-based classifiers.
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
