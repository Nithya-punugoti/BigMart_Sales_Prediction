<h1 align="center">BigMart Sales Prediction using Machine Learning</h1>

<p align="center">
Predicting Retail Product Sales using Machine Learning Models
</p>

<p align="center">
<img src="https://img.shields.io/badge/Python-3.x-blue?logo=python">
<img src="https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas">
<img src="https://img.shields.io/badge/NumPy-Numerical%20Computing-orange?logo=numpy">
<img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-yellow?logo=scikitlearn">
<img src="https://img.shields.io/badge/Matplotlib-Visualization-red">
<img src="https://img.shields.io/badge/Seaborn-Statistical%20Plots-purple">
</p>

<hr>

<h2>📌 Project Overview</h2>

<p>
BigMart is a retail chain that operates multiple outlets across different locations.
The objective of this project is to build a <b>machine learning model that predicts product sales</b>
at various BigMart outlets using historical sales data.
</p>

<p>
By analyzing product attributes and store characteristics, the model identifies
patterns that influence product sales and helps improve retail business decisions.
</p>

<hr>

<h2>🎯 Problem Statement</h2>

<p>
Retail companies need accurate sales predictions to optimize inventory,
improve product placement, and make data-driven decisions.
</p>

<ul>
<li>Product price (Item_MRP)</li>
<li>Product visibility</li>
<li>Product category</li>
<li>Store size</li>
<li>Store location</li>
<li>Store type</li>
</ul>

<p>
This project aims to build a predictive model that estimates the sales
of products at different retail outlets.
</p>

<hr>

<h2>📂 Dataset Description</h2>

<table border="1" cellpadding="6" cellspacing="0">

<tr>
<th>Feature</th>
<th>Description</th>
</tr>

<tr>
<td>Item_Weight</td>
<td>Weight of the product</td>
</tr>

<tr>
<td>Item_Fat_Content</td>
<td>Fat content category</td>
</tr>

<tr>
<td>Item_Visibility</td>
<td>Product visibility inside the store</td>
</tr>

<tr>
<td>Item_Type</td>
<td>Category of the product</td>
</tr>

<tr>
<td>Item_MRP</td>
<td>Maximum Retail Price</td>
</tr>

<tr>
<td>Outlet_Establishment_Year</td>
<td>Year the store was established</td>
</tr>

<tr>
<td>Outlet_Size</td>
<td>Size of the outlet</td>
</tr>

<tr>
<td>Outlet_Location_Type</td>
<td>Location tier of the city</td>
</tr>

<tr>
<td>Outlet_Type</td>
<td>Type of retail outlet</td>
</tr>

<tr>
<td>Item_Outlet_Sales</td>
<td>Sales of the product (Target variable)</td>
</tr>

</table>

<hr>

<h2>⚙️ Data Preprocessing</h2>

<ul>
<li>Handling missing values in <b>Item_Weight</b> and <b>Outlet_Size</b></li>
<li>Standardizing categorical values</li>
<li>Encoding categorical variables</li>
<li>Removing identifier columns not useful for prediction</li>
<li>Handling zero values in <b>Item_Visibility</b></li>
</ul>

<hr>

<h2>🧠 Feature Engineering</h2>

<p>A new feature was created:</p>

<pre>
Outlet_Age = Current Year − Outlet Establishment Year
</pre>

<p>
This feature captures how long a store has been operating,
which can influence customer trust and sales patterns.
</p>

<hr>

<h2>🤖 Machine Learning Models Used</h2>

<h3>Linear Regression</h3>

<ul>
<li>Baseline regression model</li>
<li>Used for predicting continuous values</li>
<li>Assumes a linear relationship between features and sales</li>
</ul>

<h3>Random Forest Regressor</h3>

<ul>
<li>Ensemble learning algorithm</li>
<li>Builds multiple decision trees</li>
<li>Handles nonlinear relationships better</li>
<li>Less sensitive to outliers</li>
</ul>

<hr>

<h2>📊 Model Evaluation</h2>

<table border="1" cellpadding="6" cellspacing="0">

<tr>
<th>Model</th>
<th>R² Score</th>
<th>RMSE</th>
</tr>

<tr>
<td>Linear Regression</td>
<td>~0.57</td>
<td>~1071</td>
</tr>

<tr>
<td>Random Forest</td>
<td>~0.59</td>
<td>~1047</td>
</tr>

</table>

<hr>

<h2>📈 Feature Importance</h2>

<ul>
<li>Item_MRP</li>
<li>Outlet_Type</li>
<li>Item_Visibility</li>
<li>Outlet_Location_Type</li>
<li>Outlet_Size</li>
</ul>

<hr>

<h2>🛠 Technologies Used</h2>

<ul>
<li>Python</li>
<li>Pandas</li>
<li>NumPy</li>
<li>Matplotlib</li>
<li>Seaborn</li>
<li>Scikit-learn</li>
</ul>

<hr>

<h2>📁 Project Structure</h2>

<pre>
BigMart-Sales-Prediction
│
├── data
│   ├── train.csv
│   └── test.csv
│
├── notebooks
│   └── Sales.ipynb
│
├── requirements.txt
└── README.md
</pre>

<hr>

<h2>▶️ How to Run the Project</h2>

<p>Clone the repository:</p>

<pre>
git clone https://github.com/Nithya-punugoti/BigMart_Sales_Prediction.git
</pre>

<p>Navigate to the folder:</p>

<pre>
cd Notebook
</pre>

<p>Install dependencies:</p>

<pre>
pip install -r requirements.txt
</pre>

<p>Run the notebook:</p>

<pre>
Sales.ipynb
</pre>

<hr>

<h2>🚀 Future Improvements</h2>

<ul>
<li>Hyperparameter tuning</li>
<li>Cross validation</li>
<li>Using boosting algorithms such as XGBoost</li>
<li>Deploying the model using Flask or Streamlit</li>
</ul>

<hr>

<h2>👩‍💻 Author</h2>

<p>
<b>Nithya Sri</b><br>
Computer Science & Data Science Student<br>
Interested in Machine Learning, Data Science, and Problem Solving
</p>
