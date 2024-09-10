# HELP-International-Project
HELP International an NGO, is committed to fighting poverty and providing the people in developing countries with basic amenities and relief during the time of disasters and natural calamities.
 
Task:  Provide the NGO with a group of countries that are in critical conditions. Explore countries in different groups to prioritize when allocating resources.
Action: Used K-means clustering algorithm to determine the optimal number of clusters and categorize countries based on their foreign aid requirement using the development indicators provided.

**Data Distribution**

[visualization1.pdf](https://github.com/user-attachments/files/16949933/visualization1.pdf)


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

**Exploring Relationships across Variables**
[visualization2.pdf](https://github.com/user-attachments/files/16950046/visualization2.pdf)

**Variables with high positive correlation**
- Total fertility and Child Mortality: The higher the fertility rates, the higher the child mortality rate
  
-Imports and Exports: The higher the imports, the higher the exports. So 
countries that have high exports also import a lot.

-Income and exports: The higher the countries exports, the higher their income,
which is intuitive because the foreign exchange obtained from selling locally produced goods
increases the net income per person. 

- Gdp and Income: The higher the Gross domestic product of a coutry, the higher 
their income.

- Life expectancy and GDP: The higher the country's GDP, the higher their life expectancy.

**Variables with high negative correlation**
- Income and Child Mortality:The higher the country's net income per person, the lower its 
child mortality.
[visualization3.pdf](https://github.com/user-attachments/files/16950047/visualization3.pdf)


- Life expectancy and Total fertility: The higher the country's fertility rate, the lower
its life expectancy
[visualization4.pdf](https://github.com/user-attachments/files/16950048/visualization4.pdf)

Top Countries by Indicators 

[top_5_countries_exports.pdf](https://github.com/user-attachments/files/16950041/top_5_countries_exports.pdf)
[top_5_countries_gdpp.pdf](https://github.com/user-attachments/files/16950042/top_5_countries_gdpp.pdf)
[top_5_countries_health.pdf](https://github.com/user-attachments/files/16950043/top_5_countries_health.pdf)
[top_5_countries_life_expec.pdf](https://github.com/user-attachments/files/16950044/top_5_countries_life_expec.pdf)
[top_5_countries_total_fer.pdf](https://github.com/user-attachments/files/16950045/top_5_countries_total_fer.pdf)


**Clustering Process**

Optimal number of clusters

[visualization5.pdf](https://github.com/user-attachments/files/16950049/visualization5.pdf)

**Cluster Definition**
 Class 0 - requires urgent foreign aid
 Class 1 - No foreign aid 
 Class 2 - not a priority
 
[visualization6.pdf](https://github.com/user-attachments/files/16950050/visualization6.pdf)

Clustering Insights:
Most countries in Africa require foreign aid urgently. These countries are characterized 
by low levels of development which is evidenced by indicators such as  
- high child mortality rates
- ligh inflation rate
- high fertility rates
- low health expenditure
- high total fertility rate

Certain countries in the Middle East and Asia are in urgent need of foreign aid. In South America, only a handful of countries require immediate assistance. Meanwhile, countries in North America and Europe do not need foreign aid.

Comparing the median indicator values across clusters

[visualization9.pdf](https://github.com/user-attachments/files/16950053/visualization9.pdf)
[visualization8.pdf](https://github.com/user-attachments/files/16950054/visualization8.pdf)
