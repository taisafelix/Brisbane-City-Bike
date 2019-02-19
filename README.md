# Brisbane-City-Bike
Performing a clustering based on the location of bike stations in Brisbane


First five lines of Brisbane_CityBike.json file: 

![data](https://user-images.githubusercontent.com/39279175/53047722-57d62680-3493-11e9-8847-1ce88bf5808a.PNG)


The algorithm used to do the clustering was K-means, wich is unsupervised learning algorithm. The data is grouped according to feature similarity, in this case this similarity is represented by the Euclidian distance between the stations. 

The K-means algorithm has a major drawback: it's necessary to provide the required number of clusters. Therefore, the first step was to find the optimal number of clusters. 

![opt_n_clusters](https://user-images.githubusercontent.com/39279175/53047873-b00d2880-3493-11e9-90a8-0f033e3460ee.PNG)

As it's possible to verify at the picture above, the optimal number of clusters for the bike station is 3. 


With the number of clusters it's was possible to divide the bike stations in 3 clusters. To do that the function KMeans (avaliable in sklearn library) was used.

The results can be observed in the picture bellow:

![clusters](https://user-images.githubusercontent.com/39279175/53047878-b13e5580-3493-11e9-9d6b-1e6a996779cf.PNG)
