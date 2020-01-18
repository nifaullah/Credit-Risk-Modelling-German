# Credit-Risk-Modelling-German-
EDA, Classifier analysis, Simulated cost analysis and Model development on German Credit data

Data: The dataset contains 1000 entries with 20 categorial/symbolic attributes prepared by Prof. Hofmann. In this dataset, each entry represents a person who takes a credit by a bank. Each person is classified as good or bad credit risks according to the set of attributes. Link for the dataset - https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29

Goal: Find the best model which classifies potential loans as bad risk or good risk.

Approach: 
  1. First perform extensive EDA to yeild influencing features.
  2. Use precision scores from Cross-Validation technique to shortlist the number of classifiers.
  3. Run shortlisted classifiers against a series of Standard Classifiers Performance Measures.
  4. Run simulated analysis of assymetric cost and then finalize model.
 
Major Finding:
  1. Random forest is the best classifier in terms of returns based on the simulated cost analysis.
  2. As the number of applicants increase over time, overall all models are profitable.
  
Recommendation:

It is recommend that the potential loans are to be broadly divided into three categories  low, medium and High on the basis of the loan amount. 

For low & medium risk loans model can be directly applied category wise, even though it is likely to wrongly term few bad loans as good loans but over a long period of time, as corroborated by cost analysis, the model is still profitable by huge margin. 

For High loan amounts model can be used as a filtering system, which filters out applications at the initial level, after loans are filtered through, it is recommended that bank follows a rigorous systemic process to reverify these applicants.
