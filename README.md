# Food Waste & Nutrition Indicators (FAOSTAT Data)

Case work from https://github.com/Marchev-Science/case-fao-nutrition-food-waste?tab=readme-ov-file

" Food loss and waste is a critical global issue with multifaceted impacts. Roughly 30% of food produced for human consumption is lost or wasted each year, amounting to about 1.3 billion tonnes of food. This squandered food has enormous implications: FAO estimates that the food we lose and waste annually could feed 1.26 billion hungry people. Reducing food wastage is thus not only a matter of resource efficiency but also of improving food security and nutrition. In fact, cutting food loss and waste is enshrined in Sustainable Development Goal (SDG) 12.3, which calls for halving per-capita global food waste and reducing losses by 2030.

Paradoxically, the world today faces a “double burden” of malnutrition – persistent undernourishment in many countries alongside rising obesity in others. Over 828 million people were undernourished in 2021, even as obesity rates have climbed worldwide. Understanding how food waste relates to nutrition outcomes is therefore a pressing analytical challenge. For example, excess food availability might contribute to both higher obesity and more waste, while inadequate distribution and access lead to undernutrition even amid plenty. Recent research has hypothesized that greater food losses lead to lower per-capita food supply, thereby reducing a population’s dietary intake. Empirical findings support some of these links – for instance, studies show that increases in per-capita food supply are associated with lower prevalence of undernourishment. This complex relationship may involve intermediate factors (e.g., overall food availability) mediating the impact of waste on nutritional status.

Against this backdrop, this week-long challenge asks participants to explore and model the relationships between food waste and nutrition indicators using data from FAO’s FAOSTAT database. Participants will investigate how variations in food waste/losses correlate with three key nutrition outcomes – dietary energy adequacy, undernourishment, and obesity – and assess whether an abundance of food supply (per capita) mediates these relationships. The goal is to derive insights that could inform policies for reducing waste while improving nutrition. This project is geared toward postgraduate students (Masters/PhD level) with mixed levels of experience in statistics, data science, and domain knowledge. Over the course of one intensive week, teams will formulate a research question, assemble and analyze a country-level panel dataset from FAOSTAT, apply suitable statistical or machine-learning models, and present their findings in a reproducible Jupyter Notebook. "

# Challenge Objectives and Core Task
## Objective
Determine how food waste is related to national-level nutrition and food-security indicators, and whether food supply per capita mediates these relationships. Participants should use only FAOSTAT data for a panel of countries over time to ensure consistency and comparability.

## Core Modeling Task
Analyze how food waste relates to each of the following three target nutrition indicators (with potential mediation by per-capita food supply):

- Dietary Energy Adequacy – The average dietary energy supply as a percentage of the population’s required energy needs.
- Prevalence of Undernourishment – The share of the population that is chronically undernourished (consuming less than the minimum dietary energy requirement).
- Prevalence of Obesity – The share of the adult population that is obese (BMI ≥ 30).

Mediating Factor: Food Supply per Capita – The average food availability per person, measured in kilocalories per person per day.

# Introduction

Food supply remains unevenly distributed across the globe. As of 2022, an estimated 9.1% of the world’s population is undernourished, while 16.02% is classified as obese. These figures underscore a global paradox of coexisting food insecurity and overnutrition. Moreover, the average dietary energy supply, expressed as a percentage of the population’s required energy needs, varies significantly across regions, countries, and even within national borders. 

Projections that the global population will reach 9.7 billion by 2050 raise pressing questions about how to ensure adequate food supply for all. In the context of limited natural resources, ongoing socio-economic development, and changing dietary preferences, particularly in developing countries, scientists and policymakers are increasingly examining strategies to meet future nutritional needs. One promising approach is to reduce food loss and waste, which currently account for approximately one-quarter of all calories produced worldwide.  Recovering these lost calories could potentially increase global food availability without the need for additional natural resources.

