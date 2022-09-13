# Table-Price

Mythral Artifice is a VTTRPG Table making company that combines the functionality of a VTT with the classic DND experience of sitting at a table. As a founding member, I want to know what price we should charge for the table on our kickstarter to make the most profit. I need to gather data on previous successful Kickstarters and find the trend line for the price of the table, then calculate the cost of the table to produce, then find the point that they intersect to determine the best price for profit.

Business Question: What price should my Kickstarter table be for the most total profit?

Stakeholders: My team and I

Data Source: Kickstarter.com

Step 1: Options for Data sources

As Kickstarter is the platform that we will be launching on, I looked to find other successful kickstarter of similar product or with similar audiences. I searched in kickstarter for "table" in the "Games" category and ordered it by "Most Funded". I found that there were 9 Kickstarters from 8 companies that were considered successful (Reached their backing goal) that had both a similar player base and product. As the kickstarter pages were still accessible, I decided to use them for my external data collection as there were significant commonalities in the characteristics of the companies and their products to ours.

Step 2: Collect data

In the linked document called "Mythral Artificer Table Price Data", I gathered the pricing data on the successful Kickstarters to be able to analyze them. I pulled the Kickstarter link from the address bar, the Total Backers and Total Pledged from the top of the page, the Cost for most popular Pledge and Backers for most popular Pledge from the Support side bar.

As I am looking to calculate based on profit, I also was given the cost of materials and Labor for the table which was $2,557.00

Step 3: Clean Data

Problem 1: Pounds vs. USD

As some of these kickstarters ran outside of the US, they recorded their Pledged in Pounds. This created a situation where, if left alone, would compare incompatible currencies in the same data column. To fix this, I found the final funding day of each kickstarter and entered in the Pound amount into a historical rate calculator (www.x-rates.com/historical) to convert the pounds into USD based on the conversion rate at the time.

Problem 2: Inflation

As this data was created over several years as these kickstarters ran, the dollar value does not have a consistent meaning in the data as the power of the dollar fluctuated in that time. To make sure the dollar value was standardized, I brought all Pledged values to 2022 value using an inflation calculator (https://www.usinflationcalculator.com/). This is the data in the "Total Pledged (ADJ 2022)" and "Cost for most popular Pledge (ADJ 2022)" columns.

Problem 3:  Data outlier

Data point 1, "The Duchess", is very close to an outlier in the data, with a calculated z score of 2.75 in number of backers. Looking further into the datapoint, this was the first kickstarter of its kind, creating an abnormal situation in comparison to the rest of the kickstarters. Due to the near outlier data and unique situation, "the Duchess" will not be included in future calculations.

Step 4: Analyze the Data
A. Create Calculation for Profit per table: as Profit = Price - Cost, and we are willing to change price to increase profit, the profit equation goes like this: y = x - 1,757.00

B. Create total profit calculation: as total profit = profit per table * number of tables sold and profit per table = x - 1757.00, Total Profit = (x - 2557) * z where x is table cost and z is number of tables sold.

C. Create an equation that finds z using x: because we cannot easily solve an equation with two independent variables, we need to find the relationship between z and x to replace z in the total profit calculation. 

In our data, we have both the "Cost for most popular Pledge (ADJ 2022)" and "Backers for most popular Pledge". Using this data, we will create a scatterplot graph to find the trendline defining the relationship between these two values. As we cannot sell less than 0 tables, the trendline for this data will be exponential instead of linear. 

As shown in the Table Price Vs. Number of Backers, the exponential trendline is y = 2130e^-0.001x where y is number of backers and x is price of table. Compiling the Total Profit and quantity of backers per table price gives us Total Profit = (x - 2557) * 2130e^-0.001x.

D. Find the Maximum of the final Total Profit Equation: Using Wolfram alpha, we paste in the equation and ask for the maximum and it returns to us that the Total Profit is largest at the table price $3,575 with a calculated number of tables sold at 59.67 tables, rounded up to 60 tables, with a total calculated profit of $59,672

Step 5: Present the Data

The information above is reformatted in a PowerPoint deck including snippets of the graphs, data, and trends talked about above with a voice overlay. Please enjoy the presentation and give me feedback on what I can improve upon.

