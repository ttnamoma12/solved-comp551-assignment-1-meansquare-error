Download Link: https://assignmentchef.com/product/solved-comp551-assignment-1-meansquare-error
<br>
You have to use Dataset-1 for this experiment. Dataset-1 consists of train, validation, and test files. The input is a real valued scalar and the output is also a real valued scalar. The dataset is generated from an <em>n</em>-degree polynomial and a small Gaussian noise is added to the target.

<ol>

 <li>Fit a 20-degree polynomial to the data. Report the training and validation MSE (MeanSquare Error). Do not use any regularization. Visualize the fit. Comment about the quality of the fit.</li>

 <li>Now add L2 regularization to your model. Vary the value of <em>λ </em>from 0 to 1. For different values of <em>λ</em>, plot the training MSE and the validation MSE. Pick the best value of <em>λ </em>and report the test performance for the corresponding model. Also visualize the fit for the chosen model. Comment about the quality of the fit.</li>

 <li>What do you think is the degree of the source polynomial? Can you infer that from thevisualization produced in the previous question?</li>

</ol>

<h1>2             Gradient Descent for Regression</h1>

You have to use Dataset-2 for this experiment. Dataset-2 consists of train, validation, and test files. The input is a real valued scalar and the output is also a real valued scalar.

<ol>

 <li>Fit a linear regression model to this dataset by using stochastic gradient descent. Youwill do online-SGD (with one example at a time). Use the step size of 1e-6. Compute the MSE on validation set for every epoch. Plot the learning curve i.e. training and validation MSE for every epoch.</li>

 <li>Try different step sizes and choose the best step size by using validation data. Reportthe test MSE of the chosen model.</li>

 <li>Visualize the fit for every epoch and report 5 visualizations which shows how the regression fit evolves during the training process.</li>

</ol>

<h1>3             Real life dataset</h1>

For this question, you will use the Communities and Crime Data Set from the UCI repository <a href="https://archive.ics.uci.edu/ml/datasets/Communities+and+Crime">(</a><a href="https://archive.ics.uci.edu/ml/datasets/Communities+and+Crime">http://archive.ics.uci.edu/ml/datasets/Communities+and+Crime</a><a href="https://archive.ics.uci.edu/ml/datasets/Communities+and+Crime">)</a>.

<ol>

 <li>This is a real-life data set and as such would not have the nice properties that we expect.Your first job is to make this dataset usable, by filling in all the missing values. Use the sample mean of each column to fill in the missing attribute. Is this is a good choice? What else might you use? If you have a better method, describe it, and you may use it for filling in the missing data. Turn in the completed data set.</li>

 <li>Fit the above data using linear regression. Report the 5-fold cross-validation error: TheMSE of the best fit achieved on test data, averaged over 5 different 80-20 splits, along with the parameters learnt for each of the five models.</li>

 <li>Use Ridge-regression on the above data. Repeat the experiment for different values of<em>λ</em>. Report the MSE for each value, on test data, averaged over 5 different 80-20 splits, along with the parameters learnt. Which value of <em>λ </em>gives the best fit? Is it possible to use the information you obtained during this experiment for feature selection? If so, what is the best fit you achieve with a reduced set of features?</li>

</ol>

<h2>Instructions on how to use 80-20 splits</h2>

<ol>

 <li>Make 5 different 80-20 splits in the data and name them as <em>CandC</em>−<em>train</em>h<em>num</em>i<em>.csv </em>and <em>CandC </em>− <em>test</em>h<em>num</em>i<em>.csv</em>.</li>

 <li>For all 5 datasets that you have generated, learn a regression model using the 80%data and test it using 20% data.</li>

 <li>Report the average MSE over these 5 different runs.</li>

</ol>

<a href="#_ftnref1" name="_ftn1">[1]</a> Because of a wrong date appearing on the slides in class, we’ll accept submissions until Jan 29 at <strong>noon</strong>. We recommend aiming for the original deadline since the second assignment will start Jan 26.