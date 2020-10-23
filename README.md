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


###  Recommendations 
---
- Some of the things we didn’t get to do for this project was classify WHERE the PE is. Being that we only had a few days and that CNNs are computationally stressing, we just classified if there was a PE or not. 
- Also, Radiologists will use the size of the left and right ventricles to further determine morbidity. Can we use a CNN to measure the sizes and output a probability that this scan has high morbidity? 


## Links 
- **Google Slides Presentation:** https://docs.google.com/presentation/d/1p4VuCOoV3bwCLtrCccHUAjWcxJAHMOGNIu_sMCHDAcY/edit?usp=sharing
- **CDC statistics on PEs:** https://www.cdc.gov/ncbddd/dvt/data.html#:~:text=The%20precise%20number%20of%20people,(also%20called%20venous%20thromboembolism)
- **Data:** https://www.kaggle.com/c/rsna-str-pulmonary-embolism-detection
- **Google Colab Notebook for Transfer Learning Models:** https://colab.research.google.com/drive/1hm0cOi4mKFBe_tdrxgnMiIC5go1LnDu3?usp=sharing