However, food systems are highly complex, and such outcomes cannot be assumed. Any prediction about the effects of reducing food loss must be grounded in rigorous analysis that considers the interplay of multiple factors shaping food production, distribution, and consumption across different contexts.

This study therefore aims to examine the relationship between food losses and three key nutrition indicators, with a focus on the potential mediating role of per capita food supply:
- Dietary Energy Adequacy – the average dietary energy supply as a percentage of the population’s required energy intake.
- Prevalence of Undernourishment – the proportion of the population consuming less than the minimum dietary energy requirement.
-  Prevalence of Obesity – the share of the adult population classified as obese (BMI ≥ 30).
 
The analysis draws on FAO data from a 20-year period for a sample of three countries, each representing a different global region and income level: one high-income (Germany), one middle-income (Nigeria), and one lower-middle-income country (Vietnam).

# Approach

1. Research: We researched the case.
2. Data processing: We have created a pipeline for processing FAOSTAT data for any country, and turning it into suitable format for Mediation Analysis, and modelling. 
 - Example notebook: EDA/FAO_eda-Germany.ipynb
 - All countries we've analysed the results of have a separate notebook with the processing and exploration steps.
3. Modelling and Mediation Analysis
- We've performed a Mediation analysis to see if Food Supply per Capita has an effect on the realtionship between Food Losses and several nutrition indicators such as Dietary Energy Adequacy and Prevalence of Obesity.
- We've trained models: Logistic Regression, Random Forest...
4. Data analysis: we've compared the distributions of the features for each country (Germany, Vietnam, Nigeria) via visualization. We've analyzed the results of the Mediation Analysis and models.

# Conclusion  

This study examined how national-level food losses are associated with key nutrition and food security outcomes across countries, with a particular focus on the mediating role of food supply per capita. Using FAOSTAT panel data and a structured mediation modeling approach, the analysis highlighted the complex and often counterintuitive relationships between food system inefficiencies and public health indicators, including dietary energy adequacy, undernourishment, and obesity.

- Mediation Matters: Food supply per capita plays a role in mediating the relationship between food losses and nutrition indicators. Any interpretation of food waste effects should account for this mediating pathway.

- Context-Specific Dynamics: The varied patterns across Vietnam, Nigeria, and Germany emphasize that the impact of food losses is not universal. Factors such as baseline food insecurity, dietary norms, and economic development modulate these effects.

- Food Loss =/ Food Scarcity: Ironically, food losses may signal abundance rather than scarcity in many systems. Policymakers must consider that reducing food waste may not automatically enhance food security unless underlying supply and distribution structures are also addressed.

# Team 
Aysun Aliosman <br>
Spartak Tsakov <br>
Valeria Nikolaeva <br>

# References
1 Hannah Ritchie (2022) - “What is undernourishment and how is it measured?” Published online at
OurWorldinData.org. Retrieved from: &#39;https://ourworldindata.org/undernourishment-definition&#39; [Online
Resource]
2 Hannah Ritchie (2022) - “What is obesity and how is it measured?” Published online at
OurWorldinData.org. Retrieved from: &#39;https://ourworldindata.org/obesity-definition&#39; [Online Resource]
3 Max Roser, Hannah Ritchie, and Pablo Rosado (2013) - “Food Supply” Published online at
OurWorldinData.org. Retrieved from: &#39;https://ourworldindata.org/food-supply&#39; [Online Resource]
4 Van Dijk, M., Morley, T., Rau, M. L., &amp; Saghai, Y. (2021). A meta-analysis of projected global food
demand and population at risk of hunger for the period 2010–2050. Nature Food, 2(7), 494–501.
doi:10.1038/s43016-021-00322-9
5 Searchinger, T. et al. (2018). Creating a Sustainable Food Future—A Menu of Solutions to Feed Nearly
10 Billion People by 2050. World Resources Institute.
6. Todorova & Haralampiev (2024), “What Are the Impacts of Food Losses on Nutrition?”
