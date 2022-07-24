# Student-Performance-Analysis

## Motivation
***
In the Data Science domain after having the basis knowledge from end to end, a beginner is generally facing a lot of issue while putting all things together.

So, it is going to be great starting reference point for a beginner who wants to getting started with some basic end to end models.

We will follow the below mentioned path 

Objective
Loading and understanding the dataset. 
Exploratory Analysis of Data and Visualization.
Model Building.
We will keep it as simple as possible by putting ourselves in the shoes of a beginner.


## Objective and Data Set
***
In this getting started project, we will Analyze Student Performance based on few parameters such as gender, race/ethnicity, parental level of education, lunch type and whether the student prepare for test or not.

For this Purpose we are going to use StudentsPerformance.csv file , If you are interested (highly recommended) to follow along you can download the data file from here and go along.

In this Student-Performance-Analysis Project we will analyze the different parameters as mentioned above and their impact on the student performance, we will also create visualization for the same.
After the Analysis is done we will try to make some simple models with the available features and evaluate the performance of our Model.
So, Let's Started !!!


## Loading and understanding the dataset
***
* We have 1000 data points each having 8 features.
* Out of 8 features 
..*5 are categorical features
..*3 are numerical features
* There is a high correlation between Reading and Writing Score of a Student.
* We don't have any null or empty cell in our data frame.

## Exploratory Data Analysis and Visualization:
***
### Univariate Analysis of Numerical Variable
* Distribution of Marks in Math and Reading seems to be equal, while students are performing well in writing section.

### Univariate Analysis of Categorical Variable
* We have almost equal number of male and female students.
* We have least number of students from group A and highest number of student from group C.
* Around 60 parents have a master's degree.
* Around 350 students not able to get a standard lunch and depends on free or reduced lunch.
* 2/3rd students are not preparing test while 1/3rd number of students are completely preparing for the test.

### Multivariate Analysis with Boxplot
* In general Male student performs better in Math, While female performs better in reading and writing section.
* student with race as group E are performing better in Math and reading but incase of writing except group A which is lacking rest all race students performs same in the writing section.
* students with parental level of education as master's degree have an edge in reading and writing section.
* students having standard lunch seems to perform well in all the 3 sections.
* As Expected in general students who completely prepare for the tests performs better in all the 3 section than the students who are not prepared.

## Data Preparation for Model Building:
***
* We have 5 independent features and trying to analysis the 3 features such as math score, reading score and writing score for those we only have 1000 data points. So rather than predicting the score in each subject, we will try to predict the grade of the student.
* We will calculate the percentage mark of each student and on the basis of the percentage mark , we will divide the students into 7 categories and then with our model we will try to predict those categories.
* Finally we will save the processed data as prepared.csv for further proceeding.
