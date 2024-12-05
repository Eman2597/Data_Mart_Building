# Intoduction:
      
By using AdventureWorks2022 Dataset I have built a Sales Data Mart using (SQL Server Integration Services SSIS) SQL Server involves leveraging the capabilities of Integration Services (SSIS) and the Modeling of SQL Server, This Data mart offers several benefits, making them valuable components in the main purpose of data management and analytics within organizations
#Data Source:   
    using AdventureWorks2022 (OLTP)  [Data Source](https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorks2022.bak)   

# Technologies:

  Visual Studio
  
  SQL Server Integration Services (SSIS)
  
  SQL Server Management Studio (SSMS)
  
  Slowly Changing Dimension (SCD)
  
# Project Stages

1- Data Source Selection:
    We began by selecting the AdventureWorks2022 database as our primary data source. This OLTP system serves as the foundation for our data mart.

2- Data Extraction:
    Using SQL Server Integration Services (SSIS), we extracted relevant data from the AdventureWorks2022 database. This extraction process involved identifying essential tables and fields for analysis.

3- Data Cleansing and Preprocessing:
    To ensure data quality and accuracy, we performed data cleansing and preprocessing tasks. This step involved handling missing values, removing duplicates, and transforming data as needed.

4- Star Schema Design:
    The foundation of our data mart is the star schema. We meticulously designed this schema to align with the specific analytical requirements of our project. This schema includes dimension tables describing various attributes and a central fact table containing numerical measures.

5- ETL Development:
    The core of our data integration process is the development of Extract, Transform, Load (ETL) processes. Leveraging SSIS and other ETL tools, we created workflows to extract data, apply transformations, and load it into the star schema.

6- Data Mart Population:
  We populated the data mart with cleansed and transformed data, ensuring that it is readily available for analysis.

 These stages represent the key milestones in our journey to create a Sales Data Mart using SSIS and SQL Server. The resulting star schema empowers my mindset with an efficient view of data access and valuable insights for informed decision-making.
# Project Workflow:
## Star Schema Design:
Data Modeling by creating star schema for the data mart:
![Data Modeling by creating star schema for the data mart: ](https://github.com/Eman2597/Data_Mart_Building/blob/main/Image/Star%20Schema.png)
## SSIS Packages:
I have created six packages to build this data mart

ETL_Dim_Product

ETL_Dim_Customer

ETL_Dim_Territory

ETL_Dim_Date

Fact_Sales_Full_Load 1

Fact_Sales_Increamental_Load

### 1.Product Dimension 
 ![Dimension Product ETL](https://github.com/Eman2597/Data_Mart_Building/blob/main/Image/Dim%20Product_ETL.png)
 ### 2.Customer Dimension
 ![Customer Dimension ETL](https://github.com/Eman2597/Data_Mart_Building/blob/main/Image/Dim%20Customer_ETL.png)
 ### 3.Territory Dimension
 ![Territory Dimension ETL](https://github.com/Eman2597/Data_Mart_Building/blob/main/Image/Dim_Territory_ETL.png)
 ### 4.Date Dimension
 ![Date Dimension ETL](https://github.com/Eman2597/Data_Mart_Building/blob/main/Image/Dim%20Date_ETL.png)
### 5.Fact_Sales_Full_Load
![Fact_Sales_Full_Load](https://github.com/Eman2597/Data_Mart_Building/blob/main/Image/Fact%20Sales_Full%20Load.png)
### 6.Fact_Sales_Increamental_Load
![Fact_Sales_Increamental_Load](https://github.com/Eman2597/Data_Mart_Building/blob/main/Image/Fact%20Sales-Incerment%20Load_Control%20Flow.png)
![](https://github.com/Eman2597/Data_Mart_Building/blob/main/Image/Fact%20Sales-Incerment%20Load.png)
## Result Load
![Load](https://github.com/Eman2597/Data_Mart_Building/blob/main/Image/Full%20Load%20result.png)

