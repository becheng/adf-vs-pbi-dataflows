# ADF vs Power BI Dataflows

## Setting up a PBI Dataflow

- [ ] Create a custom workspace in **PBI Service**.
- [ ] Create a sample datasource - in my case, I spun up an Azure SQL Database and used the sample AdventureWorks database. 
- [ ] In PBI Service, use **Get Data** to connect to  my datasource and selected a few sample tables.
- [ ] Transform the data using the Power Query Editor. 
    - [ ] Merged queries
    - [ ] Added/Removed/Renamed Columns
    - [ ] Disabled Load of Tables
    - [ ] Aggregated data
- [ ] Perform an on-demand refresh
- [ ] Refresh based on a schedule
- [ ] Use **Get Data** from **PBI Desktop** to connect this dataflow from the customer workspace to product reports.

### Configure PBI Workspace to access Azure Data Lake Storage (ADLS)
Reference: https://docs.microsoft.com/en-ca/power-bi/service-dataflows-connect-azure-data-lake-storage-gen2#prepare-your-azure-data-lake-storage-gen2-for-power-bi

Unfortunatley I could not preform this task as I only have access to my corporate PBI tenant, which I'm not an administastor on.  One of the requirements is that ADLS account must be created in the same AAD tenant as your Power BI tenant.

## Setting up an ADF Dataflow
- [ ] Spin up a new ADF instance.
- [ ] Create a Azure Storage with a blob container and uploaded a new blob, eg. test.csv.  This will be the datasink for the ADF data flow.
- [ ] Create 2 separate datasets within in the ADF using the same Azure Sql db as above, one for Customer and one for the CustomerAddress table.
- [ ] Create a new Wraggling Data Flow in the ADF with the 2 datasetes as the source and the blob storage test.csv as the datasink.
- [ ] Transformed the data using the Power Query Editor. 
    - [ ] Merged queries
    - [ ] Added/Removed/Renamed Columns
    - [ ] Disabled Load of Tables
    - [ ] Aggregated data
- [ ] Run the dataflow

