# Model-to-predict-Energy-consumption-City-of-Seattle
Use Seattle's public energy data and build a model predicting energy consumption

![](asset/map.jpg)

The objective of this project is to build a supervised predictive model using energy consumption reports from buildings of the city of Seattle.
The data are available at Kaggle [here](https://www.kaggle.com/city-of-seattle/sea-building-energy-benchmarking?select=socrata_metadata_2016-building-energy-benchmarking.json). The data and additional information can also be found on the [official public website of Seattle's administration](http://www.seattle.gov/environment/climate-change/buildings-and-energy/energy-benchmarking).

# Context
Buildings account for 33% of Seattle's core emissions. The benchmarking policy supports Seattle's goals to reduce energy use and greenhouse gas emissions from existing buildings. In 2013, the City of Seattle adopted a Climate Action Plan to achieve zero net greenhouse gas (GHG) emissions by 2050. Annual benchmarking, reporting and disclosing of building performance are foundational elements of creating more market value for energy efficiency. 

Seattle's Energy Benchmarking Program requires owners of non-residential and multifamily buildings (20,000 sf or larger) to track energy performance and annually report  to the City of Seattle.

# Project structure

A significant part of the project is dedicated to prepare and clean the raw data for the machine learning algorithms.
Two years of data (2015 & 2016) are used.
The project steps include:
- Loading and Exploring the datasets
- Harmonize the datasets so that they can be combined
- Develop strategy for missing values
- Decide on the features to keep and those to discard
- Prepare the cleaned dataset for training and testing
- Train model and test accuracy
- Observe the most important features

RandomForest and XGBoost are used and achieve over 97% accuracy.
More important features are building floor area, building year and the number of floors. Building surface is obvious a key driver for energy consumption.
