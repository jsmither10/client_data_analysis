# Client Data Analysis

### Overview:

This analysis is a mock data analytics and enrichment project. A new company, BourbonBaked, ran a small beta launch of their new product offering and collected information from each beta participant. The company is interested in learning more about these beta users in order to create successful marketing campaigns for the future launches throughout the United States. This project explores the data enrichment and analysis of user data to determine those insights. 

This project utilizes a random generator API to gather fake client data. If you run this project locally your data will differ from that included in this project. Therefore, the analysis included in *data_vizualization* is only applicable to the current posted version of the *enriched_customer_file.csv*. If you run data_analysis.ipynb locally it will overwrite the *enriched_customer_file.csv* and the data you read in for *data_visualization* may not be accurate to the analysis provided. 

---

### Primary Files:

The entire project is in Python using Jupyter Notebooks. There are three primary files involved: 

1. **data_analysis**: This is the data gathering, cleaning, and enrichment process. The final file at the end of this exploration is exported to *enriched_customer_file.csv* This file can be reviewed as is, or follow the instructions below to generate your own custom data set utilizing the APIs. 
2. **data_vizualization**: This contains the charts exploring the final enriched data set. Please note: The final charts and graphs are based on the original working data set. Since the API generates new user information each time, the analysis included here only pertains to the original data set included in this repo and may not be relevant for a new subset of users generated from the API. 
3. **data_dictionary**: This is the dictionary for the final file that is the result of the data_analysis process. The raw file is *enriched_customer_file.csv* and this is the data dictionary to correspond to that file.

---

### Running the Program:

The following is a guide to running the project files locally:

1. Fork the repository [repo link](https://github.com/jsmither10/client_data_analysis.git)  
2. Clone the repository to your Github account
3. Access the repository from your command line or preferred CMD software
4. Install a virtual environment. The command in Gitbash is *python -m venv venv*
5. Activate the virtual environment. The command in Gitbash is *source venv/scripts/activate*
3. Install the *requirements.txt* file to install necessary packages by running *pip install requirements.txt* 

**Please note:** This requirements file was created on a Windows computer and uses Windows Python version pywin32==306. This project was done in a Windows environment and uses pathing that works in a Windows environment. In its current state, it can not be guarenteed to work in a Mac or Linux based system.

4. Create a new file, *creds.py*, and add it into the main project folder "Client_Data_Analysis"
5. This project utilizes the following two APIS
- [BMI API Calculator](https://rapidapi.com/malaaddincelik/api/fitness-calculator/) 
- [US State Info API](https://rapidapi.com/aptitudeapps/api/us-states) 
- You will need to create a free account on rapidapi.com in order to run this project. [Link to rapid API](https://rapidapi.com/auth/sign-up?referral=/aptitudeapps/api/us-states/pricing)
- Once you have created an account, click the API link above for US State Info and subscribe to the free tier by clicking on the "Pricing" link on the page. You can subscribe to the "Basic" plan for $0/month. Once for both to authenticate your API key. Your API key should be the same for both APIs. 
6. Copy your API key from the rapid API website
7. Open the creds.py file you created and add this block of code, adding in your API key into the placeholder space: 
```
api_key = "INSERT YOUR API KEY HERE"
```
8. You should now be able to run the entire notebook file *data_vizualization.ipynb* to generate your unique list of customers for the project 

---

### Sources:

Enrichment information came from the following sources:

- Census Bureau Regions: [www.census.gov](https://www2.census.gov/geo/pdfs/maps-data/maps/reference/us_regdiv.pdf)
- Per Capita Personal Income for 2022: [www.statsamerica.org](https://www.statsamerica.org/sip/rank_list.aspx?rank_label=pcpi1)
- Income Levels for the USA: [money.usnews.com](https://money.usnews.com/money/personal-finance/family-finance/articles/where-do-i-fall-in-the-american-economic-class-system)

API's Utilized:

- [Fitness Calculator API](https://rapidapi.com/malaaddincelik/api/fitness-calculator/)
- [US States API](https://rapidapi.com/aptitudeapps/api/us-states)


---

### Features:
1. Loading Data - Reading in a JSON file, Connecting to two APIs to create one data set
2. Cleaning Data - Merged data together from two different APIs
3. Visualize Data - Made 3 different visualizations on the data 
4. Best Practices - Included instructions on virtual environment setup, built a custom data dictionary 
5. Interpretation - Included a final anaylsis write up in *data_vizualization.ipynb*

