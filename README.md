# Big_Data_EX_03

# EX_03 - Visualize data using basic plotting techniques in Python.

## Aim:

To visualize data using basic plotting functions provided by the Pandas library, such as bar plots, line plots, scatter plots, histograms, box plots, and hexbin plots.

## Requirements:

1. Python 3.x installed

2. Pandas library

3. Matplotlib library (usually installed along with Pandas)

4. Internet connection to load dataset
   

## Algorithm:

1. Import Pandas and Matplotlib libraries.

2. Load dataset from the provided URL using pd.read_csv().

3. Use the .plot() method on the DataFrame to create various plots like bar, line, scatter, histogram, box, and hexbin.

4. For plots requiring x and y axes (e.g., scatter, hexbin), specify column names.

5. Select subsets of columns to focus plots on relevant data.


## Program:
```
DEVELOPED BY : NIRAUNJANA GAYATHRI G R
REGISTER NO. : 212222230096
```
```
import pandas as pd  
import matplotlib.pyplot as plt  

# Step 1: Load the dataset  
df = pd.read_csv("https://waf.cs.illinois.edu/discovery/football.csv")  

# Step 2: Create a box plot of all numeric columns  
df.plot.box(title="Box Plot of All Numeric Columns")  
plt.show()  

# Step 3: Create a box plot of selected columns only  
df[["IlliniScore", "OpponentScore"]].plot.box(title="Box Plot of IlliniScore and OpponentScore")  
plt.show()  

# Step 4: Create a scatter plot of IlliniScore vs OpponentScore  
df.plot.scatter(x="IlliniScore", y="OpponentScore", title="Scatter Plot: IlliniScore vs OpponentScore")  
plt.show()  

# Step 5: Create a hexbin plot (density plot) of IlliniScore vs OpponentScore  
df.plot.hexbin(x="IlliniScore", y="OpponentScore", gridsize=25, title="Hexbin Plot: IlliniScore vs OpponentScore")  
plt.show()

```

## Output:

![image](https://github.com/user-attachments/assets/49bb86e9-f07b-4f65-a8cc-1a6d7ce73faa)


![image](https://github.com/user-attachments/assets/59bc0ddc-bb76-4521-9511-93ab4403c38f)


![image](https://github.com/user-attachments/assets/016651d1-b1ec-4157-8f4c-4bbcb06d2519)


![image](https://github.com/user-attachments/assets/07be2882-c7c9-4705-9464-bf84bba83b0a)


## Result:

Data visualization was successfully performed using Pandas plotting methods. Different plot types were used to explore the dataset, highlighting score distributions and relationships. Specifying columns and plot types allowed focused insights from the dataset.




