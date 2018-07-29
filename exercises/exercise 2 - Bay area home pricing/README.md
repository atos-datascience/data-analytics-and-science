# The problem
We want to predict the home pricing based on records of recently sold homes in the Bay area.

# Data
The training set can be found [here](./data/train.csv)

| Variable | Description|
|----------|------------|
| id  | Unique ID |
| address   | Address of the house |
| info  | City and sales price info |
| z_address | Abbreviated address |
| bathrooms | The number of bathrooms present when the house was last sold |
| bedrooms | The number of bedrooms present when the house was last sold |
| finishedsqft | The number of square feet the house consisted of when it was last sold |
| lastsolddate | The date of the last house sale |
| lastsoldprice | The price of the house when it was last sold |
| latitude | Latitude of the house |
| longitude | Longitude of the house |
| neighberhood | Location of the house e.g. South of the market |
| totalrooms | Total number of rooms present when the house was last sold |
| usecode | The type of the house e.g. Condominium or a Single family house |
| yearbuilt | The year the house was built | 
| zestimate | The price estimate provided by Zillow, a house price estimate website |
| zindexvalue | Market value |
| zipcode | Zipcode of the house |
| zpid | Unique ID in Zillow database |

# Possible Solution direction and pointers
- Clean up the data
	- A lot of columns contain redundant information, doesn't seem very useful..
	- We want to estimate prices, but somebody already did. Damn Zillow!
	- zindexvalue does not show up when using dataframe.describe()... What is up with that?

- Find a good correlation
	- The last sold price feature is nice. Are there any features that correlate?


# How to submit
Create a folder with your name e.g. john-doe inside the solutions folder and put your notebooks inside.
Commit this to your own fork of the data-analytics-and-science repository and create a pull request to the main repository.