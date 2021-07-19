# Ads-Click-Prediction-Report

- DataSet: Ad Click Prediction
- Problem: Classification Problem
- DataSet Source: https://www.kaggle.com/jahnveenarang/cvdcvd-vd - DataSet Description:

   1. 'User ID': unique identification for consumers.
   2. 'Age': customer age in years.
   3. 'Estimated Salary': Avg. Income of consumer.
   4. 'Gender': Whether the consumer was male or female.
   5. 'Purchased': 0 or 1 indicated clicking on Ad.

- Features after Preprocessing:

   1. 'Age': customer age in years.
   2. 'Estimated Salary': Avg. Income of consumer.
   3. 'Gender': Whether the consumer was male[0] or female[1].
   4. 'Purchased': 0 or 1 indicated clicking on Ad.


- Machine Learning Model and Evaluation:
   ➔ Decision Tree Classifier model.
   ➔ Accuracy Score for evaluation.
   
   <img width="371" alt="1" src="https://user-images.githubusercontent.com/51120437/126098361-40ae0444-cdee-4e44-ba27-6f9a28382b11.png">
# Male Samples
<img width="535" alt="2" src="https://user-images.githubusercontent.com/51120437/126098383-25b18948-aeb0-4aab-a46b-28dcd9bc9bfd.png">

<img width="420" alt="3" src="https://user-images.githubusercontent.com/51120437/126098393-6dec79f4-9b35-4f00-af85-8c7a7f68cf86.png">

-Males between [40,60] clicks with negative correlation to the Salary.

-Males between [20,40] don't click with positive correlation to the Salary.



# Female Samples
<img width="535" alt="4" src="https://user-images.githubusercontent.com/51120437/126098418-0e87af56-e9fc-4821-b3fe-add1de0a2235.png">
<img width="429" alt="5" src="https://user-images.githubusercontent.com/51120437/126098432-b60c99ad-6077-40af-b248-198dd1ea4f6f.png">


-Females with a salary between [8000,140000] clicks with negative correlation to age.

-Females with a salary between [20000,80000] clicks with positive correlation to age.

# Age>40 for both genders
<img width="444" alt="6" src="https://user-images.githubusercontent.com/51120437/126098470-48f4b5ae-ae30-4ddd-b6c3-99b3f7634d95.png">
Female Makes more click then male

# Decision Tree Model
![diab](https://user-images.githubusercontent.com/51120437/126098495-c955b43d-74ab-49f0-b0f7-fc8af79d3807.jpg)

