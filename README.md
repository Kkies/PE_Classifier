# Pulmonary Embolism Classification Using Convolutional Neural Networks 

#### Ben Inoyatov, Jamil Mirabito, Kyle Kieser

### Introduction
---
- A PE is a blood clot that gets lodged in the vasculature of the lungs. Typically patients who are unhealthy will have many, small emboli however, a massive PE can be deadly as your heart and lungs are directly attached to one another. According to the CDC, sudden death is the FIRST symptom in about a quarter of patients with a PE. Additionally, 10-30% of patients will die within one month of diagnosis. 
- Data was taken from Kaggle. The original size of the data was over 900 gigabytes due to the large image files. However, we were able to find a smaller sized JPEG version of the data which we used for this project. 
- Libraries used: ```pandas numpy matplotlib scikitlearn tensorflow keras```

Notebooks to refer to:
- pulmonary_embolism_EDA.ipynb
- pe_classification.ipynb
- Google Colab Notebook for Transfer Learning Models: https://colab.research.google.com/drive/1hm0cOi4mKFBe_tdrxgnMiIC5go1LnDu3?usp=sharing

### The Business Question/Case 
---
- PEs can be hard to spot even for experienced and specialized practitioners. However, with the advent of Deep Learning, we have another tool in our toolbox to help classify PEs with more accuracy. 

### Data
---
**Data:** RSNA STR Pulmonary Embolism Detection Dataset

**Sample:** 1,790,594 images; 7,297 participants


**Only 5 percent of images in the dataset presented a Pulmonary Embolism**
![class_imbalance](https://user-images.githubusercontent.com/64563191/96951229-0842cc00-14ba-11eb-85b8-1c286cc5431b.png)


### Modeling Process
**Random Sampling:**
We randomly selected 5,000 images from each class to train, validate, and test our model.
- Train: 4,200 images
- Validation: 1,800 images
- Test: 5,000 images


**Modeling:**
- We tested a total of 13 models in Jupyter Notebooks and Google Colab.
- 10 used multiple optimizers, batch sizes, epochs, & numbers of layers - 3 were Transfer Learning models - Inception & ResNet 50


**Model Evaluation:**
- We optimized our models on the Recall score so as to limit the number of PE misses (false negatives).


###  Select Observations/Findings and Conclusions
---
- Final model had 3 convolutional layers with a max pooling layer after each one
- Adam was the best optimizer
- Transfer Learners (Inception & ResNet) increased complexity for marginal improvement

<img width="517" alt="Screen Shot 2020-10-23 at 11 07 35 AM" src="https://user-images.githubusercontent.com/65979022/97020842-0f042a00-1520-11eb-8866-583e31ad75c7.png">


###  Limitations & Recommendations 
---
- We were unable to train the model to identify where the PE was located in each image (i.e., right lung, left lung, pulmonary artery). Future models could create multi-class outputs to identify the location of the PE.
- Given the large size of the dataset and computational limitations, we were unable to train the model on the full dataset thereby limiting the performance of the model. With more time and computational power, future models could train/validate/test on more than just 5,000 images.
- We were unable to incorporate RV/LV into our analyses. Future models could compare the size of the Left and Right Ventricles (RV/LV ratio*) to predict probability of morbidity.
 


## Links 
- **Google Slides Presentation:** https://docs.google.com/presentation/d/1p4VuCOoV3bwCLtrCccHUAjWcxJAHMOGNIu_sMCHDAcY/edit?usp=sharing
- **CDC statistics on PEs:** https://www.cdc.gov/ncbddd/dvt/data.html#:~:text=The%20precise%20number%20of%20people,(also%20called%20venous%20thromboembolism)
- **Data:** https://www.kaggle.com/c/rsna-str-pulmonary-embolism-detection
