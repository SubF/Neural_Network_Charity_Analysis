# Neural_Network_Charity_Analysis

### Overview of Analysis

In this analysis we are analyzing a dataset of companies Alphabet Soup has invested in to predict whether applicants will be successful if funded by Alphabet Soup. 

### Results 

- What variable(s) are considered the target(s) for your model? The IS_SUCCESSFUL column is a target because it determines if the company was successful after the Alphabet Soup investment.
- What variable(s) are considered to be the features for your model? APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, and ASK_AMT.
- What variable(s) are neither targets nor features, and should be removed from the input data? EIN, NAME, and SPECIAL_CONSIDERATIONS
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
The final run had 2 layers with 80 and 30 neurons. The Relu function was used for the first two and Sigmoid was used for the output. A third hidden layer was removed due to loss of accuracy.
![This is an image](https://github.com/SubF/Neural_Network_Charity_Analysis/blob/main/images/1.png)
- Were you able to achieve the target model performance? I was not able to achieve the target 75% accuracy. The final result was 73.06%.
- What steps did you take to try and increase model performance?
1. Dropping the SPECIAL_CONSIDERATIONS column
2. Adding a third hidden layer (This was removed after it lowered accuracy)
3. Increasing the Epochs from 5 to 100

### Summary

After testing several iterations the highest accuracy reached was 73.06% which is below the target of 75%. 75% is a reasonable accuracy to aim for so I would suggest using Random Forest Classifier to analyze the data. This requires less processing power and will weight outliers better than the current neural network analysis.
