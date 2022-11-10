# Airbnb-in-Madrid
This project was completed as part of the Data Science Nanodegree (Udacity) in November 2022 by José Imedio.

It aims at answering the following main question: 
  - What is the best spot/area to stay in Madrid (Spain)?

In order to do that, data from Airbnb in Madrid was used (http://insideairbnb.com/get-the-data/). 
After filtering the database, we plotted the data on a scatter plot, using the latitude and longitude information to make it geographically consistent. Then, we went over it and created a grid with general information of each small region. We repeated this process three times, in order to answer the following three subquestions:
  - Where do people tend to give a higher location rating?
  - Where are there more options to choose from?
  - Are the best areas too expensive?

#### Blog post on Medium: https://cutt.ly/xMtuZ2Y

## List of files

#### Project I - AirBnB in Madrid
Jupyter Notebook, main code file.
#### listings
Zip file containing data from Airbnb in Madrid (http://insideairbnb.com/get-the-data/). It needs to be unzipped and saved in the same folder as the other file.


## Libraries used

#### numpy
Mathematical and logical operations on arrays.
#### pandas 
Data analysis.
#### matplotlib
Data visualization.
#### math
Additional mathematical operations.


## Comments on the process
Firstly, it is important to note that we used the location score and not the general score as the main source of information. 

During the data filtering process, we realized that accommodations with a low number of reviews tended to have very high scores. So we had to drop those rows to make sure the data we were using was as objective as possible.

Some geographical references were included on every scatter plot. That way, drawing conclusions became easier.

In order to create the grid, different sizes were tried. The one that yielded the most visual results was 1 square km (approx.). This is equivalent to a rectangle of 0.009 degrees of latitude by 0.012 degrees of longitude (https://www.johndcook.com/how_big_is_a_degree.html). 

Finally, it was necessary to filter the results again before making the scatter plots. This is because the presence of outliers made the color code way less informative. And thus, the scatter plots less visual.


## Results

#### Where do people tend to give a higher location rating?
We can see the preferred areas by Airbnb users include most of the Centro district (only excluding the west end) and the west half of the Salamanca neighborhood (https://misstourist.com/wp-content/uploads/2022/01/Map-of-best-places-to-stay-in-Madrid-660x440@2x.jpg).
#### Where are there more options to choose from?
Here it's very clear that the surroundings of Puerta del Sol have the highest amount of accommodations.
#### Are the best areas too expensive?
The most expensive areas are not among the ones mentioned in the previous two questions. The prices at the preferred areas are intermediate or high-intermediate.

## Conclusion
It seems that Puerta del Sol and its surroundings are the best areas to stay in Madrid for the general public. It's one of the preferred areas, it offers a great variety of options and it's not among the most expensive.


