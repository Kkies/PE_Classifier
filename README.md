# Pulmonary Embolism Classification Using Convolutional Neural Networks 

#### Ben Inoyatov, Jamil Mirabito, Kyle Kieser

## Introduction
---
- A PE is a blood clot that gets lodged in the vasculature of the lungs. Typically patients who are unhealthy will have many, small emboli however, a massive PE can be deadly as your heart and lungs are directly attached to one another. According to the CDC, sudden death is the FIRST symptom in about a quarter of patients with a PE. Additionally, 10-30% of patients will die within one month of diagnosis. 
- Data was taken from Kaggle. The original size of the data was over 900 gigabytes due to the large image files. However, we were able to find a smaller sized JPEG version of the data which we used for this project. 
- Libraries used: ```pandas numpy matplotlib scikitlearn tensorflow keras```
- Notebooks to refer to 
### The Business Question/Case 
---
- PEs can be hard to spot even for experienced and specialized practitioners. However, with the advent of Deep Learning, we have another tool in our toolbox to help classify PEs with more accuracy. 
###  Select Observations/Findings and Conclusions
---


###  Limitations & Recommendations 
---
- We were unable to train the model to identify where the PE was located in each image (i.e., right lung, left lung, pulmonary artery). Future models could create multi-class outputs to identify the location of the PE.
- Given the large size of the dataset and computational limitations, we were unable to train the model on the full dataset thereby limiting the performance of the model. With more time and computational power, future models could train/validate/test on more than just 5,000 images.
- We were unable to incorporate RV/LV into our analyses. Future models could compare the size of the Left and Right Ventricles (RV/LV ratio*) to predict probability of morbidity.
 


## Links 
- **Google Slides Presentation:** https://docs.google.com/presentation/d/1p4VuCOoV3bwCLtrCccHUAjWcxJAHMOGNIu_sMCHDAcY/edit?usp=sharing
- **CDC statistics on PEs:** https://www.cdc.gov/ncbddd/dvt/data.html#:~:text=The%20precise%20number%20of%20people,(also%20called%20venous%20thromboembolism)
- **Data:** https://www.kaggle.com/c/rsna-str-pulmonary-embolism-detection
- **Google Colab Notebook for Transfer Learning Models:** https://colab.research.google.com/drive/1hm0cOi4mKFBe_tdrxgnMiIC5go1LnDu3?usp=sharing
