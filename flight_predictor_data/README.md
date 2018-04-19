## Problem Statement

Laxman is a paragliding enthusiast. There are several spots for paragliding in his country but these spots are far away from his home so he has to leave his home to one of these spots early in the morning. Often after reaching the paragliding spot, he finds that weather conditions are not good for paragliding and it may be dangerous to paraglide in those conditions.

There are 5 weather stations near these paragliding spots. Every day around 2 AM weather data is collected for 45 heights at equal height intervals at each of these stations. Weather data collected includes pressure, temperature, dew point, wind speed and wind direction for each height. Using this weather data Laxman wants to predict whether it will be a good day or bad day for paragliding. He has been collecting paragliding data for several years. This data includes flight details for 288 paragliding spots for several days. Flight details for each spot include max distance, total distance, number of flights that took place at that spot on a particular day. He has also concluded that if the total number of flights combining all these spots is more than or equal to 15 then it is good day else it is a bad day for paragliding. 

Laxman wants you to help him to predict good(1) or bad(0) day based on the weather data for a day. The training data includes flight data and weather data with 2183 rows in each of them. Test data includes weather data for 100 days for which you have to make predictions. 

Laxman knows that some of the factors responsible for a bad day are rain, high-speed winds, and the high-pressure difference between height levels. He also knows that sometimes sensor devices at weather stations record wrong weather parameters so it would be great if you could take care of that as well. 

## Approach

1. Create the target column using the given condition.
2. Merge the target column into the weather data.
3. Remove outliers (some of the rows had wind speed negative).
4. Train the dataset on LightGBM classifier.
5. Got 76% accuracy.
