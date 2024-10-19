# Census Data Standardization and Analysis Pipeline
**Description :**
Census Data Standardization and Analysis Pipeline is a basic project for learning Data cleaning and analysis. Data is first imported from a CSV file, then the columns are standardized as per the requirements, then comes the cleaning part and then finally Visualizing some valuable insights from the cleaned data. Between this cleaning and visualiations parts, the cleaned is first inserted into MongoDB (NoSQL DB) and then retrived from it to store in a MySQL DB; from where the data is retrieved as per the required queries to visualize the data.

**Tools used :**
Python, Pandas, Matplotlib, MySQL Connector Python, PyMongo, Streamlit

**Basic workflow :**
1. Start
2. Read the data from CSV file
3. Standardize the column names
4. Edit the existing data to comply with new rules
5. Identify the percentage of missing data for each column before cleaning
6. If all required values are available (Not Null):
>>>True: Fill the values based on the calculation performed on the values
>>>False: Do not fill
7. Identify the percentage of missing data for each column after cleaning
8. Write the missing data details in a new file for visualization
9. Upload the cleaned data into MongoDB
10. Retrieve the stored data from MongoDB and upload it to MySQL
11. Query the MySQL DB and display the results in Streamlit 
12. End

**Caution**

**Note :**

1. Please make sure that you're connected to the MySQL server before running the files.
2. Please run the CensusDataPipeline.ipynb first. The CensusDataPipeline.ipynb file consists the Data imports, cleaning and uploading to Database.
3. Before running the CensusDataPipeline.ipynb file make sure to change the variable uri with your MongoDB localhost connection string. (At the beginning of Task 5)
4. Please make sure that you have installed streamlit before running the Census2011_Queries.py file.
5. In case if you've not installed streamlit previously, open the Project document in VS Code, open the terminal and execute the command - pip install streamlit.
   Or just open command prompt and execute the command pip install streamlit.
6. In order to run the Census2011_Queries.py, open the terminal and execute - streamlit run Census2011_Queries.py
