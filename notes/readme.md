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


#### Key dimensions of data quality:

1. Completeness is a metric that helps you understand whether your data is sufficient to answer interesting questions or solve your problem.
2. Validity is a metric helping you understand how well your data conforms to a defined set of rules for data, also known as a schema.
3. Accuracy is a metric that helps you understand whether your data accurately represents the reality it aims to depict.
4. Consistency is a metric that helps you understand two things: whether your data follows a standard format and whether your data’s info matches with information from other data sources.
Uniqueness is a metric that helps you understand whether there are duplicate or overlapping values in your data.

#### Three requirements for tidiness:

1. Each variable forms a column
2. Each observation forms a row
3. Each type of observational unit forms a table
