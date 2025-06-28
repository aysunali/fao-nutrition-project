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
  
