dsa v073.5 (Release date: 2020-03-05)
==============
Changes:
	- Bug fix: Now multiple external regressors can be added correctly

dsa v073.5 (Release date: 2020-03-05)
==============
Changes: 
	- fixed bug in xts2ts for leapyears

dsa v073.3 (Release date: 2020-01-20)
==============
Changes: 
	- dow_dummy now has an option delete 29_2 to make it possible to delete the values for the 29th of February
	- Improved treatment of 29th February


dsa v0.72.1 (Release date: 2019-11-01)
==============
Changes: 
	- In drop31, more iterations are allowed, to find the correct length of the dates for the new variables



dsa v0.71.6 (Release date: 2019-10-10)
==============
Changes: 
	- In output: for the graphics cairo-png is no longer used, as on some devices it does not create graphics


dsa v0.70.1 (Release date: 2019-04-04)
==============
Changes: 
	- Bug fixes:  - Some minor code clean-up

Additional Functionality:
	- get_sa, get_trend, get_original: Inclusion of helper function to quickly get the most important series from the seasonal adjustment




dsa v0.64.1 (Release date: 2019-03-26)
==============
Changes: 
		- output(): Now contains additional visualizations of the outlier adjustment


dsa v0.63.3 (Release date: 2019-02-26)
==============
Changes: 
- Bug fixes  
	- Multiple regressors were sometimes not considered correctly
	- In output(): Last graphic of spectrum previously showed original instead of seasonally adjusted series


dsa v0.62.1 (Release date: 2019-02-10)
==============
Changes: 
- Bug fixes (thanks to Fernando Kawaoka and Rodrigo da Silva)
	- outlier estimation in case of too low critical value was not processed correctly
        - Creation of dummy variables mixed up from and to values
	- improved the fill_up function to correctly identify the 29th of February even if there is some mismatch of series length



dsa v0.60.35 (Release date: 2019-01-04)
==============
Changes: 
- Bug fixes
	- descaler: set y=NA as a default. Otherwise when descaler is only used for log-transformations, as then y does not need to be supplied, it lead to an error




dsa v0.60.34 (Release date: 2019-01-04)
==============
Changes: 
- Bug fixes
	- drop31: fixed an error that could lead to faulty transformation
	
	

dsa v0.60.33 (Release date: 2019-01-04)
==============
Changes: 
- Bug fixes
	- fixed the fill_up function to correctly identify the 29th of February



dsa v0.60.32 (Release date: 2019-01-04)
==============

Changes: 
- Changes
	- Minor changes of examples to decrease run time


dsa v0.60.31 (Release date: 2018-10-29)
==============

Changes: 
- Bug fixes
	- previously, setting option reiterate3 > 0 in the dsa function did not work together with diff > 0
	- if scaling the data became active in the dsa function, the data where not propably rescaled at the end
	- fixed display of SI ratios for annual period


dsa v0.60.21 (Release date: 2018-10-19)
==============

Changes:

* First public release of the dsa package