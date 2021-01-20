1. Place all downloaded files in dataset/Download Dataset

2. Click on Notebook.bat

3. Run PrepareDataset - 
	It read all csv's  ,
	adjust dataframe,
	remove useless columns,
	remove countries where data is too less ( < 5 )
	fill missing values
	- saves dataframe in dataset

4. Corona Case Prepare file is not very useful.
	it fill 0 in remaining years and fills data in 2020 quarters and saves it in a dataframe


5.  Predict.ipynb

	It reads data from all datasets in ./dataset/ and country list from ./dataset/Downloaded Dataset.	
	Country List contains list of country for which model is executed
	
	Model - Random FOrest Regressor
	Training  and testing from 2000 Q1 to 2020Q2
	Predicting for 2020Q3

	
	To add more countries , we have to check if it we have proper dataset availbale for the country.
	then we can add that country in ./dataset/Downloaded Dataset/countries.csv


There is an Intersection.ipynb to check the countries for which data exist. But still some country data are useless as they are interpolate d with too less training data. Like only data for 5 6 years and interpolated for 20 years generated wrong data.
		



