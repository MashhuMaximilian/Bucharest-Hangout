# Best City in the US for Coffee Lovers

*Applied Data Science Capstone - IBM Data Science Professional Certificate by IBM on Coursera*



## Introduction 

Coffee is one of the most consumed beverages in the world. One can say that, even on vacations, you cannot survive without it. Therefore, I took this thought in practice and though:
"What if I were to go to the USA, for travel, where should I go to drink coffee from as many coffee stores as possible, in proximity to my hotel."

So I want to go to a place with a high density of Coffee Shops around me.

The problem we aim to solve is that different cities have different layouts and citizens with different preferences, which may favor or inhibit the proximity of a coffee shop to another.

We must, therefore, analyze the Coffee Shops' locations in some of the major US cities and find the best place for our tourists so that they can have a good coffee.



## Data section 

I will use the FourSquare API to collect data about locations of Coffee Shops in 5 major US cities which are: Los Angeles, Seattle, San Francisco, Houston, and Boston. These are one of the most populated US cities and I am hopeful that they will contain the best coffee shops in the US.

After collecting them, my main target here is to asses which city would have the highest Coffee shop density. I used the Four Square API through the venues channel. I used the near query to get venues in the cities. Also, I use the CategoryID to set it to show only Coffee Shops.

Moreover, I repeated this request for the 5 studied cities and got their top 100 venues. I saved the name and coordinate data only from the result and plotted them on the map for visual inspection.

Next, to get an indicator of the density of Coffee shops, I calculated a center coordinate of the venues to get the mean longitude and latitude values. Then I calculated the mean of the Euclidean distance from each venue to the mean coordinates. That was my indicator; mean distance to the mean coordinate.
