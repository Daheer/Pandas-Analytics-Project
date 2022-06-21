# Project XYZ

This project aims to explore the data gathered by the company XYZ.
It intends to do so by parsing the data into meaningful representations using pandas,
plotting graphs to pick out informative insights using seaborn and recommending the
appropriate further actions to be taken by the company depending on what
the insights are.

# Project Steps

**Step 1**: The necessary python libraries were imported, the csv files for each city was loaded and concatenated into a mother csv file. 

Libraries Imported 
- os
- glob
- pandas

Methods Used

- chdir()
- glob()
- concat()
- map()
- read_csv()
- to_csv()

**Step 2**: This step involved checking details about the data

Libraries Imported
- pandas
- numpy
- seaborn
- matplotlib.pyplot
- warnings

Methods Used

- head()
- describe()
- isnull()
- sum()
- info()

Attributes Used

- shape
- columns

**Step 3**: This step involved the parsing of the Date and Time column into new Day, Month, Year and Hour columns.

Libraries Imported

- datetime

Methods Used

- to_datetime()
- info()
- nunique()
- unique()

Attributes Used

- day
- month
- year
- hour

**Step 4**: Categorical type columns were looked into in this step.

Methods Used

- unique()
- tolist()
- value_counts()

**Step 5**: This step aggregates the data by some columns so statistical information like mean and sum can be gotten for those aggreated columns

Methods Used

- groupby()
- agg()
- sum()
- idmax()
- max()

**Step 6**: Plots were created using the data in this step. These plots show some very important information that gave insights which will be discussed in a later section of this report.

Plots Created

- countplot
- boxplot
- catplot of 'swarm' kind
- catplot of 'point' kind
- catplot of 'strip' kind

Methods Used

- set_title()

**Step 7**: This part was included as an extra to make this report standout from the rest. It includes more processing of columns and more creation of plots to provide extra insights about the data.

Plots Created

- catplit of 'count' type
- countplot
- barplot

Methods Used

- apply()
- strftime()

Expressions

- lambda expression


# Insights

1. Port Harcourt is XYZ's most profitable city with the maximum gross income coming from there
2. The maximum sales come from branch 'A'
3. The most used payment method is Epay, followed by Cash and Card respectively
4. The most sales come from Lagos city
5. The most bought product line is 'Fashion accessories' and the least bought is 'Health and beauty'
6. The line where cash is used most to pay is 'Electronic accessories', the products where epay is used most to pay is 'Fashion accessories' and the product line where card is the most popular means of payment is 'Food and beverages'
7. Epay is the most used payment method in branch 'A', Cash in branch 'C' and card in branch 'B'
8. The lowest rating of about 5.5 comes from branch 'B' and the highest at about 8.5 comes from branch 'C'
9. 'Health and beauty' products are mostly bought by females
10. 'Food and beverages' products tend to bought more in bulk.


# Future Work

XYZ could take note of the arrival and exit times of each customer in order to know the duration they used pondering whether they should by the product they checked out with. This would give even richer information of how easy it is to sell products to customers.

# Standout Section

- I created a catplot of the 'City' column with 'Customer type' as the hue paramter to show how:
    - Company XYZ rakes in more regular (non member) customers from Lagos.
    - Their member customers are more populated in Port Harcourt.
- I parsed the 'Date' column using strftime() method to create a new column 'Day_words' that stores the day in English. (Example: 1 would be 'Monday' and 7 would be 'Sunday')
- I then created a catplot (kind = 'count') of the newly created 'Day_words' column to show how:
    - Saturday, followed by Tuesday are the most popular days for shopping in Company XYZ's stores
    - Monday is less busy day at Company XYZ's stores
- I created a countplot of the 'Customer type' column with the hue parameter set to 'Gender' to show how:
    - XYZ has more female customers than male
- I plotted a catplot (kind = count) of the 'Hour' column to show how:
    - The highest amount of customers walk in to XYZ's stores at 19:00 or 7PM
    - The least favorite time to go into the stores is 5PM and 8PM
- I plotted a barplot of 'Rating' and 'Total' to show how:
    - Customers who enjoy XYZ's services tend to buy more items


# Executive Summary.

Can be found in <a href = 'Executive_Summary.md'> Executive_Summary.md </a>
