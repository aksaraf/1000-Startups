# [1000-Startups](https://public.tableau.com/app/profile/akshay.saraf/viz/TopStartupsforVCInvestment/TopStartups#1)

## Project Overview
This data analysis project aims to provide insights for venture capital funds by analyzing over 1000 new startups to guide investment decisions.
The selection criteria for investments in this fund is based on a combination of:
1. High Revenue
2. Low Expense
3. Top Growth

## Data Source
The primary dataset utilized for this analysis is a CSV file containing financial and overview information about 1000 startups.

## Data Cleaning/Preparation
In the initial data preparation phase, I performed the following tasks:

- Data loading and inspection
  - The two sheets in the CSV file, Financials and Overview, are linked to each other using an inner join in Tableau.
    ![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/Inner%20Join.jpg)
- Handling missing values
- Data cleaning and formatting
  - Duplicate columns "ID" and "Name" have been removed.
  - Created folders to group the 2013–2014 and 2015 columns together.
    
    ![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/Folders.jpg)

## Exploratory Data Analysis
### 1. Number Of Companies Founded Each Year
The following bar chart displays the number of companies founded each year from 1999 to 2014.
![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/No.%20of%20companies%20founded%20each%20year.jpg)

We can use the group function in Tableau to combine the data from the previous years (1999–2009) together.
![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/No.%20of%20companies%20founded%20each%20other%20(group).jpg)

### 2. Average Number Of Employees In Each Industry
![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/Avg%20no.%20of%20employees%20in%20each%20industry.jpg)

### 3. Top 10 Startups By Growth %
![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/top%2010%20startups%20by%20growth%20%25.jpg)

### 4. 2015 Revenue vs. 2015 Expenses
Scatterplot

![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/2015%20Revenue%20vs.%202015%20Expenses%20Scatterplot.jpg)

Highlighted are the companies with higher revenue (>$9 million).

![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/2015%20Revenue%20vs.%202015%20Expenses%20Scatterplot(High%20Revenue).jpg)

Highlighted are the companies with lower expenses (<$5 million).

![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/2015%20Revenue%20vs.%202015%20Expenses%20Scatterplot(Lower%20Expenses).jpg)

Highlighted are the companies with higher revenue (>$9 million) and lower expenses (<$5 million). The Y-axis is reversed to position the quadrant on the top-right side.
![](https://github.com/aksaraf/1000-Startups/blob/97ac005c8d4353cf94221d1e4ab2dc027493daa4/Images/2015%20Revenue%20vs.%202015%20Expenses%20Scatterplot(High%20Revenue%20%26%20Low%20Expenses).jpg)

## Final Dashboard
The dashboard includes a revenue cutoff, an expense cutoff, and a slider for top startups by growth percentage. This allows venture capitalists to adjust the values according to their individual requirements when selecting the top startups for investment.
![](https://github.com/aksaraf/1000-Startups/blob/0be6a3816a19bc48fa3962288339eba8e145a666/Images/Top%20Startups.png)

## Reference
[Tableau Advanced: Master Tableau in Data Science](https://www.udemy.com/course/tableau10-advanced/)
