# Data portfolio : Excel to Power BI



# Table of Contents
## - Introduction
## - Project overview
## - Analysis tools
## - Data acquisition
## - Data cleaning and validation
## - Data analysis
## -  Key findings
## - Recommendations
## - Conclusions

# Introduction
This report analyses a financial consumer complaints dataset to uncover insights into the types of complaints received, the timeliness of company responses, and patterns in consumer dispute resolutions.
# Project Overview
This report provides insights into complaint trends, company performance, and areas for improvement. The dataset consists of the following columns;
#### Response Days: Time taken by the company to respond to a complaint.
#### Products: Financial products involved in the complaints.
#### Issues: Types of issues raised by consumers.
#### Countries: Geographic locations where complaints originated.
#### Consumer Dispute: Indicator of whether the consumer disputed the resolution.
#### Consumer Consent: Whether the consumer consented to share complaint data publicly.
#### Medium via Issues Were Submitted: Channels through which complaints were submitted (e.g., email, phone, web).
#### Company Response: Descriptions of how companies responded to complaints.
#### Timely Response: Indicator of whether the company responded within a specified time frame.

# Analysis Tools
#### •	Google Sheets: Used for initial data extraction online

#### •	Microsoft Excel: Employed for advanced data cleaning and transformation

#### •	Power BI: DAX was utilized for creating custom calculations and metrics to derive deeper insights, bi was used for reporting and dashboard creation to visualize trends and performance metrics.
# Data Acquisition: data was extracted on kaggle.
![Image](https://github.com/user-attachments/assets/a64a73ef-5f68-46bc-a085-8ffa96959bed)
# Data Cleaning and Validation
To ensure accuracy and reliability of the dataset, missing values were checked. 3% of the dataset were missing, the missing values in the country column were replaced with others, empty entries in columns were replaced with N/A. Also, columns that were unnecessary for the analysis were removed, duplicate entries were removed and the date column was also checked to ensure the issues were recorded between 2011- 2020.
![Image](https://github.com/user-attachments/assets/ac9bc0db-b95d-44b5-a176-6421ae69c2a6)


# Data Analysis

## Descriptive Analysis

•	Issues: The dataset’s "Issues" column highlights recurring problems reported by customers. By Summarizing the number of complaints for each product category, grouping and analysing these issues, we can identify the most frequently reported problems. The company received a total of 75,513 complaints between the year 2011-2020.

•	Product: The products purchased from the company shows more insights into issue reported, there are 8 products the company offers its customers. Identifying which products generate the most complaints can help prioritize areas for process improvements.

•	Regional Trends: Analysis of the "countries" column provides insights into geographical patterns. Specific regions or countries may have higher complaint volumes, possibly reflecting market size or unique financial challenges in those areas. There are 62 countries in total in this dataset.

•	Timely Response: Using the "Timely Response" column, I evaluated how often companies meet deadlines for responding to complaints. High levels of timely responses indicate strong operational efficiency, whereas delays may point to congestion in complaint handling processes.

•	Response Days: Using the date complaint was submitted and received a new column Response Days" was created. It provides a quantitative measure of the average response time. Trends can reveal if certain issues or products take longer to address, allowing companies to refine complaint management processes.

•	Dispute Resolution: The "Consumer Dispute" column tracks whether consumers dispute the company’s resolution. High dispute rates may signal dissatisfaction with company practices or inadequate resolution methods. These trends are critical for improving customer satisfaction.

•	Consent to Share: Examining the "Consumer Consent" column reveals how many consumers agreed to share their complaints publicly, understanding this trend helps determine the level of consumer trust and transparency.

•	Submission Medium: The "Medium via Issues Were Submitted" column provides valuable insights into consumer behaviour. Popular submission methods, such as web portals or phone calls, can inform companies on optimizing communication channels.

# Comparative Analysis

•	Issue by Product: Analysing which products (e.g., credit cards, student loans) generate the most complaints and identifying differences in complaint frequency or types of issues across products.
The chart shows credit card was the product associated with high volume of complaints while vehicle loan or lease had least complaints recorded


![Image](https://github.com/user-attachments/assets/59fd844c-452f-4991-9e7b-9f038e48b3d1)

•	Geographical Trends: Examining complaint patterns across different countries or regions to determine which areas have higher or lower complaint volumes and understanding the reasons behind them.

![Image](https://github.com/user-attachments/assets/7b2cf349-dece-472f-ac66-034e4aa6c87c)
![Image](https://github.com/user-attachments/assets/30362cdc-5c64-41ef-9f29-70b45354a3f7)

The chart above shows the top countries complaints were received and countries with least complaints. California had the highest while Palau had the least received complaints.
Furthermore, it was necessary to examine the dominant issues in the 62 geographical locations customers reside. To achieve this, new measures dominant issues and their respective counts were created using DAX. Dominant issues, their counts and percentage in each country are showed in the table below.

![Image](https://github.com/user-attachments/assets/6cae22d1-6852-409a-b755-24b992940b45)

•	Company Responses: Comparing the timeliness and effectiveness of responses across different companies or types of complaints.
Majority of complaints (98%) received were timely responded to. Furthermore, 55k issues were closed and explanation were given to customers. This resulted in 41.32% of complaints not disputed by customers.

![Image](https://github.com/user-attachments/assets/268455d9-242d-4a25-a14d-e5a286b42073)
![Image](https://github.com/user-attachments/assets/ec8fd78e-d70c-4ab9-8563-9d4bf0d5a904)
![Image](https://github.com/user-attachments/assets/9a816547-5c27-4360-a68f-e76f9e06e169)

•	Submission Mediums: Analysing which communication channels are most effective for resolving complaints quickly or which channels consumers prefer to use. High number of customers prefer to submit issues via web, fewer customers complained via email.

![Image](https://github.com/user-attachments/assets/89e92496-4999-4641-b161-062a36e33fc9)

Further analysis into the average number of days issues were received showed issues received via email takes longer time compared to via web.

![Image](https://github.com/user-attachments/assets/734fd1d1-43b6-46fe-832d-f84c853be713)

•	Complaints over the time: Analysis revealed more complaints were received during the year 2018 with April been the peak month.
Overall, August was the month highest complaints were received.

![Image](https://github.com/user-attachments/assets/d2cfb7dc-9e55-46e8-95ae-56f197aa5401)
![Image](https://github.com/user-attachments/assets/ef493dcf-8f25-4918-9943-3ec88ccc0cd9)

# Key Findings

![Image](https://github.com/user-attachments/assets/767e3df5-8a97-411a-8ba1-a0290c02508a)
![Image](https://github.com/user-attachments/assets/4e67432a-769f-48d3-b0d0-40d874194b4c)

•	Product Trends: Credit cards have the highest number of complaints, while vehicle loans have the lowest.

•	Geographical Insights: California reports the highest number of complaints.

•	Timeliness: The overall timely response rate is 98%.

•	Channel Preference: Web is the fastest medium for issue resolution, while email is the slowest.

•	Consumer Disputes: The dispute rate is 9.75%, suggesting room for improvement in resolution quality.

•	Recurring Issues: The dominant issue reported is "managing an account."

•	Seasonal Patterns: August has the highest complaint volume, followed by July.

# Recommendations

Address High Complaint Products

Focus on resolving recurring issues with credit cards, as they generate the most complaints.

Provide proactive account management solutions and educational resources for consumers.

Improve Complaint Resolution Quality

Analyse the root causes of disputes and implement solutions to address consumer dissatisfaction.







