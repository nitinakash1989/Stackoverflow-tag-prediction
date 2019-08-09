
<img src='images/img.jpeg'/>

# Stack Overflow: Tag Prediction

This ipython notebook is developed to predict as many tags as possible for questions posted on StackOverflow by applying differnt machine learning algorithm. A step by step analysis has been done on the data provided in the Kaggle. Based on the data provided, the machine learning model predicts the tags like(C#, Java etc) for each question.

<b>Data Source:</b><a href="https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/">https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction</a>


Data Dictionary
- Title,
- Body,
- Tags

With the provided data, we will first clean the data to get data in required format followed by exploratory data analysis.

Featurizing is one of the most important steps for building machine learning model. We will use `TF-IDF` to convert text into vector.

Since the dimension of input vector is high, we will be using linear multilevel classification algorithm to predict the tags.
We will be applying different multilevel classification model having optimized hyperparameter.  
- `Logistic Regression with GridSearch`
- `XgBoost classifier with Random search`

For testing the result we will use
- `Micro f1 scoore`
- `Macro f1 scoore`
- `Hamming loss`

__Objective: redict the Tag based on the text present in question posted using different classification technique with high precision and recall.__

This project is developed with the help of videos and basic code provided by appliedaicourse.com.
