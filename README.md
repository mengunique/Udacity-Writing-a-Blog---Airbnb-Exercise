
### Airbnb in Seattle, Boston and Beijing

#### Analysis of Seasonal Trend, Availability and Pricing


### Motivation and synopsis
This project is part of the requirement for Data Scientist Nanodegree on Udacity to follow the CRISP-DM (Cross-industry standard process for data mining). The project aims to analyze some aspects of the Airbnb renting scene in the chosen cities. 
Key questions to answers as follows:

[Data exploratory Questions]
1.	How does the average availability of Airbnb homes vary over time in each city? Is there a clear seasonal pattern for the average nightly rate on Airbnb in the chosen city? Is there a clear weekly pattern?
2.	Which neighborhood is the most expensive? Which property type is most common? 
3.	How does the trends compare between cities? Seattle, Boston and Beijing?

[Model prediction] 
4.	Can we predict the listing price? We know that price quite depends on the location, but many other factors may help predict the listing price such as room type, property type, size, #beds, any correlation between # of comments and price? E.g. Multiple regression analysis can be done in Python to put these variables together to predict the listing price of a property？

### File Descriptions
Thanks to Airbnb Open data source: http://insideairbnb.com/get-the-data.html

There are 3 different folders with 3 files each (data updated as of 2019-07)
- listing.csv.gz: provide individual listing and its attributes: host information, listing information, pricing, review etc
- calendar.csv.gz: occupancy and availability of listings in 365-day period
- reviews.csv.gz: for all historical listings 

### Analysis Results in Brief
Q1. I tried to compare Seattle, Boston and Beijing Airbnb Renting scene. There is a clear seasonal pattern for Boston and Seattle, according to the best time to visit for these cities. 
Strangely, Beijing City only has a slight price difference for August, but there is no clear changes in the price. Possible reason is that the price is generally cheaper as compared to the States, and Airbnb is not that popular in China, so the occupancy rate is not as high to generate a higher seasonal price point.  

Q2. Now we understand more of different cities geographical distribution, and most expensive neighbourhood and most common property type. Useful tips for travel to these cities. :)

Q3. Boston has a higher price point as compared to Seattle, and has the most apartment %. Good season to visit will be April - June. 

Q4. I used "Random Forest" to predict for price with chosen factors including neighbourhood, size, #beds, #of comments etc. For the test set, the model runs very well with R2 being 0.7 and above; for the training set, the model is not yet so good. 
Possible next step if there is more time will be to explore other models, or try to use unsurpervised learning like PCA to tighten the constraints. 

### Acknowledgements
A special thanks to a few super blogs on github and medium to help me with the data exploratory and modelling:
    https://medium.com/@anhchu1291/seattle-airbnb-renting-scene-a-closer-look-powered-by-data-f7498ae57262
    https://towardsdatascience.com/exploring-machine-learning-for-airbnb-listings-in-toronto-efdbdeba2644
    https://github.com/jclh/airbnb-boston-seattle
        
### Author
April Li
- https://github.com/mengunique
- medium blog: https://medium.com/@limengapril/data-science-to-help-you-find-the-best-time-to-travel-da6403d41f90


### Installation Remakr 
The Jupyter Project highly recommends users to install [Anaconda](https://www.anaconda.com/distribution/)
since it conveniently installs Python, the Jupyter Notebook, and other commonly used packages for scientific computing and data science.

Use the following installation steps:
1. Download Anaconda.
2. Install the version of Anaconda which you downloaded, following the instructions on the download page.
3. To run the notebook:
jupyter notebook:
    Airbnb homework_Seattle.ipynb
    Airbnb homework_Boston.ipynb
    Airbnb homework_Beijing.ipynb
    
### Python libraries

The Jupyter Notebook files requires the following Python libraries:
- numpy
- pandas
- matplotlib
- seaborn
- sklearn.model_selection
- sklearn.ensemble




```python

```
