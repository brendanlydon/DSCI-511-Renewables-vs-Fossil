-- API INFORMATION --
Code can be found at my Github Profile:
	https://github.com/brendanlydon

Main EIA Site:
	https://www.eia.gov/
	
Main API Site:
	https://www.eia.gov/opendata/
	https://www.eia.gov/opendata/qb.php 
	
API Mapping:
	Electricity ---> Net Generation ---> By Fuel Type ---> Fuel Type ---> State
	Electricity ---> Total Consumption ---> By Fuel Type ---> Fuel Type ---> State
	Electricity ---> Retail sales of electricity ---> State
	Electricity ---> Average Retail Price of Electricity ---> State
	Electricity ---> Revenue from Retail Sales of Electricity ---> State
	Electricity ---> Number of Customer Accounts ---> State
	
	
-- PROJECT OVERVIEW --
With climate change shaping up to be arguably the biggest challenge humanity has ever faced in our long history, this data set hopes to start looking into where our electricty is coming from in the 21st century: Renewables vs Fossil Fuels. The data pulled into the electricty_data.csv file looks at nearly two decades worth of information on every state in the U.S., broken down by month and the fuel source used. 
	
The goal is three-fold:
	1. To see where our power generation is coming from;
	2. To understand directionally where the U.S. is heading when it comes to sourcing our power generation;
	3. To ultimately model out the financial impact of moving 100% of the country's power generation to renewable energy.

For reference, the definition of each heading in the electricity_data.csv file (to be generated) is listed below:
	prime_category: Dictates whether we are looking at generation, consumption, costs, etc..
	series_name: The final data series used to generate the data in this row from the EIA Website.
	period: The month corresponding with this row of data. 202107 = August, 2021
	frequency: The relevant reporting frequency. In this case, it is always by month but can be pulled by Year or Quarter as well.
	fuel_type: Whatever fuel source was used to generate the electricty (coal, hydroelectric, gas, etc.)
	energy_type: Renewables, Non-Renewables, or All (See list below for specifics). If all, it is indeterminate.
	value: The corresponding numerical value for each given row.
	units: The unit type corresponding with each row.
	
-- CHALLENGES / CONCERNS --
First, I do not go down to the level of sector (Industry, commercial, etc.). This is the final level of data available on the site and is something I may end up pull into the final dataset before the class is over. This will give a deeper view into where the electricty being generated is both coming from and going towards.

Second, all of the financial data doesn't seem to be split by renewable generation vs. fossil fuel generaiton. This could just be something I'm missing from not being as familiar with the industry as I should be, but it is an important piece that I would like to include.

Including both the sectors and the financial impact split between renewable energies and fossil fuels is something that I think will push this data to another level. Ultimately, this is what I'm trying to hone in on so it is crucial to make that connection.