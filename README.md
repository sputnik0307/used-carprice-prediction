## Car Price Prediction

The objective of this project to make a end to end machine learning project and help others in figuring out their old car's selling price.

Hence,for instance, we get data from the car website CarDekho.com, filled with information on a wide variety of cars, including their selling price and present price. We realize that we can use this data to make sure we get a good deal on a new car. In particular, we can figure out exactly how much one should pay for a specific type of car.

### Data Information
This dataset contains information about used cars listed on www.cardekho.com This data can be used for a lot of purposes such as price prediction to exemplify the use of linear regression in Machine Learning. The columns in the given dataset is as follows:

* Car_Name
* Year
* Selling_Price
* Present_Price
* Kms_Driven
* Fuel_Type
* Seller_Type
* Transmission
* Owner

I have used the RandomForestRegressor to solve this ML problem.

## Deploying ML Model using Flask
This is a simple project to elaborate how to deploy a Machine Learning model using Flask API

### Prerequisites
You must have Scikit Learn, Pandas (for Machine Leraning Model) and Flask (for API) installed.

Flask version: 0.12.2 conda install flask=0.12.2 (or) pip install Flask==0.12.2

### Project Structure
This project has four major parts :

* model.py - This contains code fot our Machine Learning model to predict car selling price from the data in 'car data.csv' file.
* app.py - This contains Flask APIs that receives employee details through GUI or API calls, computes the precited value based on our model and returns it.
* template - This folder contains the HTML template (index.html) to allow user to enter employee detail and displays the predicted employee salary.
* static - This folder contains the css folder with (style.css) file which has the styling required for out index.html file.

### Running the project
* Ensure that you are in the project home directory. Create the machine learning model by running below command from command prompt.

      python model.py 
       
* This would create a serialized version of our model into a file model.pkl

* Run app.py using below command to start Flask API

      python app.py
   
* By default, flask will run on port 5000.Navigate to URL http://127.0.0.1:5000/ (or) http://localhost:5000
* Enter valid numerical values in all input boxes and hit Predict.

If everything goes well, you should be able to see the predcited car selling price on the HTML page! check the output here: http://127.0.0.1:5000/predict

