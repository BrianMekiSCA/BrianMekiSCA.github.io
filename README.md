# Main Objective
This post seeks to examplify steps that could be employed by Data Scientist to address business questions.

# Scenario
Consider this overly simplified situation. An entrepreneur wishes to open a simple shop say in Istanbul. Immediately, some of the questions they may ask could be,
1. What might be the best location to setup the shop?
2. What goods might be worthwhile selling?
3. Can demand be expected to vary between males and females?

# How to Prepare a Responce
As a data scientist, it first imperative to understand the business needs clearly as this will significantly influence the type of data sourced and used to address the issue.
Said data could be collected first-hand or obtained from existing sources.
For the situation hypothesized above, this existing [Istanbul Customer Shopping Data](https://www.kaggle.com/datasets/mehmettahiraslan/customer-shopping-dataset) suffices to provide rudimentray yet data-driven answers to the questions posed.

# Steps Taken To Analyze the Data
Generally, the first step taken is to clean and preparing the data to aid in answering the question(s) asked. This could involve;
1. Identifying and retaining information most relevant to the task at hand,
2. Fixing incorrect data, removing corrupt infomation and /or addressing incomplete information.

The choice of tool(s) employed are at the discretion of the data scientist. These could include such programming languages as R and Python which 
can be used to not only clean the data but also analyze it and visualize the resulting outcome. In this blog, Python was the tool of choice. 

Putting all this together results in the following:

# 1. What might be the best location to setup the shop?
Here it was necessary to determine the best mall for the entrepreneur's shop. To this end, only the following columns were deeemed necessary to analyze;
shopping_mall, price and quantity. Firstly, it was necessary to understand if any of the Malls generally sold relatively lots of goods cheaply or on the other streme, sold few but expensive items. To help in this led to analysing the weighted average item cost price per mall. This was found to be roughly the same 
across malls at around 842 or, proportionally, about 10%. What this implied was that the the quantity of goods sold would be most indicitive of the 
mall that sell the most number of items. This happens to be The Mall of Istanbul which sold about 20.1% of all units with Kanyon close behind at 19.9%. 


# 2. What goods might be worthwhile selling?
The product categories to invest in once the shop is located in the Mall of Istanbul is Clothing as it has the most items bought at roughly 35%. 
In second and third places would be Cosmetics and Food&Beverage with 15.3% and 14.8% of the units sold respectively. Together these categories amount to about 65%
of all units sold at this particular mall.



# 3. Can demand be expected to vary between males and females?
The average number of items consumed by males versus that consumed by females is roughly the same at approx 3 with a standard deviation of 1.4. It stands to reason 
that males and females show the same demand for goods. 

# Conclusion
In Conclusion, the entrepreneur will be well advised to open their shop in the Istanbul Mall where they can immediately start selling Clothing, Cosmetics and Food&Beverage as these product categories have shown to be a significant proportion of the market. Though gender might play a role in the buying tendancies of the cutomers, ultimately, the demand is relatively symmetrical. As result, keep enough stock of each product category at all times.   
