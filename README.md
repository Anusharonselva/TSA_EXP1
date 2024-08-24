# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 
### Developed by: ANUSHARON.S
### Register no.: 212222240010

# AIM:
To Develop a python program to Plot a time series data based on olympics nations medals distribution.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt

file_path = '/mnt/data/Paris 2024 Olympics Nations Medals.csv'
data = pd.read_csv('/content/Paris 2024 Olympics Nations Medals.csv')

plt.figure(figsize=(10, 6))

data.set_index('NOC')[['Gold', 'Silver', 'Bronze']].plot(kind='bar', stacked=True, colormap='viridis', ax=plt.gca())

plt.title('Paris 2024 Olympics Nations Medals Distribution')
plt.xlabel('National Olympic Committee (NOC)')
plt.ylabel('Number of Medals')

plt.legend(title='Medal Type')

plt.tight_layout()
plt.show()
```










# OUTPUT:

![Screenshot 2024-08-24 092116](https://github.com/user-attachments/assets/1249c8e8-c8b8-4739-b1c2-7af869ac4130)





# RESULT:
Thus the python code for plotting the time series of given data is created .
