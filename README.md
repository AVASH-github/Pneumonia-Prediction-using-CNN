

# Identifying Pneumonia by Chest X-Ray Images




## ***Repository Contents***

- code  
    - 1_Data_Collection_EDA  
    - 2_Data_Preprosessing_Simple_CNN  
    
- data
    -chest_xray
        -test
            -bacteria
            -normal
            -viral
        -train
            -bacteria
            -normal 
            -viral
- flask  
- media  


## ***Table of Contents***

* [***1. Executive Summary***](#---1-executive-summary---)
* [***2. Data***](#---2-data---)
* [***5. Web Application***](#---4-web-application---)
* [***5. Next Steps***](#---5-next-steps---)

## ***1. Executive Summary***

Pneumonia is an inflammatory condition of the lung affecting primarily the small air sacs known as alveoli. Typically symptoms include some combination of productive or dry cough, chest pain, fever, and trouble breathing. Severity is variable.

Pneumonia is usually caused by infection with viruses or bacteria and less commonly by other microorganisms, certain medications and conditions such as autoimmune diseases. Diagnosis is often based on the symptoms and physical examination. Chest X-ray, blood tests, and culture of the sputum may help confirm the diagnosis. The disease may be classified by where it was acquired with community, hospital, or health care associated pneumonia.

The goal of this project is constructing a convolutional neural network (CNN) to identify whether a patient has pneumonia or not by classifying their chest X-ray images. This project is adequately scoped and focuses on one specific type of disease rather than targeting multiple diagnosis. Creating a robust algorithm that provides fast and accurate diagnosis is beneficial for both patients and medical proffesionals.




## ***2. Data***

Source: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

The data used was collected from Mendeley public datasets repository and described as Labeled Optical Coherence Tomography (OCT) and Chest X-Ray Images for Classification. The dataset consists of 5856 X-Ray images (JPEG) and 2 categories: Pneumonia/Normal. Pneumonia images are to be annotated as  Bacterial or Noraml or Viral in file names that were later separated to build a multiclass classification network.  
Approximately 10% of the images from each category have to be moved to test folder to be used in validation of the model.




## ***4. Web Application***

A web application was built where user uploads a chest x-ray image and immediately receives the probability rates of 3 distinct diagnoses:   
1- Normal  
2- Bacterial Pneumonia  
3- Viral Pneumonia  




## ***5. Next Steps***

- Collecting more data.  
- Adding more complexity in model and using gridsearch functionality.  
- Creating additional model with PyTorch library and compare the results.  
- Researching on how to detect most informative pixels on X-ray (highest weights) and highlight them on image output.  
- Having radiologists interpret same X-rays and compare their performance with model’s performance.


### ***6. How to run the code

Step 1: Create a virtual environment and install all the necessary library which is present in the file called requirement.txt.
Step 2: Download the data from the source given above and categories them into three folder namely bacteria, normal and viral. 
Step 3: Run the python code which is present in flask/app.py.
Step 4: Choose the file from the local device and get your result. 
