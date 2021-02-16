# MNIST_Number_Generalized_Linear

# Introduction to Topic

In this assignment we are going to implement Random Forest algorithm for classification problem. As per the described problem we have 3 classes or categories of different type of fruit flies as target variable. This dataset is comprised of 2 sets 1 is training set and testing set with 17259 rows and 5001 columns. This data is built from the audio of wingbeats which is recorded through the sensors in environment where aptitude of infra-red lights is recording over the period of time which is occurred by wings of flies while flying. This need to be understood that these flies are classified into 3 breads as follows: Melanogaster (6,064), suzukii (10,142), zaprionus (18,312) with the given number of recordings in the training and testing set which are randomly partitioned. 

In this problem are task is to train the model using RandomForestClassifier so that by using this model or system we can categorize the flies bread. To test out results as mentioned we are given test data to check the accuracy of our model. 

It is important us to know what Random forest Classifier is and how it works also how will this algorithm going to help us in solving this problem. So, Random forest is a technique which a ensemble method which functions in a way that it uses multiple algorithms to obtain better performance or we can say it runs the algorithms multiple time and see which parameter combination is giving the better predictive performance instead of just using 1 learning algorithms. This method reduces the risk of overfitting which is highly seen in decision trees. 

 
Picture Credit: Wikipedia
As a part of problem statement given by the professor, we have to check the results as accuracy of model by using number of tree values as 5, 50 and 500 while keeping all the parameters in default state.

The problem statement for the below work is obtained from ( https://drive.google.com/drive/folders/1MmADP0xSDowsH7zZ-vXcxlBONS7rFAEi?usp=sharing ) the dataset used for the problem and python code used for the code has been uploaded in the google folder. In the following step we are importing all the required libraries based on requirement of the assignment

# Code and Outputs with Explanation: 

Step 1: In the first step of our analysis as this dataset was in “arff” format which is named as attribute relation file format, we have used scipy library to import .arff files of train and test data. Other then this we have imported numpy, pandas, copy, and Random forest Classifier from sklearn ensemble library. [2]

 

Step 2: In this step we have imported the train and test dataset into notebook of Colab environment. Further to which we have converted the dataset into data frame which displays the dataset into 2-dimensional tabular data structure with designated labeled rows and columns.[3]

 

Step 3: In this step after identifying the target variable, they were in string form and as mentioned in the description there are 3 categories. We converted the categories from string form to numerical form for both the train and test datasets i.e., 0, 1, 2.

 

Step 4: In this step we can see the outputs after the target variable it’s in numerical form.

 


Step 5: In this step our aim was to separate the dataset into train and test sets. Where we are aware, we already have test and train set. So, we have made 4 distinct variables with “x_train”, “x_test” having independent variable and “y_train”, “y_test” having target variable or dependent variable.
 

Step 5: In this step we have applied random forest classifier using different values of trees as 5, 50,500. Instead, I have used 5,50,70,80,100,150,200,250,500 to check how number of trees works which I will be explaining in analysis section of results.

 

Critical Analysis:

In the above analysis we have used “i” as the values of number of trees. As per the problem statement we are asked to use only 5, 50, 500. To see how increase in number of trees could make a difference in model learning. After looking the accuracy score, we can see after 70 the model stopped learning by much difference.

Random Forest algorithms include extra randomness while building multiple trees. Instead of looking for the foremost important feature while part a node, it looks for the finest include among a random subset of highlights.  Therefore, in arbitrary timberland, as it where an irregular subset of the highlights is taken into thought by the algorithm for part a hub. You'll indeed make trees more irregular by furthermore utilizing irregular limits for each include instead of looking for the leading conceivable thresholds.


 

References:
[1] Random forest https://en.wikipedia.org/wiki/Random_forest
[2]Scipy.io.arff.loadarff¶https://docs.scipy.org/doc/scipy/reference/generated/scipy.io.arff.loadarff.html
[3] Python: Pandas Data Frame https://www.geeksforgeeks.org/python-pandas-dataframe/
[4] https://timeseriesclassification.com/description.php?Dataset=FruitFlies
[5] Multiclass Classification using Random Forest on Scikit-Learn Library
[6] Agarwal https://www.codementor.io/@agarrahul01/multiclass-classification-using-random-forest-on-scikit-learn-library-hkk4lwawu







