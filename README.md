# DevSoc01
DevSoc Module 0  (AI/ML) 

# Linear Regression from Scratch

I wanted to understand how linear regression works, so instead of just calling linear regression directly, I wrote it with NumPy which is a library to perform mathematical operations, usually on arrays. The model learns to predict house prices using gradient descent, and uses scikit-learn for the train/test split and the scoring metrics.

## while running it

1. The housing data gets loaded. We drop `Price` (that's what we're predicting) and `Address` (it's text, so it can't go into the maths).
2. 80% of the houses are used for training and 20% are kept hidden for testing.
3. Everything gets normalised so the features are on a similar scale. The scaling numbers come from the training data only, so the test set stays truly unseen and the evaluation process is accurate.
4. The model trains for 2000 rounds of gradient descent. Each round it checks how wrong it is and nudges the weights to be a bit less wrong.
5. A graph shows the error decreasing over time, so you can see that it actually learned something.
6. Finally it predicts prices for the test houses, converts them back to dollars, and prints RMSE and R²(error metrics). The second graph compares actual vs predicted prices.


## to run it

Install what you need:

run on terminal
pip install pandas numpy matplotlib scikit-learn


Keep `Module_0.py` and `USA_Housing.csv` in the same folder and run:

python Module_0.py

