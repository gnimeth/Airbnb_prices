# **Final Project - Chicago AirBnB Pricing Model**

### **Contributors:**

* Genevieve Nimeth
* Sandhya Datla
* Rebecca Levine
* Samuel Rose
* Caitlin Cavanaugh

### **About our dataset:**

* Used data collected from [Inside Airbnb](http://insideairbnb.com/get-the-data/) for Chicago which is updated quarterly for the last year. Our pull was from March 19, 2023	
	
	        
 ### **About our project:**

* Can we predict the future prices of AirBnB's across Chicago using location, property type, size of property, past pricing, and various review types?
* We sought to create a Data Model to check the reliability of the above variables in predicting price.
	* What are the main variables that contribute to pricing?

### **Restrictions:**
* AirBnB pricing varies per day of the week and on holidays - this type of pricing information was not within our dataset. 
	* Only date information provided was Host Since, First Review, and Last Review 
* Using provided location data was diffcult since there are many neighborhoods within Chicago and zip code data was not provided
	* Location data provided was not consistent across different categories. It did not include all Chicago neighborhoods. Some neighborhoods included had very 	      little data within them. 

### **Languages/Techniques Used:**
* Pandas
* Numpy
* Matplotlib
* RandomForest Regressor
* Standard Scalar
* OneHot Encoding
* Confusion Matrix
* Tableau
* GridSearchCV
	

## **Preparing the Data:**
* ETL process performed on dataset 
* Drop multitude of columns, remove NaN values, and locations not within Chicago city limits
* Ensure data types are appropriate to the categorical columns and numerical columns. Our target (Y variable) was converted to a float
* Identified price outliers using IQR 
* Used Get Dummies to help define our X variable within our model

## **Data Model Process:**
1) Eliminated columns in which data was not trainable.
	- Binned data so that samples with low frequency were bundled under other
	- Scaled the data.
	- Set up test environments.
	- Targeted/Y variable : price prediction
		- X variable : feature categoreis
	- Fit model
	- Elevated the model
	- Saved Model
	- Created optimized model
	
2) Select random samples from a given data or training set
3) This algorthim extracts random data entries for training
4) Voting will be performed for every predicted result
5) Select the most voted predicted result as the final prediction result


* Used 2 random processes - bootstrapping and aggregation
* Optimized our model using GridSearchCV and hypertuning parameters, which gave us the best fit for the model


## **Analysis:**
* Model produced inconclusive evidence that the chosen attributes could accurately predict pricing
	* Predicted pricing values produced were only accurate within $64, proving unreliable
		* Bedrooms was the highest contributing factor at 36%, followed by Accomodates at 16% and Reviews per Month at 8%







	 
