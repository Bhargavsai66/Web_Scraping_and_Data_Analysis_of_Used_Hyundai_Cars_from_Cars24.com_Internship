# Web_Scraping_and_Data_Analysis_of_Used_Hyundai_Cars_from_Cars24.com_Internship

### 📝 Project Title

🚗Web Scraping and Data Analysis of Used Hyundai Cars from Cars24.com

### 🎯 Objective

In this project, I developed a complete data pipeline to automatically extract, clean, and analyze data of used Hyundai cars listed on **Cars24.com**.
My goal was to collect details like model name, year, kilometers driven, fuel type, transmission, price, and location — and use them for market analysis.

### 🔹 Tools & Technologies

I used Python along with the following libraries and tools:

* Selenium WebDriver – to handle dynamic web pages and load all listings.
* BeautifulSoup– to parse the HTML content and extract car details.
* Pandas – for data cleaning, structuring, and exporting to CSV.
* Regular Expressions (re)– to clean inconsistent formats like “₹6.5 Lakh” or “82,657 km”.

### 📝 Step-by-Step Work Done

### Step 1 – Planning & Setup
I started by selecting Cars24.com as my data source and focused on **Hyundai cars**.
I set up my Python environment, installed Selenium, BeautifulSoup, and Pandas, and connected ChromeDriver for browser automation.

### Step 2 –🌐 Web Scraping Using Selenium
I automated the Chrome browser using Selenium.
The script scrolled through the webpage, loaded all listings, and navigated through multiple pages to ensure that all data was captured.
Once the page was fully loaded, I extracted the complete HTML content.

### Step 3 –🔍 Data Extraction with BeautifulSoup
I parsed the collected HTML using BeautifulSoup and extracted key attributes for each car:

* Model name
* Year of manufacture
* Kilometers driven
* Fuel type
* Transmission
* Price
* Location

### Step 4 –🧹 Data Cleaning & Processing
The extracted data had inconsistent formats, so I cleaned and standardized it using Python string operations and regex.
For example:

* `"82,657 km"` → `82657`
* `"₹ 6.5 Lakh"` → `650000`

After cleaning, I structured the data into a Pandas DataFrame and exported it to a CSV file.

### Step 5 – 📊Data Visualization & Analysis
Once the dataset was ready, I analyzed it using different plots and charts:

* Manual vs Automatic Transmission Count – showed that manual cars are more common.
* Fuel Type Distribution – revealed that petrol cars dominate the market.
* Kilometers Driven Distribution – compared mileage patterns for manual vs automatic.
* Average Kilometers by Location – identified areas with higher usage.
* Scatter Plot (KMs vs Transmission) – showed that high-mileage cars are mostly manual.
* Heatmap (Transmission vs Fuel Type) – confirmed that petrol-manual cars are the most common combination.
* Cars by Year of Manufacture – indicated peaks between 2017 and 2019.

### Step 6 – 🧠Challenges Faced & Solutions

* Dynamic content: Cars24 loads listings dynamically, so I used Selenium instead of static HTML parsing.
* Inconsistent formats: Handled various numeric and unit formats using regex.
* Data duplication: Removed duplicates before final export.

### Step 7 –📈 Results & Insights

* Manual transmission cars dominate the used Hyundai car market.
* Petrol is the most common fuel type.
* Cars from 2017–2019 are most frequently available for resale.
* Some regions have higher average kilometers, showing more long-distance usage.

### Step 8 –🧩 Outcome & Learning

This project gave me strong hands-on experience in:
🔧 Web Scraping of dynamic websites
🧼 Data Cleaning & Preprocessing
📉 Data Visualization & Insight Extraction

