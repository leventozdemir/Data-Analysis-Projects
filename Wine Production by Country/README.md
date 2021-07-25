# Wine Production by Country

![intro_wme](https://user-images.githubusercontent.com/51120437/126898167-e48e873b-4ee7-4c40-873c-17ea76ac1abd.jpeg)

## - Library to install:
    pip install openpyxl

## - DataSet:
- Context: this dataset represents wine production by each country.

- Content: It can be used to by beginners for EDA, Data visualization etc.

- Acknowledgements: DataWorld.
- File Type: Excel.


## Calling libraries and data:

      import pandas as pd
      import matplotlib.pyplot as plt
      %matplotlib inline
      import seaborn as sns

      DATA_PATH = "DataSet/Wine_Production_by_country.xlsx"
      data= pd.read_excel(DATA_PATH, names=["Country","Year", "Wine production in mhl"], engine='openpyxl')
      
## Exploring the data:
      data.head()
      data.shape
      data.isnull().sum()
      data.columns
      countires= data.Country.unique()
      print(countires)
      print(len(countires))
      data.describe().transpose()
      
      
      
      
      
## Exploration Report:

- #### We have 120 line and 3  features
- #### No null Values
- #### the countries we have (24):
    - 'Italy'
    - 'France'
    - 'Spain'
    - 'United States'
    - 'Australia'
    - 'China'
    - 'South Africa'
    - 'Chile'
    - 'Argentina'
    - 'Germany'
    - 'Portugal'
    - 'Russia'
    - 'Romania'
    - 'New Zealand'
    - 'Greece'
    - 'Serbia'
    - 'Austria'
    - 'Hungary'
    - 'Moldova'
    - 'Brazil'
    - 'Bulgaria'
    - 'Georgia'
    - 'Switzerland'
    - 'World total'









## Data Visualization:
      data.hist(figsize=(15,5))
![bar](https://user-images.githubusercontent.com/51120437/126898332-688972e5-85d0-4d58-b3e5-e4963b2a3f83.png)

      plt.figure(figsize=(10,10))
      plot =sns.barplot(data['Year'], data["Wine production in mhl"])

![2](https://user-images.githubusercontent.com/51120437/126898344-9247c24b-3d89-44b7-8a11-af9070dbfd18.png)

      plt.figure(figsize=(10,10))
      plot =sns.barplot(data['Year'], data["Country"])
      plot.set(xlim=(data['Year'].min(), data['Year'].max()))

![3](https://user-images.githubusercontent.com/51120437/126898354-8d99c0f7-2b01-4cef-864e-0b7ea66c708b.png)

      data['Country'].value_counts().plot(kind='pie', figsize=(10,10), autopct="%1.2f%%")
      plt.title("Country Pie")
      plt.show()

![3](https://user-images.githubusercontent.com/51120437/126898369-d4ecb834-aadb-45b3-a24d-e815952b6eb8.png)

      data['Wine production in mhl'].value_counts().plot(kind='pie', figsize=(10,10), autopct="%1.2f%%")
      plt.title("Wine production in mhl Pie")
      plt.show()

![3](https://user-images.githubusercontent.com/51120437/126898375-76f2557e-7c14-45e6-9726-d6422796a18d.png)

      data_hight= data.loc[data["Wine production in mhl"]==2.3]
      data_hight['Country'].value_counts().plot(kind='pie', figsize=(10,10), autopct="%1.2f%%")
      plt.title("Country Pie")
      plt.show()

![3](https://user-images.githubusercontent.com/51120437/126898384-96f2f864-8bf4-4abb-b420-cdae3ea6ce0c.png)





#### The End:**By looking to the pie we can see that 2.3 is the most value repated in the data set so let's take it as our refference because too much production means too much using for this 2.3 is the most wanted type and we will see which country make production more.**









