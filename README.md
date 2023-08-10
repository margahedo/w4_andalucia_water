# w4_andalucia_water

![portada](https://cdn1.img.sputniknews.lat/img/07e7/01/12/1134795230_0:789:2048:1941_1920x0_80_0_0_e13b49c54b945c2aa32eb15351c76368.jpg)


## Introduction
With water reserves at a minimum, six continuous years of scarce rainfall, high temperatures and no precipitation on the horizon, Andalusia is facing a situation of drought that has important repercussions for the economy, biodiversity and everyone's life. of the living things that inhabit it.

The reserve of water for human consumption is the lowest in the last 12 years, the reservoirs before the summer are at 51.2% of their capacity and the rain forecast is disastrous. 60% of the country's crops are damaged.

The situation is due to the fact that it does not rain in Spain. The winter has turned out to be very mild, March was abnormally hot and April, still inconclusive, is on the way to being so. The lack of rainfall has been the general trend that has accompanied this deceptive weather bonanza and the results are already being felt in the form of serious damage to crops.
According to data from the Coordinator of Organizations of Farmers and Ranchers (COAG), the main agricultural organization in the country, the drought is already suffocating 60% of the Spanish countryside and is causing irreversible losses in more than 3.5 million hectares of dryland cereals.

The wheat and barley crops in Andalusia, Extremadura, Castilla-La Mancha, Murcia and the most arid areas of Aragon, Catalonia, Castilla y León, are considered lost. The scarcity of rain also threatens honey production. The lack of vegetation and flowering in the mountains prevents bees from being able to feed and produce it. "It would be the third campaign without a harvest for beekeepers," COAG warned in an official statement.

The objective of this project is to analyze data on drought in an Andalucian area. 

For this project, we wll start with a dataset and we will import it, using our skills cleaning and processing the data. We will demonstrate our proficiency with the tools we cover (functions, classes, list comprehension, string operations, pandas and error handling, etc.) in our functions.

---

## Technical Requirements

The technical requirements for this project are as follows:

* We must put our code wrapped in functions.
* The following data pipeline stages should be covered: acquisition, wrangling, analysis, and reporting.
* We must extract data from **3 different sources using 2 different tools**(Downloading a `.csv`,API, web scrapping...)
* We must demonstrate all the topics we covered in the chapter (functions, list comprehensions, string operations, etc) in your processing of the data.
* We code should be saved in a Python executable file (.py), your our should be saved in a folder named data or src.
* We should also include a README.md file that describes the steps we took and your thought process as you built your data pipeline.


## TO DO's

- A) Find a dataset to start you work! The first place where we found our data was:
https://monitordesequia.csic.es/monitor/?lang=es#index=spei#months=0#week=4#month=0#year=2023
A drought monitor that shows the levels of drought in specific parts of the world and returns the indices that you ask for.

We ask for the drought data by the SPEI index from 1961 to today in .csv format.
The data we obtained has been taken once a week, so we have a very wide range of data to compare

  
- B) Clean and wrangle your dataset, prepare the data for your needs and intentions.
      1. IMPORT LIBRARIES:
      2. IMPORT CSV: One for each province
      3. CLEAN CSV: For this step, you have to eliminate all the columns that are not interesting for the study. In this case, they are the columns that                     give us other types of indexes. We also create a column that groups the data as an average, and leaves only two decimal places                            (important to pass it to MySQL later). This step must be done with each of the columns.
      4. Pass it to MySQL to have the database saved and clean
      5. Make a single table to have all the information on the drought by province. Also change the column names for better understanding.
      6. With Beautiful.Soup we extract the population data of each of the provinces.