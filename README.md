# HELP-International-Project
HELP International an NGO, is committed to fighting poverty and providing the people in developing countries with basic amenities and relief during the time of disasters and natural calamities.
 
Task:  Provide the NGO with a group of countries that are in critical conditions. Explore countries in different groups to prioritize when allocating resources.
Action: Used K-means clustering algorithm to determine the optimal number of clusters and categorize countries based on their foreign aid requirement using the development indicators provided.

****Data Distribution****

![visualization1_page-0001](https://github.com/user-attachments/assets/664d9b89-6125-42b8-9791-cd54db5b925e)


**Child Mortality**: The dataset shows that many countries have child mortality rates below 50. However, there 
are a few outliers with rates of 100 and above, leading to a right-skewed distribution.

**Exports:** Most countries have export values below 100, but a small number of countries have exports exceeding 
1000, which also results in a right-skewed distribution.

**Health Expenditure**: Health expenditure for the majority of countries ranges between 2% and 12%. Only a few 
countries exceed 14%, creating a right-skewed distribution.

**Imports**: Most countries have import rates below 75%, but some outliers show rates exceeding 100%, indicating 
high import levels.

**Income**: The net income per person for most countries is below 4000. There are a few outliers with income levels 
above 6000, resulting in a right-skewed distribution.

**Inflation**: Most countries have inflation rates between 0% and 20%, with a few outliers exhibiting rates over 20%.

**Life Expectancy**: In contrast to other indicators, life expectancy has a left-skewed distribution. Most countries 
have life expectancy rates between 60 and 80 years, with only a few countries having rates below 50 years.

**Total Fertility**: Over half of the countries have fertility rates below 4%. There are also some outliers with 
rates reaching up to 7%.

**GDP**: GDP per capita for most countries is below 2000, but there are outliers with values as high as 100,000, 
resulting in a right-skewed distribution.

****Exploring Relationships across Variables****
![visualization2_page-0001](https://github.com/user-attachments/assets/e986d494-9faa-4236-a7f6-3fcdad062ea8)

**Variables with high positive correlation**
- Total fertility and Child Mortality: The higher the fertility rates, the higher the child mortality rate
  
-Imports and Exports: The higher the imports, the higher the exports. So countries that have high exports also import a lot.

-Income and exports: The higher the countries exports, the higher their income,
which is intuitive because the foreign exchange obtained from selling locally produced goods
increases the net income per person. 

- Gdp and Income: The higher the Gross domestic product of a coutry, the higher 
their income.

- Life expectancy and GDP: The higher the country's GDP, the higher their life expectancy.

**Variables with high negative correlation**
- Income and Child Mortality:The higher the country's net income per person, the lower its 
child mortality.
![visualization3_page-0001](https://github.com/user-attachments/assets/68723464-3e9a-4293-aafe-f4059c0da53f)


- Life expectancy and Total fertility: The higher the country's fertility rate, the lower
its life expectancy
![visualization4_page-0001](https://github.com/user-attachments/assets/e676555d-45d9-4b35-8c80-307a411bb5f9)

**Top Countries by Indicators **

![top_5_countries_exports_page-0001](https://github.com/user-attachments/assets/928e3d4a-75b2-4854-9d31-d1909a749a5f)
![top_5_countries_gdpp_page-0001](https://github.com/user-attachments/assets/56bdff42-9317-41ce-9f58-55f2245f7424)
![top_5_countries_health_page-0001](https://github.com/user-attachments/assets/409727ec-2937-4d40-92a8-0a34f3fb58be)
![top_5_countries_life_expec_page-0001](https://github.com/user-attachments/assets/53b7c94a-45bc-4346-bd92-13fbf3395bde)
![top_5_countries_total_fer_page-0001](https://github.com/user-attachments/assets/e72ed5a2-7933-4246-b55f-3c338443d0fc)


****Clustering Process****

Optimal number of clusters

![visualization5_page-0001](https://github.com/user-attachments/assets/fa93dd87-0d9d-414c-8cab-13981658e2b8)

**Cluster Definition**
 Class 0 - requires urgent foreign aid
 Class 1 - No foreign aid 
 Class 2 - not a priority
![visualization6_page-0001](https://github.com/user-attachments/assets/e1f459b0-df64-475f-9413-ae41090b2dc5)


****Clustering Insights:****
Most countries in Africa require foreign aid urgently. These countries are characterized 
by low levels of development which is evidenced by indicators such as  
- high child mortality rates
- ligh inflation rate
- high fertility rates
- low health expenditure
- high total fertility rate

Certain countries in the Middle East and Asia are in urgent need of foreign aid. In South America, only a handful of countries require immediate assistance. Meanwhile, countries in North America and Europe do not need foreign aid.

****Comparing the median indicator values across clusters****
![visualization8_page-0001](https://github.com/user-attachments/assets/e87bb31b-6a0f-4466-98e3-01dd55c34a53)
![visualization9_page-0001](https://github.com/user-attachments/assets/d74b49f0-8e2e-438e-afa8-10c67edd069a)
