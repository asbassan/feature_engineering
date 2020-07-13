### To rename the columns of a pandas dataframe:
  1. using lambda:
     news_df.rename(columns=lambda x: x[1:], inplace=True)
  2. Using str replace
     df.columns = df.columns.str.replace('$','')
  3. if I know the names to new names mapping:
     df.rename({'a': 'X', 'b': 'Y'}, axis=1, inplace=True)
