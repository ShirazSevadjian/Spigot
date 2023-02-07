# Spigot - Predicting Water Potability
Spigot is a machine learning project to see whether a sample of water is potable or not, based on specific features

### Project Goal
The main goal of the project is to accurately conclude the potability of water. Determining whether or not a source of water is safe for consumption is
crucial to the people relying on it. A secondary goal is to determine which features are not impacting results and can be removed. 
As a secondary goal, we would like to test the accuracy and efficiency of the results on different types of models, such as Logistic Regression, Support
Vector Machines, Random Forest, KNN, etc. Having different models that we can run tests on, will help us determine which approach yields the best results
for the type of data we plan to use.


### Input
Our input will contain features needed to differentiate the quality of water, such as particulates, chemicals, and acidity. The input will be a 1
dimensional array of properties: pH (number from 0 to 14), Hardness (mg/L), Solids (ppm), Chloramines (ppm), Sulfate (mg/L), Conductivity (μs/cm), Organic
Carbon (ppm), Trihalomethanes (μg/L), Turbidity (Nephelometric Turbidity Unit) - all these values are numbers.


### Output
The desired output is a label indicating whether the water is potable (1) or not (0). Our model will output either one of these labels to indicate if we
can drink the water with the given features.


### Training and Testing Samples
The total number of rows is 3,276. We will split our data into two: a training sample (around 80%) and a testing sample (around 20%). The percentages might
vary based on the results we get. The model can be trained on a laptop, but a more powerful computer will likely be used to allow us to quickly train new
models, tune them, and compare results without having to worry about performance.


### Preprocessing
The data we selected is realistic but not perfect. Rows have missing values and the values vary a lot from one column to
another (different metrics). We will try out different approaches to deal with missing values (dropping rows, adding median values, adding values based on
similar rows). We will scale and normalize our data to see if we get better results.


### Main packages
<ul>
<li><b>Pandas:</b> Retrieve and Process data</li>
<li><b>Scikit-learn:</b> Preprocess data and train predictive models, test our models using testing datasets, and Hyperparameter Tuning</li>
<li><b>Matplotlib:</b> Data visualization to analyze our results and deduct conclusions</li>
<li><b>NumPy:</b> For computation and creation of arrays</li>
</ul>