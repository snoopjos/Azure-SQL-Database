# Azure-SQL-Database
Steps to creating a SQL database in Azure portal

## Step 1
- Create resource group and enter database name (this is the database within the SQL server and you can have multiple databases within one server). 
- Create the server, for authentication you can use an Entra user (if you have one), otherwise just create one using SQL authentication credentials.
- Select service tier
    - **DTU** is where compute and storage goes hand in hand, meaning if you scale up compute it also scales up storage. This is not ideal if don't necessarily require more storage as you scale up compute. However it is the cheaper option.
    - **vCore** is more ideal as you can scale storage independitely from the compute.