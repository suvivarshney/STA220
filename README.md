# STA220
Repository for the Project of the Course: STA220

To scrape the data from Bookings.com - 
1. Run the cells from Code/Scrape_Bookings_Data.ipynb
2. Since the google collab RAM crashes due to excessive data, data is scraped in chunks.
3. Before running the cell with function scrape_hotels_list(city_), set the range in the for loop with number of hotels you want to scrape at a time. It is recomended to run only 50 hotels at a time so loop would be like for i in range(0,50,25). This would run loop only 2 times with offset 0 and 25 and load first 50 hotels.
4. By defualt code runs for Los Angeles. Change cities[1] and cities[1][0] in the second last cell to cities[2] and cities[2][0] or cities[3] and city[3][0] if you wish to run for San Diego or Sacramento respectively
5. Change Json files names in the last cells based on the city and the number of run.

To perform the sentiment analysis - 
1. Run the cells from Code/Sentiment_Analysis.ipynb
2. Run celss 4-9 to load all json files by changing the name of json file in cell 4 and csv file in cell 9.
3. Merge all csv files into a single file 'scrapping_data_final.csv' and then continue running the cells from cell 10.
4. You should be able to clean the data, run models and visualize the results from models.
