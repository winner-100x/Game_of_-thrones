FIBAL PROJECT
​
Please use version control and virtual environments in our work.
Please commit several times as your work progress with meaningful comments and create a requirements file so we can see what you are working with.
​
Now, as for the challenges, you find the data you need in the "data" folder and should be comprised of 3 files: csv_file.csv, json_file.json, txt_file.txt
​
The challenges are divided into 4 parts:
​
__API Access__
​
This challenge will involve querying an API and extracting information from it. The API in question provides information on Game of Thrones, allowing one to access information on the houses, characters and books.
​
* API URL: http://anapioficeandfire.com/api/{SECTION}/{INDEX}
​
Where SECTION can be either ‘books’, ‘characters’, or ‘houses’ and INDEX is an integer to a certain entry in a section.
​
For example, to access the character Peter Baelish, the full request would be http://anapioficeandfire.com/api/characters/823, where 823 is the index corresponding to that character. 
​
It's recommended to read the full documentation, which can be found here: https://anapioficeandfire.com/Documentation
​
We would like you to answer the following:
​
a) What index corresponds to the house “House Breakstone”?
 
b) How many males, females and unknown genders are there in the first 40 characters? Note, index 0 does not correspond to a character, so full range is 1 - 40 both ends inclusive. 
​
c) How many books can be accessed from this API?
​
d) How many books does the character ‘High Septon’ appear in? (ignoring ‘povcharacters’) 
​
Hint: index value of Septon needs to be found first; it is smaller than 20.
​
__File type manipulation and formatting__
​
Three files are presented, one CSV, one TXT and one JSON file. Each contain 1000 rows of data. There are two challenges, both involving collating these files into one data frame. The fields in all files are:
​
'author.properties.friends',  'author.properties.status_count',  'author.properties.verified',  'content.body',  'location.country',  'properties.platform',  'properties.sentiment',  'location.latitude',  'location.longitude'
​
where the ‘.’ Indicates a nested field.
 
a) Begin by collating the CSV and TXT files together into one pandas dataframe. The resulting dataframe should be 2000 rows and have all of the columns present in both files.
​
b) Next, using the created dataframe, integrate the data from the JSON file into the existing columns. The resulting dataframe should now be 3000 rows long.
​
__Data exploration__
​
In this challenge we would like to know something interesting about the data. You are free to explore as you wish, producing plots, tables, statistics, etc. Feel free to use any variables in the dataset or include external data you may consider relevant to complement your analysis.  
​
__Model creation__
​
For this task you can use AutoGluon or you preferred algorithm.
​
This final task involves creating a predictive model for a response variable, given a set of features. The task is to create a predictive model for the variable ‘properties.sentiment’ using the remaining features in the data set. 
​
The data files attached should be used to create the model.  
​
What we would like to see from this task is your thoughts and decisions on training and testing a model. This will include, but not limited to, considering aspects such as feature selection & creation, parameter tuning of the model and train / validation / test split. 
​
This task is a blank canvas to work with. The only caveat is that you must be able to explain the methods and models you are using.
