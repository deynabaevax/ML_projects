<img width="600px" src="https://miro.medium.com/max/1400/0*IJxyJh__userm-j_.png">

# Introduction
Diabetes is one of the major diseases of the population across the world. Diabetes is a chronic disease that occurs either when the pancreas does not produce enough insulin or when the body cannot efficiently use the insulin it produces. In 2014, 8.5% of adults aged 18 years and older had diabetes. In 2012, diabetes was the direct cause of 1.5 million deaths and high blood glucose was the cause of another 2.2 million deaths. Over the time, diabetes can damage the heart, blood vessels, eyes, kidneys, and nerves. Early diagnosis can be made through a relatively inexpensive method of computation. 

# Goal
Diabetes is one of the major diseases of the population across the world. Diabetes is a chronic disease that occurs either when the pancreas does not produce enough insulin or when the body cannot efficiently use the insulin it produces. In 2014, 8.5% of adults aged 18 years and older had diabetes. In 2012, diabetes was the direct cause of 1.5 million deaths and high blood glucose was the cause of another 2.2 million deaths. Over the time, diabetes can damage the heart, blood vessels, eyes, kidneys, and nerves. Early diagnosis can be made through a relatively inexpensive method of computation. In this notebook the ANN model is used to analyze and make the diabetes prediction model.

# The Dataset
The Dataset
In this dataset, all patients are females at least 21 years old of Pima Indian heritage. The total number of instances is 768, which is completely used in this study. It contains 8 attributes plus one class (Label) column. Each attribute is numeric-valued; attributes of this dataset are as follows:

- Number of times pregnant
- Plasma glucose concentration at 2 h in an oral glucose tolerance test
- Diastolic blood pressure (mm Hg)
- Triceps skinfold thickness (mm)
- 2-hour serum insulin (mu U/ml)
- Body mass index (weight in kg/(height in m2)
- Diabetes pedigree function
- Age (years)
- Class variable (0 or 1).
- (Class value 1 is interpreted as "tested positive for diabetes").

# Exploratory Data Analysis
At first when I looked the data, I saw that there were obviously some cells, which contained zero's. I needed to handle that as it is impossible to have BMI, blood pressure and insulin as zero's.

![Screenshot 2022-10-16 160547](https://user-images.githubusercontent.com/64732465/196039871-c2723f84-9d20-4715-8497-36da062d0f22.png)

On the below figure, it can be seen the distribution of the missing data within the dataset.

![Screenshot 2022-10-16 160341](https://user-images.githubusercontent.com/64732465/196039868-7f2a5d7e-8f1a-4364-b682-13b85ecd08c5.png)

To handle that, I got the mean value of each column in which the missing values occur and I inputed it. After doing that, I noticed that there was a major problem, which was a disbalance in the dataset. In my case, I applied downsampling to quickly get rid of that. I would like to mention that this is not the best way to treat such a case but for the sake of simplicity it works.

# Modeling
In this assignment I first used an ANN. However, it did not seem to give high accuracy. So, after receiving feedback from a teacher of mine, I also applied Decision Trees and Random Forest Classifiers. They gave me better results in comparison to the Neural Networks.

### Results:
  - ANN (with 3 layers): 68%
  - ANN (with 5 layers): 71%
  - Decision Tree: 69%
  - Random Forest: 75%
