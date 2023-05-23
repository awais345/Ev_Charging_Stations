# Electric Vehicle Charging Sessions Analysis

This repository contains the dataset gathered from the field experiment [A Field Experiment on Workplace Norms and Electric Vehicle Charging Etiquette](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/NFPQLW) by Professor Omar Asensio from School of public policy, Georgia Tech uniersity. The dataset consists of information from 3395 high-resolution electric vehicle charging sessions. These sessions were recorded as part of a workplace charging program, involving 85 EV drivers, 105 stations, and 25 sites. The workplace locations encompass various facilities, including research and innovation centers, manufacturing sites, testing facilities, and office headquarters.

# Dataset
The dataset 'station_data_dataverse' is provided in a .CSV format. It contains anonymized data, ensuring the privacy of the individuals and organizations involved. Each charging session record includes details such as charging duration, energy consumption, charging cost, station ID, site information, and driver information.

# Data Dictionary
* sessionId: a random number used to identify a specific electric vehcile (EV) charging session
* kwhTotal: the total energy use of a given EV charging session, measured in kWh
* dollars: the amount paid by the user for a given charging session, measured in U.S. dollars
* created: the date and time a given session was initiated, expressed in the form "YYYY-MM-DD HOUR:MIN:SEC"
* ended: the date and time a given session was terminated
* startTime: the hour of day, from 1 to 24, during which the session was initiated
* startTime: the hour of day, from 1 to 24, during which the session was terminated
* chargeTime: the total duration of the session in hours
* weekday: the day of the week on which the charging session took place
* platform: the digital platform used by the EV driver to log the session
* distance: the distance from a user's home to the charging location, expressed in miles except where user did not report address
* userId: a random number used to uniquely identify a given user and his or her transactions
* stationId: a random number unique to each specific charging station
* locationId: a random number unique to a specific location owned by the firm, where chargers were installed
* managerVehicle: a binary variable; 1 if the vehicle logging the transcation is of the type largely used by firm managers, 0 otherwise
* facilityType: a categorical variable indicating the type of facility a station is installed at; manufacturing = 1, office = 2, research and development = 3, other = 4
* Mon, Tues, Wed, Thurs, Fri, Sat, Sun: binary variables for day of week of a given session; 1 if the session occurred on that day of week, 0 otherwise
* reportedZip: binary variable for if a user reported his or her zip code; 1 if zip code was reported, 0 otherwise

# Analysis Methodology
The analysis of the dataset is performed using Python and various data analysis libraries, such as Pandas, NumPy, seaborn and Matplotlib.

# Analysis Steps
The Jupyter Notebook file, EV_Chraging_stations.ipynb, contains the step-by-step process of analyzing this dataset. The notebook provides detailed explanations of each analysis step, including data preprocessing, exploratory data analysis, and generating visualizations.

# Results and Insights
The analysis yields valuable insights into charging behaviour, power consupmtion, charging costs, devices (android, IOS, web) used to log charging session, and the charging pattern at various locations. 
