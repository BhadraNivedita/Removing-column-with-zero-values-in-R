# Removing-column-with-zero-values-in-R

It is very common to receive a dataset for analyses which consists of columns filled with zeros. We can create subset of a dataframe which does not have a column filled with only zeros. If DF is the dataset and DF_complete is the dataset after removing the columns only with zero values, the below code example can do the tast.

```
DF_complete<-DF[,colSums(is.na(DF)) == 0] 
'''
