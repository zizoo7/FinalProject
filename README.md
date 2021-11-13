Summary:

The project deals with the analysis of information about the corona virus in the world,
Data analysis is based on information from Johns Hopkins University,
The data were taken from:
https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series

Transformation of the data was performed in 2 different forms on the same information:

	Power bi

	Ssis

Details of the project in power bi:

	Import the data from web in 3 table

	The three tables perform a transformation of:

		Unpivoted other columns in the table
		
		Then merge three tables to a new table

	Another table of date that I build like data table.

	The measure built for data analysis are:

		Daily_New_Cases

		Total_Confirmed

		Total_Deaths

		Total_Recovered

		Recovered_rate_Of_Confirmed

		Death_rate_Of_Confirmed

	After arranging the data and building the measure the reports built are for a global overview by country on:


Details of the project in ssis:

	In ssis folder you can find file:

		Python for Treatment the data

		Csv data file with result after python

		Flow chart of the ssis

	Steps in project execution:

		Script Import and clean and join 3 table data with python and then pool the data to data flow task

		In the data flow you can find Basic construction of a data warehouse with 2 tables can be found by checking every time new information arrives if it already exists or does not exist in the table

		In the final step can be fond the new db whit the table