# Erdoes_Waldo

Instructions for the Data Sets.

Statistical Moments for the Full Image:
- Waldo_Mom_df.csv
- NW_Mom_df.csv  

Clearly, one of the contains all the moments for the Waldo Images and the other the remainder  
The Full Dataframe can be constructed with the following command:  
Full_data = pd.concat([Waldo_Mom_df,NW_Mom_df])  

Notice that NW_Mom_df has NaN entries. To remove them simply do:  
Full_data.fillna(0, inplace = True)  


The Statistical Moments for Dominant Channel Images are also contained in the files:
- DomW_moments_df.csv
- DomNW_moments_df  

The same comments apply to this set. Remember the whole set can be combined with:

Extended_df = pd.concat([df1, df2], axis=1).reindex(df1.index)
