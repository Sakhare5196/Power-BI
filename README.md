#Adventure Works case study

Adventure Works must identify its top-selling products per country-region based on total sales amounts from its Sales dataset. The dataset includes varied products sold across different channels and regions. Your task is to help Adventure Works as follows:

1. Apply Group By to the two columns, using Sales Amount as the aggregation,
2. And to identify the top performing products per Category and Country-Region.
  
The objective is to provide clear insights into their highest revenue-generating products per Country, enabling strategic decision-making.

Note:
1. Download and launch the FindTopPerformingProducts Power BI file.
2. Ensure that the data is loaded correctly by downloading the AdventureWorks FactSales.xlsx file and updating the data source path from the ribbon Home > Data Source Settings.

Actions:
1. Extracted the top-performer product information by using GroupBy
   <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/123026fa-a160-4b66-8eab-a7914906b658" />

2. Identified the best-performing product for each Category per Country-Region by using DAX formaula Table.Max( Table.Group([All Rows], "Product", {"Total Sales", each List.Sum([Sales Amount]) } ), "Total Sales")
<img width="1050" height="921" alt="image" src="https://github.com/user-attachments/assets/35649c38-b5f7-4e13-a901-f62dc7946a8f" />


Apllied Steps:
<img width="376" height="480" alt="image" src="https://github.com/user-attachments/assets/88a85c56-8e67-4941-8428-0707e9716dca" />

