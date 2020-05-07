Required
1. Python 3.7
2.Jupiter Notebook


Merge and Join in Pandas
#
Pandas has full-featured, high performance in-memory join operations idiomatically very similar 
to relational databases like SQL.

Pandas provides a single function, merge, as the entry point for all standard database
join operations between DataFrame objects −

*****The generic Syntax for merge in Pandas*****

pd.merge(left, right, how='inner', on=None, left_on=None, right_on=None,left_index=False, right_index=False, sort=True)


Here, we have used the following parameters −

left − A DataFrame object.

right − Another DataFrame object.

on − Columns (names) to join on. Must be found in both the left and right DataFrame objects.

left_on − Columns from the left DataFrame to use as keys. Can either be column names or arrays with length equal to the length of the DataFrame.

right_on − Columns from the right DataFrame to use as keys. Can either be column names or arrays with length equal to the length of the DataFrame.

left_index − If True, use the index (row labels) from the left DataFrame as its join key(s). In case of a DataFrame with a MultiIndex (hierarchical), the number of levels must match the number of join keys from the right DataFrame.

right_index − Same usage as left_index for the right DataFrame.

how − One of 'left', 'right', 'outer', 'inner'. Defaults to inner. Each method has been described below.

sort − Sort the result DataFrame by the join keys in lexicographical order. Defaults to True, setting to False will improve the performance substantially in many cases.

Let us now create two different DataFrames and perform the merging operations on it.

**********
