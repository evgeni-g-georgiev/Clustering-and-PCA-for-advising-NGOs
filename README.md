# Utilising clustering and PCA reduction methods to provide insights for NGOs

## Problem statement

**Problem Statement:** HELP International have been able to raise around $ 10 million. Now the CEO of the NGO needs to decide how to use this money strategically and effectively. So, CEO has to make decision to choose the countries that are in the direst need of aid. Hence, your Job as a Data scientist is to categorise the countries using some socio-economic and health factors that determine the overall development of the country. Then you need to suggest the countries which the CEO needs to focus on the most.

**About organization:** HELP International is an international humanitarian NGO that is committed to fighting poverty and providing the people of backward countries with basic amenities and relief during the time of disasters and natural calamities.

## Overview of my approach

**My approach is simple and can be explained broadly in three main steps:**

1. Analysis and characterisation of the broader dataset of all countries. I identify a pool of poorest countries.
2. Zoom-in on the poorest countries to better understand those facing the greatest hardship economically and from a public health crisis perspective.
3. Recommendations made taking our results into context.

**Brief summary of results:**

I identify Haiti as the prime contender for aid. It has the lowest life expectancy, the highest child mortality and is amongst the countries facing the greatest economic hardship.

**Other important observations:**

- I identify the following cluster of countries in greatest economic turmoil:  
[Afghanistan, Benin, Burkina Faso, Burundi, Cameroon, Central African Republic, Chad, Comoros, Congo, Dem. Rep., Cote d'Ivoire, Gambia, Guineau-Bissau, Haiti, Kenya, Kiribati, Lesotho, Liberia, Madagascar, Malawi, Mali, Mozambique, Niger, Rwanda, Senegal, Sierra Leone, Tanzania, Timor-Leste, Togo, Uganda]
- Identify the following cluster of countries in greatest public health struggle:  
[Angola, Burkina Faso, Central African Republic, Chad, Congo, Dem. Rep., Haiti, Mali, Niger, Nigeria, Sierra Leone]
- The following cluster of countries are amongst those with greatest economic turmoil and public health struggles:  
[Burkina Faso, Central African Republic, Chad, Congo, Dem. Rep., Haiti, Mali, Niger, Sierra Leone]

## Table of Contents

0. **Problem Statement**
1. **Overview of my results and my approach**
2. **Importing all relevant modules**
3. **Data Preparation**
   - 3.1 Importing the data
   - 3.2 Checking for any outliers
4. **Correlation Analysis**
5. **Principal Components Analysis (PCA) for dimensionality reduction**
   - 5.1 Running PCA and choosing the optimal amount of principal components
   - 5.2 Interpreting the PCA results
6. **Employing k-means clustering to classify the broader dataset**
   - 6.1 Elbow Method to find the optimal number of clusters
   - 6.2 Performing k-means clustering
   - 6.3 Visualising the clusters
7. **Focusing on poorer countries**
   - 7.1 Clustering: preparing the data
   - 7.2 Clustering: which countries face the greatest economic hardships?
   - 7.3 Clustering: which countries face the greatest public health crisis?
   - 7.4 Final Results: to be used in context and in collaboration with domain expertise
   - 7.5 The only specific recommendation I will make...
8. **Acknowledgements**

## Acknowledgements

Data downloaded from Kaggle website: https://www.kaggle.com/datasets/gauravduttakiit/help-international/data
