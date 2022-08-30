# Categorical-Features-Encoding

   In this project, you was predicting the probability [0, 1] of a binary target column called cat.
   The structer dataset  contains binary features , nominal features , ordinal features  as well as (potentially cyclical) day (of the week) and month features, aand     in this project we tried to encoding with diffents methodes:

# 1-binary features:

   features that contain exactly two classes, for example, 0/1, or positive/negative, or on/off.

# 2-nominal features:

   This type of categorical data consists of the name variable without any numerical values.
 
   a-if we have low-cardinality (<15) use for encoding:
   

   b-high-cardinality (>15):

   -Hash encoding:
 
   uses a hash function to map each categorical value in the variable to a unique random number. It’s similar to one-hot encoding but more flexible as it allows us to   determine the number of dimension we want to output. The advantage of the hash encoding is lower number of dimensions. However, it can lead to collision of hash numbers in cases where we have large number of categorical features.

   -Frequency Encoding:
    
   we count the number of observation for each category and replace the specific value with its equivalent number of occurrence.

   -Target encoder:

   by computing the average of the target variable for each value of the categorical variable and replacing the calculated mean with the categorical value.

   -LeaveOneOut Encoder:

# 3-ordinal features:

   This type of categorical data consists of a set of orders or scales.



# 4-(potentially) cyclical features (time like day, month):

   A common method for encoding cyclical data is to transform the data into two dimensions using a sine and consine transformation.

   We can do that using the following transformations:

   xsin=sin(2∗π∗xmax(x)) 
   xcos=cos(2∗π∗xmax(x))

Now we go to the fundamental question , Do I have to stick to these methods for every type?

   Let me tell you that you don't have to necessity, and that's what the project explains , find it in file (the best cat-encoding-0.80286-in-private-lb) and the   coding for the Previous methods in file (catecorigal features).

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# TOOLES:
 
   -Language of programming python
 
   -Dataset form  kaggle (https://www.kaggle.com/competitions/cat-in-the-dat)
 
 
 
