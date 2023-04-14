# **Final Project - Chicago AirBnB Pricing Model**

### **Contributors**:

* Genevieve Nimeth
* Sandhya Datla
* Becca Levine
* Samuel Rose
* Caitlin Cavanaugh

### **About our dataset**:

* Used data collected from [Inside Airbnb](http://insideairbnb.com/get-the-data/) for Chicago which is updated quarterly. Our pull was from March 19, 2023	
	
	        
 ### **About our project**:

* Can we predict the future prices of Airbnb's across Chicago using location, property type, size of property,  past pricing, and various review types?
* Want to get a feel for some great Chicago Airbnb's based on what future pricing is likely to be? Then check out our Data Model!

### **Restrictions**:
* Pricing varies per day of the week as well as holidays and this type of data was not within our dataset, so we have to use other prediction factors outside of the realm of time
* Using provided location data was diffcult since there are many neighborhoods within Chicago and zip code 		information was not provided

### **Languages/Techniques Used**:
* Pandas
* Numpy
* Matplotlib
* RandomForest Regressor
* Standard Scalar
* OneHot Encoding
* Confusion Matrix
* Tableau
* GridSearchCV
	

## **Preparing the Data**:
* ETL process performed on dataset 
* Drop multitude of columns, remove NaN values, and locations not in Chicago not relevent to our goal
* Ensure data types are appropriate to the categorical columns and numerical columns. Our target Y variable was 	converted to a float
* Identified price outliers using IQR 
* Used Get Dummies to help define our X variable within our model

## **Process:**
- Eliminated columns that’s data was not trainable.
	- Binned data so that samples with low frequency were bundled under other.
	- Scaled the data.
	- Set up test environments.
	- Targeted variable Y: price prediction
		- X variable is our features
	- Fit model
	- Elevated the model
	- Saved Model
	- Created optimized model.
	- 
1) Select random samples from a given data or training set
2) This algorthim extracts random data entries for training
3) Voting will be performed for every predicted result
4) Select the most voted predicted result as the final prediction result

* Used 2 random processes - bootstrapping and aggregation
* Optimized our model using GridSearchCV and hypertuning parameters, which gave us the best fit for the model


## **Analysis:**
* Model produced inconclusive evidence that the chosen attributes could accurately predict pricing
	* Predicted pricing values produced were only accurate within $64, proving unreliable
		* Bedrooms was the highest contributing factor at 36%, followed by Accomodates at 16% and Reviews per Month 			at 8%







	 
