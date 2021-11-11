# Car price in auction, Which feature matter more?

# Dataset

The dataset is about car price in auction.It contains about 558,811 data points and 16 features .
The features are:
- year: The year of production
- make: the brand of the car
- model: eddition name of the car
- trim: the level or the virsion of the model
- body: body type or the style of the vehicle 
- transmission: transmission type( Automatic, Manual 
- vin: Vehicle identification number 
- state: the state where the car is auctioned
- condition: the rating of the car at the time of the auction(5=excellent, 4=very good, 3=good, 2=fair, 1=poor )
- odometer: the distance traveled by a vehicle
- color:  exterior color of the car
- interior: interior color of the car
- seller: the seller of the car , or the car dealer
- mmr: Manheim Market Report is the estimated price of the car in the market whch is done by Manheim company and it is refereshed every night in order to provide accurate price
- sellingprice: the price of the car when it was sold at the auction
- saledate: the date when the car was sold at auction

# Problem 

- What are the main features that affect the price of used car?
- What is the relation between odometer & selling price?
- Should the seller trust MMR (Manheim Market Report)?
- What is the relation between the sellingprice and the age of the car?
- can we predict the selling price for used car based on thier information provided in this dataset

## After cleaning the data I  applied pairplot to understand the relations between the features 


![pairplot.png](attachment:pairplot.png)

### observation from the pair plots
It is obvious that some features have a direct affect on the selling price of used car in auction
- (`sellingprice` & `year`)as the used car get older it selling price get less
- (`sellingprice` & `condition`) car with good condition get higher selling price
- (`sellingprice` & `odometer`) the more miles traveld by the car the less selling price it gets
- (`sellingprice` & `mmr`) there is astrong correlation between mmr(sugested selling price) and sellingprice and i think thiis indicates that mmr represents the real sellingprice
