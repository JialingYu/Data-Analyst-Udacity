# Notes
## Gathering data
#### Json file

Json file structure: two of JSON's types provide most of the format's flexibility for hierarchical data

json object: a collection of key-values pairs in the form like python dictionary

json array: like a python list

json object and array can nest together.


#### Web scraping, how to gather html files
we first get the webpage through url using requests.get() into a response object and then write the content of the response object into a file

#### Json vs Bson
JSON consumes less space and is comprehensible, whereas BSON consumes more space and is challenging to read. However, BSON is easy to programmatically parse, fast, and supports advanced data types compares to JSON.

## Accessing data

Two types of unclean data: dirty data(data quality issue) and messy data(data structural issue). 

### Data quanlity issue

#### Key dimensions of data quality:

1. Completeness is a metric that helps you understand whether your data is sufficient to answer interesting questions or solve your problem.
2. Validity is a metric helping you understand how well your data conforms to a defined set of rules for data, also known as a schema.
3. Accuracy is a metric that helps you understand whether your data accurately represents the reality it aims to depict.
4. Consistency is a metric that helps you understand two things: whether your data follows a standard format and whether your data’s info matches with information from other data sources.
Uniqueness is a metric that helps you understand whether there are duplicate or overlapping values in your data.


### Data tidiness issue
#### Three requirements for tidiness:

1. Each variable forms a column
2. Each observation forms a row
3. Each type of observational unit forms a table

a. There are many common issues that make data messy:

1. Column headers are values, rather than variable names

2. Multiple variables are stored in one column

3. Variables are stored in both rows and columns

4. Multiple types of observational units are stored in the same table

5. A single observational unit is stored in multiple tables.


b. Analytical data set: Analytical data helps us perform analyses, like visualizing trends or training machine learning models. Data tidiness is essential for analytical datasets, as analytical data is often used to help with business decision-making and is typically based on big data. Merging data from additional sources by defining a clear analysis unit can help enrich your dataset's value. Units of analysis can be individuals, groups, artifacts (i.e., items like books), and geographical units (e.g., states). Note that while a unit of analysis is the item you want to structure your data around, a unit of observation is the item you can actually observe. Unique keys can help with merging multiple datasets/data tables. Note that both primary keys and unique keys can be used to uniquely identify records in a table; however, a primary key does not allow NULL values, whereas a unique key can allow one NULL value per column and can be used for additional uniqueness constraints on columns other than the primary key. When defining analytical datasets, you need to consider the granularity and aggregation level in your dataset.

