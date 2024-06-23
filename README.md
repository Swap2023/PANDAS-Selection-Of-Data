# PANDAS-Selection-Of-Data #
For Selecting The Data
1. s.loc / s.iloc - s.loc[‘index’] , s.loc[‘index1’:’index2’] , s.iloc[0] , s.iloc[0:3] 
# Selection by object Index and Selection by integer Index. 
2. Series Indexing - s[0] , s[‘index’] , s.index , s[0:5] , s[‘index1’:’index2’] , s[0:-1] , s[-3,-1] , s[::-1] 
3. Boolean Series Indexing - s[s>=20] # Show a new series with boolean condition satisfied.
4. df[‘Col_name’] , df.Col_name # Selecting single column from the DF.
5. df[[‘Col1’, ‘Col2’ , ‘Col3’ ]] # Selecting multiple Columns from the DF.
6. df.iloc[ : , [1, 3, 5 ]] # Selecting multiple Columns from the DF.
7. df.loc[ : , ‘Col1’ : ‘Col2’] # Selecting columns with object slicing.
8. df.iloc[ : , 1:4 ] # Selecting columns with integer slicing.
 
9. df.loc[‘Row_index’] # Selecting single row from the DF.
10. df.loc[[‘index1’ , ‘index2’ , ‘index3’ ]] # Selecting multiple rows from the DF.
11. df.iloc[[1, 3 , 5 ]] # Selecting multiple rows from the DF.
12. df[‘index1’ : ‘index2’ ] - df[‘P’ : ‘R’] # Selecting rows with object slicing.
13. df[index1 : index2] - df[1:3] # Selecting rows with integer slicing.
14. df.loc[‘index1’ : ‘index2’ , ‘Col1’ : ‘Col2’] # Selecting rows & columns with slicing using loc( ). 
15. df.iloc[ 1:3 , 1:3] # Selecting rows & columns with slicing using iloc ( ).
16. df.loc[‘row_label’ , ‘col_label’] # Selecting one row and one column by label.
17. df.iloc[‘row_index’ , ‘col_index’] # Selecting one row and one column by index.
18. df.iloc[[2,4,6],[2,4,6]] # Selecting multiple rows & multiple columns.
19. df>3 , df[df>3] # Showing the elements of the DF which are greater than 3.
20. data.loc["2012-01-06", 'Stn Press (kPa)'][2:4]
21. Selecting columns by data-type - df.select_dtypes(include = 'number' / ‘int’ / ‘float’ / ‘object’)
df.select_dtypes(include = [‘object’ , ‘number’ , ‘category’ , ‘datetime’] ) 
df.select_dtypes(exclude = 'number' / ‘int’ / ‘float’ / ‘object’
