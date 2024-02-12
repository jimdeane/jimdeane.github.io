1. View or Set the Azure Active Directory admin for the SQL Server instance on Azure.
2. Log in with the AAD Admin account via SSMS.
3. Run the following scripts against the master db:

```
CREATE LOGIN malue_readonly WITH PASSWORD = 'password';

GO

CREATE USER malue_readonly FOR LOGIN malue_readonly;

GO
```
4. Run the following scripts against the malue db:
```
CREATE USER malue_readonly FOR LOGIN malue_readonly;

GO

EXEC sp_addrolemember 'db_datareader', 'malue_readonly';

GO
```
5. Save the password used in the corresponding KeyVault instance on Azure
See here how to get access to keyvault secrets: https://learn.microsoft.com/en-us/azure/key-vault/general/rbac-guide?tabs=azure-cli
6. Test the new user connection