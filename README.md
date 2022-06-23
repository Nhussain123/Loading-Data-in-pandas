# Loading-Data-in-pandas
Pandas is module for tabular data i.e spreadsheets, database

# Panda:
Load tabular data from different sources
Search for particular rows and columns
Calculate aggregate statistics
Combine data from multiple sources

# Panda introduces DataFrame

Easiest way to load DataFrame is through csv file.

Loading a CSV

import pandas as pd

df = pd.read.csv('ransom.csv')
print(df) to show dataframe

# Inspect a dataframe in short (first 5 rows)
df.head() 
print(df.head())

alteratively
df.info()
print(df.info())

df.info() provides details of data i.e rows, columns

# Selecting columns
Can be used in calculations
credit_records.price.sum()

Plot data
plt.plot(random['letter'], random['frequency'])

To select a column name:
suspect = credit_records['suspect']
print(suspect)

Alternatively
if column name only uses commas, names and _ you can use dotnotation
type name of variable followed by . then name of column
price = credit.report.price

If column contains special characters, space then must use [] and ''

# Select rows with logic
Logical statements checks for relationship between two values and returns true or false

== - checks relationship

question = 12 * 8
solution = 96
question == solution
True

Booleans = True and False

Other types of logic inc >,>=,<,<=

Price = 2.25
Price > 5.00
False

Not equal to - !
name= 'bayes'
name != 'Bayes'
True

Compare one value to all
credit_records.price > 20.00
returns whole column of true and false

By putting the statement in [] it will select places only where statement is true
credit_records[credit_records.price > 20.00]

credit_records - name then [credit_records.price > 20.00] - logical staement

Credit_records[credit_records.suspect == 'Ronald Aylmer Fisher'] To find specific names 

== means equal to
