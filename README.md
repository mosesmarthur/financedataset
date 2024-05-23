# Financeusecase

# Dataset information

df_train.csv - Data columns (total 22 columns):

Column 0 : Cutomer id
Column 1-20 :  features to train
Column 20 : target variable to classify


 #   Column     Non-Null Count  Dtype  <br />
---  ------     --------------  -----  <br />
 0   Customer   6700 non-null   int64  <br />
 1   feat1      6700 non-null   float64 <br />
 2   feat2      6700 non-null   float64 <br />
 3   feat3      6700 non-null   float64<br />
 4   feat4      6700 non-null   float64<br />
 5   feat5      6700 non-null   float64<br />
 6   feat6      6700 non-null   float64<br />
 7   feat7      6700 non-null   float64<br />
 8   feat8      6700 non-null   float64<br />
 9   feat9      6700 non-null   float64<br />
 10  feat10     6700 non-null   float64<br />
 11  feat11     6700 non-null   float64<br />
 12  feat12     6700 non-null   float64<br />
 13  feat13     6700 non-null   float64<br />
 14  feat14     6700 non-null   float64<br />
 15  feat15     6700 non-null   float64<br />
 16  feat16     6700 non-null   float64<br />
 17  feat17     6700 non-null   float64<br />
 18  feat18     6700 non-null   float64<br />
 19  feat19     6700 non-null   float64<br />
 20  feat20     6700 non-null   float64<br />
 21  Y          6700 non-null   int64  <br />
dtypes: float64(20), int64(2)<br />

df_test.csv - Data columns (total 20 columns):<br />
 #   Column  Non-Null Count  Dtype  <br />
---  ------  --------------  -----  <br />
 0   feat1   3300 non-null   float64<br />
 1   feat2   3300 non-null   float64<br />
 2   feat3   3300 non-null   float64<br />
 3   feat4   3300 non-null   float64<br />
 4   feat5   3300 non-null   float64<br />
 5   feat6   3300 non-null   float64<br />
 6   feat7   3300 non-null   float64<br />
 7   feat8   3300 non-null   float64<br />
 8   feat9   3300 non-null   float64<br />
 9   feat10  3300 non-null   float64<br />
 10  feat11  3300 non-null   float64<br />
 11  feat12  3300 non-null   float64<br />
 12  feat13  3300 non-null   float64<br />
 13  feat14  3300 non-null   float64<br />
 14  feat15  3300 non-null   float64<br />
 15  feat16  3300 non-null   float64<br />
 16  feat17  3300 non-null   float64<br />
 17  feat18  3300 non-null   float64<br />
 18  feat19  3300 non-null   float64<br />
 19  feat20  3300 non-null   float64<br />
dtypes: float64(20)


# Description about the dataset

df_train.csv: 6700 rows x 22 columns

- Customer column is the unique id of each customer
- From the features 1-20, the customer are classfied into 3 classes which reflects in cloumn 22 (Y)

    Cluster 2: 681 values
    Cluster 0: 1346 values
    Cluster 1: 4673 values

- Most of the customer are present in Cluster 1 (this data is biased)


df_test.csv : 3300 rows x 21 columns
- Customer column is the unique id of each customer
- From the features 1-20, we could build ml model to classify and predict the column Y

# Scripts
- mlmodel.ipynb : Has list of machine learning model and output
- deploytolambda.ipy : how the same model can used in AWS 
