# Diamonds-Price-Prediction
## Description
The "Diamonds" dataset contains tens of thousands of records of diamonds and their price, as determined by experts. In this Project we will analyze the data (by their cut, color, clarity, price, and other attributes) and draw conclusions from the data and build a model that can predict diamond prices according to their characteristics.
![Image](https://repository-images.githubusercontent.com/355545549/cd08f880-b4f0-11eb-878d-7a636e555189)
## Diamonds Dataset 
This classic dataset contains the prices and other attributes of almost 54,000 diamonds. It's a great dataset for machine learnung and work with data analysis and visualization.

### Dataset Columns :
- price : price in US dollars ( $326 - $18,823 )

- carat : weight of the diamond ( 0.2 - 5.01 )

- cut : quality of the cut ( Fair , Good , Very Good , Premium , Ideal )

- color : diamond colour, from J ( worst ) to D ( best )

- clarity : a measurement of how clear the diamond is ( I1 (worst) ,SI2 ,SI1 ,VS2 ,VS1 ,VVS2 ,VVS1 ,IF (best))

- x : length in mm ( 0 - 10.74 )

- y : width in mm ( 0 - 58.9 )

- z : depth in mm ( 0 - 31.8 )

- depth : total depth percentage = z / mean( x, y ) = 2 * z / ( x + y ) --> ( 43 - 79 )

- table : width of top of diamond relative to widest point ( 43 - 95 )

![Picture](https://user-images.githubusercontent.com/57026889/214210835-74392e2a-0931-4ca4-84e9-ab28c2e938a2.png)

## Visualize the Data
1. Examine distribution of target variable(price)

![Picture2](https://user-images.githubusercontent.com/57026889/214001286-16052584-036a-49eb-a415-916a1a48dd93.png)

2. Histogram all colomns



![Picture2](https://user-images.githubusercontent.com/57026889/214210929-ff4a7f9b-bae4-4773-8fd1-7cfa7f820882.png)

3. Relation between all columns and Categories.


![Picture3](https://user-images.githubusercontent.com/57026889/214211008-f3c936a2-b29d-48a8-b6fc-883f13c08bf2.png)
## Encoding Categorical Variable
We change the values of the categorical features to numeric values according to their quality, so that the model will be affected by these characteristics.
## Relationship between volume and price.
We added a feature to the dataset that represents the volume of the diamond.
## Regression Algorithms Models
1. Linear Regression
2. Random Forest Regressor
3. Decision Tree Regressor
## Results

- Linear Regression
 
 ![Picture6](https://user-images.githubusercontent.com/57026889/214211398-3f834ef3-9d2d-41cf-a496-cce280e4b6ea.png)
 
 ![Picture7](https://user-images.githubusercontent.com/57026889/214211489-5cb3456c-3689-459e-9130-1942c72c88b8.png)
 
***r2_train          :  0.9077967797893242
linear regression accuracy: 
r2_test       :  0.9105122393034278
mae           :  801.6381032948378***


- Random Forest Regressor
***R2_train          :  0.9974101929649611
Random Forest Regressor accuracy: 
R2_test       :  0.9817868852797156
MAE           :  267.9479157669652
MSE (RMSE)    :  293265.5578559805  ( 541.5399873102452 )****
- Decision Tree Regressor
***R2_train          :  0.9999954501781485
Decision Tree Regressor accuracy: 
R2_test       :  0.9656613097730191
MAE           :  357.357103115727
MSE (RMSE)    :  552917.7902911721  ( 743.5844204198822 )******
