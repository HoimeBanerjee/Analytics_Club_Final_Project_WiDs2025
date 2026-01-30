# Analytics_Club_Final_Project_WiDs2025
This repository contains the codes for the analytics club project (Data driven carbon footprint analytics for chemical processes)-IIT Bombay WiDS 2025 for Week 3 and Week 4

**Week 3: Natural Language Processing using SpaCy library:**
 Sustainability reports taken from: Reliance → https://www.ril.com
 Pdfs work on: pdf_urls = [
    "https://rilstaticasset.akamaized.net/sites/default/files/2023-11/RILs-Sustainability-Report-2017-18.pdf",
    "https://rilstaticasset.akamaized.net/sites/default/files/2023-11/RIL-Sustainability-Report-2016-17.pdf"
    This project includes the ways to extract information from the online available sustainabilty reports by using concepts like tokenization and word frequency distribution.

Task 2: Generate:
word frequency distribution
bigram/trigram extraction
TF-IDF keywords


Task 3: Done using the : Dow → https://corporate.dow.com/en-us/science-and-sustainability
Extracting sustainability metrics, e.g.:
"Reduce CO₂ by 20% by 2030"
Used URL: url = "https://corporate.dow.com/en-us/purpose-in-action/climate-protection/decarbonization.html"
Extracted imformation from the images of the report.
#Sustainability keywords to match sentences used
keywords = [
  "reduce", "reduction", "cut", "decrease", "lower",
    "emission", "emissions", "carbon", "co2", "ghg",
    "energy", "water", "climate", "decarbon", "net zero"
]


Task 4: Compare these to actual process data trends:
Is emission declining? Does process efficiency match sustainability claims?
First fetched imformation from all the available images in the report
Used the Image 8 to fetch the data and compare the trends
URL generated:Processing Image 8: https://corporate.dow.com/en-us/purpose-in-action/climate-protection/decarbonization/_jcr_content/root/container/columnband_v2/image.coreimg.jpeg/1768943133591/path-to-zero-graphic.jpeg

After fetching the data, normalised the baseline to 2020 and performed trend analysis.
Result: → Process emissions are declining.
→ Process efficiency lags behind Dow sustainability claim

Week 4: Final Project:
Dataset used:https://github.com/openclimatedata/edgar-co2-emissions

Task 1: Predict future emissions or emission intensity from historical operational dataset A
•	Clean dataset and engineer features.
•	Split data (train/test or time-based split).
•	Train at least two ML models:
a)	Linear Regression / Ridge
b)	Random Forest or XGBoost

•	Evaluate models:
a) RMSE
b) MAE
c) R²

•	Extract feature importance:
a)	Random Forest importance or
b)	SHAP values


Output
•	Table of model metrics
•	Plot: Actual vs Predicted Emissions
•	Feature importance plot

## Task 2 and 3 already done as Week 3 assignment (Company selected:  Reliance → https://www.ril.com and  Dow → https://corporate.dow.com/en-us/science-and-sustainability both
Task 2: Automatically extract emission-related commitments from any sustainability report
a)	Extract text from PDF using pdfplumber or PyMuPDF.
b)	Clean text (lowercase, remove stopwords, punctuation).
c)	Identify emission-related sentences using:
•	Keyword rules (CO₂, emission, net-zero, Scope 1/2/3)
•	TF-IDF scoring
d)	Extract commitment statements


Task 3: Check whether ML-predicted emission trends support or contradict stated goals.
a)	From ML predictions: Estimate emission trend slope (% change per year)
b)	From NLP: Extract stated reduction target (% by year)
c)	Compare: 
•	Predicted reduction vs stated reduction
•	Identify alignment gap
## Result: After fetching the data, normalised the baseline to 2020 and performed trend analysis.
Result: → Process emissions are declining.
→ Process efficiency lags behind Dow sustainability claim



    
 

