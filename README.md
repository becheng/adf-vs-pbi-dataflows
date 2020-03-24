# Analysis of ADF vs Power BI dataflows

## Setting up a PBI Dataflow

- [ ] Created a custom workspace in PBI Service.
- [ ] Set up a new sample datasource or connect to an existing one.  In my case, I spun up an Azure SQL Database and use the sample AdventureWorks database. 
- [ ] In PBI Service, used **Get Data** to connect to the my datasource and selected a few sample tables.
- [ ] Transformed the data using the Power query editor, e.g. 
    - [ ] Merged queries
    - [ ] Added/Removed/Renamed Columns
    - [ ] Disabled Load of Tables
    - [ ] Aggregated data
- [ ] Perform an on-demand refresh
- [ ] Refresh based on a schedule

## Configure PBI Workspace to access Azure Data Lake Storage (ADLS)
Reference: https://docs.microsoft.com/en-ca/power-bi/service-dataflows-connect-azure-data-lake-storage-gen2#prepare-your-azure-data-lake-storage-gen2-for-power-bi

Unfortunatley I could not preform this task as I only have access to my corporate PBI tenant, which I'm not an administastor on.  One of the requirements is that ADLS account must be created in the same AAD tenant as your Power BI tenant.

