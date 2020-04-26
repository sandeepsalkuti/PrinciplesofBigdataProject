Working Functionality: Described work done in using each software

1)Spark: 
Installed spark and practiced basic queries in scala to understand twitter data and their results upon running queries.

2)IntelliJ IDE:
Created project in IntelliJ IDE and downloaded maven dependencies required like spark context and spark sql and added them to build.sbt. Wrote small scala program by importing spark sql.
Read json data which is downloaded tweets and  save in a temporary file named parquetFile and write 10 queries planned. Save each query using coalesce  into .csv file format. So by running the scala program all 10 queries get executed at a time and data is saved as each individual folders say q1, q2….

3)matplot:
Used matplotlib for plotting which is used for python programming language.
Wrote small python program where we imported matplotlib, pandas, numpy, glob which are used for plotting then using glob we read .csv file where our query results are stored and store them in a dataframe using pandas. Now read data from data frame and plot required diagram like bar, pie etc. based on need and label them and show diagram using show() function.

4)VisualStudio:
For showing the query results all at one place created a web application using python with Django . 
This is basic web page where user clicks a button and it executes query internally and saves the query results as plot image in folder and displays plot to user. So user clicks each query button and sees visualization part without any internal data.

IMPLEMENTATION:

• We wrote a Python program to stream the tweets and save them into JSON format, the output of the program contains the tweets with all the details like the IDs, Hashtags, Text, Users’s information, etc.

• The extracted JSON tweets are persisted into the Apache SparkSQL in the form of tables. We used 1 table to manage the data: o Table “parquetFile” to store each information of Json file .

• We used Scala to write queries and saved the output in .csv file

• We used python to read the saved .csv file using glob module, and while reading csv file ,we need to give the column names and store in the form the dataframe using pandas module

• After that we used matplotlib to visualize the data in pie chart, bar chart etc

• We used python with django framework  and pyspark to create web application where user can click on queries and see viualization.

Load data
• We need to read the generated json tweets data, after running the tweetsimport.py file

• In spark, it will store in the form of named column format ,and we give a table name

Steps to run the project

1)download PBproject folder and run the scala file,then it will run all the queries and save each query in separate .csv file(we can see in python files\outputcsvfiles)

2)next run the python files(python file\python code) for individual query and it will read data from csv file and it will plot in the chart(outputvisualization\visualization)

or

1) Download pb project folder and run in visualstudio code where we can run using command
py manage.py runserver
Before that install some libraries like
pip install pyspark
pip install django
pip install gmplot
pip install numpy
pip install pandas
