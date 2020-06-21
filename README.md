# PyBer_Analysis

Paragraph 1

- The overarching purpose of this assignment was to dig into the driver, ride, and city data to uncover trends that are specific to, for example, how the average fare per driver in city types compare with each other.  Mixing and matching various data points and comparing to other data points while changing the conditions allowed us to identify interesting trends, such as how rural city types have fewer driver AND rides, BUT more profitable average fares. 
- Many individual tasks were taken to produce the deliverables, but the most notable ones that I can think of are 1) merging ride and city data to produce a more comprehensive data set for more advanced/custom calculations and 2) creating smaller, individual average fare/total rides plots and then combining them into a one plot that show many different trends. I also identified some interested trends around standard deviation, as well as outlier fare prices in certain cities.
- The final summary and multi-line graph show us a few things.  One, most of the fare amounts for each week follow approximately the same up and down trends with some exceptions.  The Urban areas have many more drivers and ride and make the company more money overall, but my guess is that the rural areas are more profitable since there are fewer driver/rides but higher fares.

![](analysis/Fig8Challenge_Multi_Line_Plot.png)

![](analysis/PyBer_Summary_Df.png)

- Short summary of results: Suburban fare amounts by week start to spike in the middle of April, which may be a seasonal effect like warmer weather making people want to hail rides more often.   Urban areas dominate when it comes to having the most rides and ESPECIALLY the most drivers.  It seems that there may be more drivers than necessary for the urban areas which drives the average fare down, vs the rural areas which have fewer drivers but higher fares.  

Paragraph 2

- I encountered some technical challenges with things like resample and pd.to_datetime, both of which are crucial for creating plots of time series data.  Through readin much documentation and a little help from the TAs, I was able to overcome this. 
- One example of a technical challenge I overcame was using the loc function to identify a very specific timeframe: "2019-01-01":"2019-04-28".  I read multiple examples of documentation from both stackoverflow and hyperlinked resources in the module to find the right syntax.  Another challenge was figuring out the syntax for resampling data by "W" and then using the sum() aggregate.   After some trial and error and replacing brackets with parentheses, I was able to fix it.

Paragraph 3

- One recommendation would be to do additional data analysis on suburban drivers to see how many of them normally drive within reasonable distance of rural cities and then create an incentive program to entice those suburban drivers to drive out to rural areas and perform rides there as well.  Coordinated ride sharing from rural areas to large suburban or even urban areas could help increase the overall number of rides in the rural areas and help cut down on average fare costs for riders. 
- As mentioned above, my first additional analysis would be to get another data set of ride/fares by specific zip codes vs general city types.  I would then do a second analsis (if legally allowed) on the ages of the riders in order find opportunities to better serve senior citizens with things like special discounts, etc.  
- I would take technical steps such as downloading and merging data sets that include ride/fare by zipcode and by rider age and merge them into the dataset that we used for this challenge and create some additional finds such as: 
    1) A dataframe of how many riders in suburban or urban areas are within reason driving distance of a rural area and what the difference in fares gained from servicing rural areas would be.  These differences in average fare between surburban and rural city types could then be highlighted to drivers who may then in turn ask for more information on how to serve those communities. 
    2) A pie chart showing riders by age groups of every 10 years (10-20 yr olds, 50-60 yr olds, etc).  If certain age groups are very underserved based on the number of total riders in each age group, then there could be opportunity to offer more rides to them and learn more about their needs.
