# Project 1 : Proposal Outline
---
### Group 2 Members
* Omar Bernal
* Emily Hurst
* Hamilton Cha
* Keith Moravec
* Victoria Barbosa
---    
### Topic: Is Climate Change Real and is it correlated with atmospheric C02 concentration?
---
### Data Sources

> APIs:  
* https://temperature.global/
* https://datahelpdesk.worldbank.org/knowledgebase/articles/902061-climate-data-api
* https://www.programmableweb.com/api/global-warming-carbon-dioxide-co2-atmosphere-concentration-rest-api-v10
 - since 2010 UN Data for CO2 emmissions (file sent from Emily)
---

* Omar (C) = Historic weather change data
* Hamilton = C02 levels in major cities (urban and rural) across date range
* Keith = find beta model for CO2 and temperature and project CO2 against time (using standard regression per year plug
* Victoria = Rate of extreme weather resulting from climate change
* Emily = Temperature/Ocean levels in major cities (urban and rural) across date range

---
### FORMATTING / PRESENTATION
1. try using plot USING Seaborn
    import seaborn as sns
    sns.scatterplot(x="Year",y="Temp",hue="CO2(ppm)",data=temp_co2)
2. PNG file for each graph
3. Answer each question using markdown and inserting PNG files


### Questions
NEED TO DO
1. explain how we pulled, cleaned, merged data

1. Is pollution (CO2) related with climate change (avg globale temparture)
    CO2 and Temperature are correlated (graph, data, r-squared correlation confirmed)
2. How does CO2 directly impact temperature. 
    1. Do we see change in temp vs time (done!)
        1. t-test on the slope from 1900 - 1950 vs 1950 - present (dates TBC)
        2. is the rate of temperature vs time changing
    2. Do we see change in CO2 vs time (done)
        1. t-test on the slope from 1900 - 1950 vs 1950 - present (dates TBC)
        2. is the rate of CO2 vs time changing
    3. Are they correlated? (done)
        linear regression with r-squared values (done)
4. Temperature rise we are seeing in regions accross the globe
    1. Are there correlation to nataral disasters related to temp or CO2?  with linear regression with r-squared values
        1. Wildfire vs Year (HYC)
        2. Drought vs Year (HYC)
        3. Flood vs Year (HYC)
        4. Extreme temperature vs Year (HYC)
        5. Extreme weather vs Year (HYC)
        6. Temp vs CO2 (HYC)
        7. Temp vs All Natural Disaster combined(HYC)
        8. CO2 vs All Natural Disaster combined (HYC)
    2. 12042021 HYC NOTE
        3. in the 'hamilton' branch i worked on the temp v co2 v disaster graphs and basic stats
        4. python filename: Temp_CO2_Disaster_v0-hyc12042021.ipynb
        5. png line charts uploaded in "Project/png_data"
         6. 8 charts
        7. basic 'stats_summary" for the above charts in "Project-1/Drafts/output_data"
         8. **TEAM QUESTION**: PLEASE REVIEW STATS SUMMARY.  What do you guys think it says?  Is there anything that looks strange?
         9. I think the non-year related data is very interesting and inline with what we have been saying.
         10. Is there anything to be concerned about with p-values for all analysis being ZERO???
          11. What would the temperature be without human activity?
          12. (OUT OF SCOPE ??) Map out temperature with no increase in CO2.


### OUT OF SCOPE QUESTIONS  - We are focused on global data and are pulling out country questions
5. What countries are polluting/fires/drought the most and does this correlate with weather CO2 in region and was there a correlation (we are focused globally)
7. Does local C02 emissions influence local temperature rise?
8. Do not include Hurricane because it is a different data set.

### REMOVED
3. Historical global model
