# Assignment3
Some researchers think that the investors' emotions could affect the price of assets and futhermore affect the return of assets. Malcolm Baker & Jeffrey Wurgler(2006) used PCA(Priciple Component Analysis) and comstruct an investor emotion factor with 6 observable variables. Dashan Huang(2013) found that PLS(Partial Least-square Method) is also an efficient way to construct investor emotion factors to predict the return of stock returns.

In this job, I construct a MySQL database contains multiple possible variables related to investors' emotions. The python files in ./db/ implement the functions of creating the tables(if you haven't created one) and updating the data. In advance of running these files, you first need to construct two schemas "emotions" and "stock_index" in your MySQL database and revise the database address in ./db/configuration.py 

The csv files in ./data is the data exported from the MySQL database, you could just run the python file ./save_data.py to export data from MySQL to csv files. Just remember to revise the database address in ./config.py

The python file corr.py is used to calculate the correlations and make a regression between variables and the return of stock index you choose. The PCA.py and PLS.py implement the functions of constructing factors by using PCA or PLS methods with the variables you choose in the database. Just change the value of list variable X with the emotion variables you choose in the python files.
