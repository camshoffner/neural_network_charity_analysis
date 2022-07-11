# Neural Network Charity Analysis

## Objective
A team member, Beks, has been working towards forecasting profitable investments for Alphabet Soup.  Aiding her assessment, a binary classifier has been created using neural networks to find patterns amongst 34,000 potential organizations.  

## Results
### Data Prepping
* Given we wanted successful investments, the ""IS_SUCCESSFUL" Column was our target.
* After much testing, the values that were kept as ______ were Name, Application Type, Affiliation, Classification, Organization, Status, Special Considerations, Ask Amount. 
* The EIN and INCOME_AMT were dropped due to lack of information and weren't beneficial to knowing whether the investment would be successful. 

### Compiling, Training, and Evalutating Model
* For compute purposes, the nodes and layers were minimized to two layers with 
* By adding back the Name column that was initially dropped, the target 75% was acheived.  
* Intiially, the fields stayed constant as the layers and neurons were manipulated.  After many failed attempts, the fields were tested by removing a few, such as Special Consieration and Status, and regrouping most of the catagories. The Name category was reintroduced after recoginzing the same organization is listed multiple times.  After reintroduction, the layers and neurons were retested.  

## Summary
The final model had to run over 100 epochs to consistently hit 75% accuracy.  The modeled used three hidden layers and an output layer, neurons ranging from 20 to 1 on the output. The hidden layers relied on the ReLu activation function, and the output used tanh.  The percentage is still low, so it may be worth to look at another type of supervized machine learning.  Random Forest may be beneficial, so weights can be given to the parameters that may be most influencial.  
