# Ali Ahmed - Data Analysis Portfolio

# About
I'm Ali! Recent graduate, obtaining a Bachelor of Art (B.A) degree from New York University, with major in Economics. Currently seeking Data Analyst opportunities as I to hone my skills in various programming languages (SQL, Python). Self-taught SQL using w3schools and datalemur.

This repository serves as a showcase of my skills, a place to share my projects, and a way to track my progress in Data Analytics and Data Science-related topics. 

# Portfolio Projects

For this project, I worked on a dataset of video game sales found on kaggle, where I graph the trend of different element of video games over the range of time period. I wanted to do this particular project because I love games myself, and was interested to see how was the game like from 1980s and how the trend changed overtime. 

I begin with data cleaning, where I removed all data from 2016 to 2020, since they were not enough information to show the flow of the market. I've also deleted any rows with NULL value for either platform and/or year column. After removing the datas, I used WITH, RANK(), and window function to reset a column for ranking. 

Then, to see if there is any duplicate game names and global_sales, I decided to use join function, joining the table to itself to see if anything is equal.

After finish up cleaning the data, I asked several question for the dataset, and answer them by querying the data 
How many times did one region had the most sales for each different games over the each year?

Visualization 
-
My first question is, how many times did one region had the most sales for each different games over each year?

To query this, I used a with function to make a temporary table with a case statement to add a count each time a region tops the sale for the game. To visualize the result, I used public tableau linked below:

https://public.tableau.com/app/profile/ali.ahmed3520 
![Screenshot_2](https://user-images.githubusercontent.com/121634275/222937327-78618396-1999-4760-b16e-e26af601746d.png)

I approached with this question because I wanted to know which region is the biggest market over the years. Looking at the graph, Japan had the most sales in 1980s. After around 1995, sales in North America drastically surpassed the market in Japan. I assume this was the case because popular publisher started off in Japan as their first entry to the industry, then later on 1995, they spread their business across the world, and North America generally having the biggest market, the amount of top sales will be at NA. Another thing to note here is that newer publisher around the world entered the gaming industry, which would affect also the total sales.

Now that we know North America having the largest market, now we want to know what is the top publisher in general, and the metric here is the amount of total profit.

![Screenshot_1](https://user-images.githubusercontent.com/121634275/222937328-91f689d1-e8c5-4514-bdd0-8aeff67c5186.png)

Here, I have decided to list top 20 publishers by their profit using the TOP function on SQL. I was curious about the quantity of games the top publishers have produced in total, since I wanted to know if the quantity mattered in gaining much profit. In the bar graph, most company has greater profit if they have greater quantity. However, it was not the case for one publisher, being Nintendo. It has less games than publisher like Electronic Art and Activision, but has greater profit. Quantity of the games usually correspond to the profit, but not always.



![Screenshot_3](https://user-images.githubusercontent.com/121634275/222937566-13220c64-4931-4f90-b54c-86f57561f534.png)
