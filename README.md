# Airbnb Trends in Mexico City 2022

*How do Airbnbs get booked?*

This repository is a Python library with Jupyter Notebooks of our team's analysis that identified the elements that help Airbnb hosts perform best in a highly competitive market, such as Mexico City. Here you will find:

## Authors

[Alejandra Espinosa](https://github.com/zuntaalejandra)
[Daniel R. Murillo Antuna](https://github.com/dan-murillo)
[Aldo Silva](https://github.com/aldosilesp)

## The link to our slide deck

[Google Slides deck](https://docs.google.com/presentation/d/1ackgipuGAcztUlJ_ftdtSCkch9yrqRrdwPKUquYkFho/)

## The '*Output_data*' folder

Contains all the figures —bar charts, boxplots, and scatterplots— and maps generated as part of the analysis.

## The '*Resources*' folder

Contains two CSV files and two shapefiles: 
- ```listings-complete.csv``` has a sample of the data with which we worked. The original file was over 100 MB, therefore, please be aware that the data you will find in the Jupyter Notebooks, the data of our slide deck, and the data you might find in your calculations will be slightly different.
- ```listings_data.csv``` has the clean data we used in our analysis.
- ```poligonos_alcaldias_cdmx.dbf``` has the polygons of the districts of Mexico City.
- ```poligonos_alcaldias_cdmx.shp``` also has the polygons of the districts of Mexico City.

## The '*project_1_data_analysis.ipynb*' Jupyter Notebook
It is the code we used to clean the data before our analysis.

## The '*project_1_exploration_and_cleanup.ipynb*' Jupyter Notebook
It is the code we used to perform our analysis.

## Our written analysis

We had three questions at the beginning of the analysis:
1. What are the most relevant factors for getting high score rating for hosts?
2. What are the most important factors when it comes to maintaining a high occupancy rate for hosts? 
3. What does the competitive landscape for Airbnb hosts look like in Mexico City?

### First answer: accuracy, communication, and cleanliness!

Based on the score rating that bookings receive, guests mostly appreciate accuracy, communication, and cleanliness.

![image](https://user-images.githubusercontent.com/118868483/220541567-af6e2634-4a89-4432-9720-a6b0745df11b.png)

Accuracy came first in our analysis since guests are looking for extensive booking details, specific room types, amenities, a room that looks exactly as the website pictures depicted it. Then, we found that communication is also highly appreciated by customers because they expect their hosts to respond to multiple inquiries and, above all, to solve unexpected issues that may arise during stays. The third important factor we identified was cleanliness. The lack of it is closely associated to health risks for guests and their travel companions (mold, pests or vermin). Guests tend to rate their hosts in terms of how often cleaning takes place.

In terms of review scores, the score for communication and the one for the check-in process are strongly positively correlated (r(23013)=.85, *p*<0.01). This means that both scores move in the same direction, so a high score in communication is related to a high score in the check-in.

![image](https://user-images.githubusercontent.com/118868483/220541624-7764b487-03ee-40bc-941e-b4f9074a389c.png)

Moreover, despite what everyone may think, location is less relevant than the abovementioned factors —a weaker correlation between location and rating score was found: r(23013)=.72, *p*<0.01. 

![image](https://user-images.githubusercontent.com/118868483/220541660-45c25397-1b89-428f-80cd-a21b4207e2c8.png)

### Second answer: have an instant-bookable listing and a profile photo. 

Our analysis revealed that the variables that had a larger impact on occupation are boolean; most importantly, having an instant-bookable listing and having a profile picture. However, being a super host and having a verified identity also helped – although not as much.

![image](https://github.com/aldosilesp/project-1/blob/main/Output_data/barchart-Superhost_occupancy.png)

On the other hand, having a high review score did not have a big impact on occupation rate. However, if we could point out a single factor that determined the place where a guest decided to stay is the location —yes, *it's location, location, location!* Guests tended to be more willing to overlook poor reviews, the lack of a profile picture, and other factors, as long as the place was located in a very desirable area.


### Final answer: the city center, its surroundings, and the west are competitive; the southeast is not.

In terms of occupancy rate, the city center and its surroundings were the most competitive, whereas the southeast was not. The busiests Airbnbs tended to be around the center of Mexico City, although they were mostly just west and south of the center. The Cuauhtémoc, the Iztacalco, and the Coyoacán district had the highest occupancy rates most likely due to the many tourist and historical attractions and the closeness of the former two to the central international airport. On the contrary, the southeast region, where we can find the Xochimilco, the Milpa Alta, and the Tláhuac districts, was the emptiest. This could be due to how generally uninhabited that region is.

![image](https://github.com/aldosilesp/project-1/blob/main/Output_data/map-Median%20yearly%20occupancy%20rate%20per%20district.png)

Based on price, the west was more competitive than the east. The priciest listings were found in the Miguel Hidalgo, the Cuajimalpa de Morelos, and the Cuauhtémoc districts, while the most economic were in Tláhuac and Iztapalapa. The Cuauhtémoc district was probably the busiest area in the city, and that could explain its high prices. Conversely, the east was inmensely less busy, and one of its main attractions is ecotourism, as opposed to more traditional touristic attractions —less tourists seemed to stay in those areas, which could explain the extremely economic listings found there.

![image](https://github.com/aldosilesp/project-1/blob/main/Output_data/map-Median%20price%20per%20night%20per%20district.png)

The number of Airbnbs per district revealed that the west was by far the most competitive area of Mexico City, whereas the southeast seemed the least competitive. The number of listings in the city was highly polarized. Almost two thirds of all the Airbnbs were found in the Cuauhtémoc district. On the other hand, apart from the Miguel Hidalgo and the Benito Juárez districts, the concentration rate of listings of the rest were much less than ten percent combined.

![image](https://github.com/aldosilesp/project-1/blob/main/Output_data/map-Concentration%20rate%20of%20listings%20per%20district.png)

In conclusion, the rating scores for accuracy, communication, and cleanliness are the most important factors for a general high score. It helps if the listing is instant-bookable and the host has a profile picture. The city center, its western and southern surroundings, and the west are currently the most competitive areas of Mexico City, whereas the southeast is practically deserted. Future studies should determine whether there is a correlation, or even causation, between the yearly occupancy rate and the concentration rate of listings in Mexico City. They could also establish whether there is potential in the southeast for more competition in the years to come, and dive deeper into the context of future data to find more trends, mainly causality and predictive models.

## Sources

The dataset used in our analysis was downloaded from insideairbnb.com. The website contains free, open data about Airbnb and its listings. The analysis was based on data from Mexico City published on December 2022.

```#Thank you for reading me!```
<br>
<br>

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
