# Credit Card Fraud Detection
  Machine-Learning-Scala-

This dataset contains transactions made by European credit cardholders. 
(A)About Data-
1.Our Dataset is highly unbalanced with 492 Frauds and 284,315 non-fraudulent transactions.
2.It contains some numerical input variables which are the result of a PCA transformation. 
3.Unfortunately, due to confidentiality issues, more details about those transformed variables couldn’t be found.
4.dataset is 66MB small and consists of 30 columns.
5.As mentioned earlier, the dataset consists of columns from V1-V28 which are already scaled and transformed by PCA.
The only numerical columns we will be scaling are AMOUNT and TIME.
We also have “CLASS” as our target variable which has values 1 or 0
         1 – Fraudulent transactions
         0 – Non-Fraudulent transactions 
(B)Data Preprocessing-
Since we are dealing with a highly unbalanced Dataset with no NULL values, we perform under sampling on our scaled data.
We have made use of two under sampling techniques :
  	using  .sampleBy ()
    using weighted data
Stratified Sampling is used here.
(C)Feature Engineering-
the “time” and “amount” columns which are numeric, are scaled. Following techniques are used for scaling-
 Assembler
 Standardizer
 Minmax scaler
(D)Machine Learning Models-
  1.Logistic Regression model (LR)
  2.Gradient boosted Trees (GBT)
  3.Random Forest (RF) 
(E)Evaluation Metrics-
  1. Accuracy
  2. Area Under Curve(AUC)
  3. Probability
  4. ROC
(F)Results-We have learned from all the techniques of evaluation that Random Forest model has the higher level of accuracy when compared to the other two models with an AUC as 97%

