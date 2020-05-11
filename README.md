# Data-Analysis-of-emergency-calls-made-to-911
This data contains the latitude,longitude,city,zip code,type,time and date and the address of the particular 911 call made.
I found out the top 5 zipcodes and top 5 towns from where the 911 calls were made.
I created a new column named Reasons.This column contains the actual reason of the 911 call. This column was produced by extracting the data from the title column. A count plot was made for the Reason column.
I used the timestamp columns to get separate columns for days,month and hour. In this process ,days was present in the form of integers with Monday as 0. I managed to change that index to 1 and so on.
A countplot of Day of the Week column was plotted with hue based on Reason column. To maintain unifomity, all palettes of seaborn plots have been named to 'viridis'.
The same plot was done with the Week column. Where it was figured that certain information was missing for months 9 ,10 and 11. This problem was eliminated by making a lineplot. To make the lineplot, the dataframe was grouped by the month column.
A plot is then created between the number of calls per month.
A new date column is created from the timestamp column.
A plot is created to count the number of calls on a given date.
3 different plots are created based on reason to find the number of calls made for a particular reason on any given date.
The dataframe is restructured in such a way that hour becomes the coloumn and the day of the week as its index.
A new heatmap is created between day of the week and the hour column.
A new clustermap is created between day of the week and the hour column.
A similar process is followed with the day of the week and month column.
