# Project 1: <font color='crimson'>Airbnb Trends in Mexico City</font>

*How do Airbnbs get booked?*

This repository is a Python library with Jupyter Notebooks of a group analysis that identified the elements that help Airbnb hosts perform best in a highly competitive market, such as Mexico City. Here you will find:

## The link to our slide deck

[Google Slides deck](https://docs.google.com/presentation/d/1ackgipuGAcztUlJ_ftdtSCkch9yrqRrdwPKUquYkFho/)

## The *Output_data* folder

Contains all the figures —bar charts, boxplots, and scatterplots— and maps generated as part of the analysis.

## The *Resources* folder

Contains two CSV files and two shapefiles: 
- ```listings-complete.csv``` has a sample of the data with which we worked. The original file was over 100 MB, therefore, please be aware that the data you will find in the Jupyter Notebooks, the data of our slide deck, and the data you might find in your calculations will be slightly different.
- ```listings_data.csv``` has the clean data we used in our analysis.
- ```poligonos_alcaldias_cdmx.dbf``` has the polygons of the districts of Mexico City.
- ```poligonos_alcaldias_cdmx.shp``` also has the polygons of the districts of Mexico City.

## The *project_1_data_analysis.ipynb* Jupyter Notebook
It is the code we used to clean the data before our analysis.

## The *project_1_exploration_and_cleanup.ipynb* Jupyter Notebook
It is the code we used to perform our analysis.

## Our written analysis

We had three questions at the beginning of the analysis:
1. What are the most relevant factors for getting high score rating for hosts?
2. What are the most important factors when it comes to maintaining a high occupancy rate for hosts? 
3. What does the competitive landscape for Airbnb hosts look like in Mexico City?

### First answer: accuracy, communication, and cleanliness!

Based on score rating that reservations receive in website Airbnb from customers, people appreciate the most the following three factors: Accuracy, communication and Cleanliness.

![image](https://user-images.githubusercontent.com/118868483/220541567-af6e2634-4a89-4432-9720-a6b0745df11b.png)

Accuracy came first in our analysis since guests are looking for extensive booking details, specific room types, amenities, a room that looks exactly as the website pictures depicted it. Then, we found that communication is also highly appreciated by customers because they expect their hosts to respond to multiple inquiries and, above all, to solve unexpected issues that may arise during stays. The third important factor we identified was cleanliness. The lack of it is closely associated to health risks for guests and their travel companions (mold, pests or vermin). Guests tend to rate their hosts in terms of how often cleaning takes place.

In terms of review scores, the score for communication and the one for the check-in process are strongly correlated (r(23013)=.85, *p*<0.01). This means that both scores move in the same direction, so a high score in communication is related to a high score in the check-in.
![image](https://user-images.githubusercontent.com/118868483/220541624-7764b487-03ee-40bc-941e-b4f9074a389c.png)

 

Despite of what everyone may think, location is less relevant than the abovementioned factors with a correlation vs. rating score of only .72. 
 

![image](https://user-images.githubusercontent.com/118868483/220541660-45c25397-1b89-428f-80cd-a21b4207e2c8.png)

```#Thank you for reading me!```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
