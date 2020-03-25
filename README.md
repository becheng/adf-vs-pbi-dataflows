# ADF vs Power BI Dataflows

## Setting up a PBI Dataflow

- [ ] Created a custom workspace in **PBI Service**.
- [ ] Created a sample datasource - in my case, I spun up an Azure SQL Database and used the sample AdventureWorks database. 
- [ ] In PBI Service, used **Get Data** to connect to the my datasource and selected a few sample tables.
- [ ] Transformed the data using the Power Query Editor. 
    - [ ] Merged queries
    - [ ] Added/Removed/Renamed Columns
    - [ ] Disabled Load of Tables
    - [ ] Aggregated data
- [ ] Performed an on-demand refresh
- [ ] Refreshed based on a schedule
- [ ] Used **Get Data** from **PBI Desktop** to connect this dataflow from the customer workspace to product reports.

## Configure PBI Workspace to access Azure Data Lake Storage (ADLS)
Reference: https://docs.microsoft.com/en-ca/power-bi/service-dataflows-connect-azure-data-lake-storage-gen2#prepare-your-azure-data-lake-storage-gen2-for-power-bi

Unfortunatley I could not preform this task as I only have access to my corporate PBI tenant, which I'm not an administastor on.  One of the requirements is that ADLS account must be created in the same AAD tenant as your Power BI tenant.

## Setting up a ADF 
