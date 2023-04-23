# Chicago AirBnB Pricing Model

### **About the dataset:**

* Used data collected from [Inside Airbnb](http://insideairbnb.com/get-the-data/) for Chicago which is updated quarterly for the last year. Data used was from March 19, 2023	
	
	        
 ### **About the project:**

* Can future prices of AirBnB's across Chicago using location, property type, size of property, past pricing, and various review types be predicted?
* Create a Data Model to check the reliability of the above variables in predicting price.
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
* Used Get Dummies to help define our X variable within the model

## **Data Model Process:**
1) Eliminated columns in which data was not trainable.
	- Binned data so that samples with low frequency were bundled under other
	- Scaled the data.
	- Set up test environments.
	- Targeted/Y variable : price prediction
		- X variable : key feature categoreis (bedrooms, accomodates, bathrooms, reviews per month, number of reviews, etc.)
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

## **Conclusions:**
* Despite limitiations, a model similar to this would still prove useful as it has potential to be further accurate with additional datasets   	 and feature categories.
* The overprediction that we got as our result is still more useful than an underprediction in pricing in this type of business landscape,    	especially for AirBnB guests







	 
