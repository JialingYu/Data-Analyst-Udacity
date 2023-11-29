# Notes

#### Json file

Json file structure: two of JSON's types provide most of the format's flexibility for hierarchical data

json object: a collection of key-values pairs in the form like python dictionary

json array: like a python list

json object and array can nest together.


#### Web scraping, how to gather html files
we first get the webpage through url using requests.get() into a response object and then write the content of the response object into a file

#### Json vs Bson
JSON consumes less space and is comprehensible, whereas BSON consumes more space and is challenging to read. However, BSON is easy to programmatically parse, fast, and supports advanced data types compares to JSON.
