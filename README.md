# **Home Sales Analysis with PySpark**

## **Project Description**

This project involves analyzing a dataset of home sales using PySpark to answer specific business questions. The analysis includes performing SQL-like queries on a Spark DataFrame, caching data for performance optimization, and working with partitioned parquet files. The results of this analysis are stored in a Jupyter Notebook file named `Home_Sales.ipynb`


## **Dataset**

The dataset used in this analysis is `home_sales_revised.csv`, which contains details of home sales, such as:

* **Bedrooms**
* **Bathrooms**
* **Year Built**
* **Price**
* **Square Footage**
* **View Rating**

## **Key Objectives**

1. Rename the starter file `Home_Sales_starter_code.ipynb` to `Home_Sales.ipynb`.
2. Import necessary PySpark SQL functions.
3. Load `home_sales_revised.csv` into a PySpark DataFrame.
4. Create a temporary table `home_sales`.
5. Answer analytical questions using SparkSQL:
   * **Question 1** : What is the average price for a four-bedroom house sold for each year? (Rounded to 2 decimal places)
   * **Question 2** : What is the average price of a home for each year it was built, with 3 bedrooms and 3 bathrooms? (Rounded to 2 decimal places)
   * **Question 3** : What is the average price of a home for each year it was built, with 3 bedrooms, 3 bathrooms, 2 floors, and >= 2,000 square feet? (Rounded to 2 decimal places)
   * **Question 4** : What is the average price of a home per "view" rating, where the average price is >= $350,000? Record the runtime.
6. Cache the `home_sales` temporary table and verify its caching status.
7. Re-run **Question 4** using the cached table and compare runtimes with the uncached query.
8. Partition the data by the `date_built` field in parquet format and create a temporary table for the parquet data.
9. Run **Question 4** on the partitioned parquet data and compare runtimes with previous methods.
10. Uncache the `home_sales` table and verify.

---

## **Project Structure**

* **Data** :
* `home_sales_revised.csv`: Input dataset.
* **Code** :
* `Home_Sales.ipynb`: Jupyter Notebook containing the complete PySpark analysis.
* **Output** :
* Results from analytical queries.
* Parquet files partitioned by `date_built`.

---

## **Technologies Used**

* Python
* PySpark
* Jupyter Notebook

---

## **How to Run the Project**

1. Install the required dependencies:
   * PySpark
   * Jupyter Notebook/Google Collaborator
2. Open `Home_Sales.ipynb` in a Jupyter Notebook environment.
3. Run the cells sequentially to load the data, create temporary tables, and execute queries.

---

## **Results**

The notebook answers the following business questions:

1. Average price of 4-bedroom houses sold each year.
2. Average price of 3-bedroom, 3-bathroom homes built each year.
3. Average price of 3-bedroom, 3-bathroom homes (2 floors, >= 2,000 sqft) built each year.
4. Average price of homes per "view" rating with an average price >= $350,000, and runtime comparisons.

---

## **Caching and Performance**

* The analysis includes caching the `home_sales` table to optimize query runtimes.
* Comparisons are made between uncached and cached queries, and parquet-partitioned data.

---

## **Repository**

* **Name** : Home_Sales
* **Contents** :
* `Home_Sales.ipynb`: Jupyter Notebook file with the analysis.
* `README.md`: This readme file.

---

## **Instructions for Submission**

1. Download the `Home_Sales.ipynb` file.
2. Upload it, along with `README.md`, to your GitHub repository.
