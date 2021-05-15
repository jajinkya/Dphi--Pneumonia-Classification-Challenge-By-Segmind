<h1 align = 'center'>Dphi-Pneumonia-Classification-Challenge-By-Segmind</h1>   

**Hackathon organised by Segmind**

Pneumonia Classification in Chest X-Rays (CXRs) is organized by Segmind. As you maybe aware, "Pneumonia killed more than 808,000 children under the age of 5 in 2017, accounting for **15% of all deaths of children under 5 years**. People at-risk for pneumonia also include adults over the age of 65 and people with preexisting health problems." — **WHO**

While prevalent, diagnosing pneumonia in a CXR accurately is difficult. Expert radiologists are required to review the CXR and also require confirmation through clinical examinations. 
## Problem Statement:  
***You are tasked to classify CXRs with pneumonia from their normal CXR counterparts, using machine learning and computer vision techniques.***

-----------------------

**Brief summary of data**  

[Segmind](https://segmind.com/) provided Chest X-ray image dataset containing the X-rays with no pnuemonia finding calles as **Normal** and with pneumonia finding as **Pnueumonia**. Dataset consists of **2425** CXRs for training and **606** CXRs for testing. 

Training data: 1145 Pneumonia CXRs and 1280 Normal CXRs. Every CXR is a 1024 X 1024 image in the PNG format.
The **labels for each CXR were extracted using an NLP label extractor from corresponding radiology reports.**   
To download the dataset: https://drive.google.com/file/d/1d_93d9oFNRBK9Vg6BRxs9wvRbKtNTylY/view?usp=sharing


----------------------
Used a pretrained weights of the [ChexNet](https://stanfordmlgroup.github.io/projects/chexnet/) a **121 densely connected convolutional neural network** and use transfer learning to build a model.  
Weights file can be found [here](https://www.kaggle.com/theewok/chexnet-keras-weights)  

-----------------------
### Results of Hackathon
To evaluate the model [**F1-Score**](https://en.wikipedia.org/wiki/F-score) is used. 

|Public Score| Rank on Public Platform|
|------------|-----------------------|
|83.8764|4th |

|Private Score| Rank on Private Platform|
|-------------|--------|
|82.5094|6th|
