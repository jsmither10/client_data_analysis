# Client Data Analysis

#### Overview:

This analysis is a mock data analytics and enrichment project. A new company, BourbonBaked, ran a small beta launch of their new product offering and collected information from each beta participant. The company is interested in learning more about these beta users in order to create successful marketing campaigns for the future launches throughout the United States. This project explores the data enrichment and analysis of user data to determine those insights. 

---

#### Running the Program:

The entire project is in Python using Jupyter Notebooks. There are two primary files involved: 

1. **data_analysis**: This is the data gathering, cleaning, and enrichment process. The final file at the end of this exploration is exported to *enriched_customer_file.csv* This file can be reviewed as is, or follow the instructions below to generate your own custom data set utilizing the APIs. 
2. **data_vizualization**: This contains the charts exploring the final enriched data set. Please note: The final charts and graphs are based on the original working data set. Since the API generates new user information each time, the analysis included here only pertains to the original data set included in this repo and may not be relevant for a new subset of users generated from the API. 



The following is a guide to accessing the project files:
1. Fork the repository [repo link](https://github.com/jsmither10/client_data_analysis.git)  
2. Clone the repository from your Github account
3. Install the *requirements.txt* file to install necessary packages
4. Create a new file, *creds.py*, and add it to the project file
5. Click on [this link](https://rapidapi.com/malaaddincelik/api/fitness-calculator/) and [this link](https://rapidapi.com/aptitudeapps/api/us-states) and subscribe to the free tier for both to authenticate your API key. Your API key should be the same for both APIs. 
6. Copy your API key from the rapid API website
7. Open the creds.py file you created and add this block of code, adding in your API key into the placeholder space: 
```
api_key = "INSERT YOUR API KEY HERE"
```
8. You should now be able to run the entire notebook file to generate your unique list of customers for the project 

---

#### Sources:

Enrichment information came from the following sources:

- Census Bureau Regions: [www.census.gov](https://www2.census.gov/geo/pdfs/maps-data/maps/reference/us_regdiv.pdf)
- Per Capita Personal Income for 2022: [www.statsamerica.org](https://www.statsamerica.org/sip/rank_list.aspx?rank_label=pcpi1)
- Income Levels for the USA: [money.usnews.com](https://money.usnews.com/money/personal-finance/family-finance/articles/where-do-i-fall-in-the-american-economic-class-system)

API's Utilized:

- [Fitness Calculator API](https://rapidapi.com/malaaddincelik/api/fitness-calculator/)
- [US States API](https://rapidapi.com/aptitudeapps/api/us-states)


---

#### Features:


Create a new creds.py file locally to store the API key, where API KEY = 'INSERT KEY HERE'
https://rapidapi.com/malaaddincelik/api/fitness-calculator/

https://www2.census.gov/geo/pdfs/maps-data/maps/reference/us_regdiv.pdf


https://rapidapi.com/aptitudeapps/api/us-states

https://www.statsamerica.org/sip/rank_list.aspx?rank_label=pcpi1


