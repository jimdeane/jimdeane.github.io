# Repository

Code is hosted in the github repository **Malue-Ltd/malue-b2c** and has a few folders:
- /devops - yaml files for CI/CD
- /policies - the custom policy xml files
- /templates - the template content referred to in the custom policy files

# DevOps
Each B2C tenant has an app registration called "sp_devops". This is the service principal with the rights to deploy custom policies to the tenant.

## Renewing secrets
The secret for sp_devops is set to expire after 6 months.
To renew, simply navigate to the app registration in the correlating b2c tenant, and click on Certificates & Secrets.
Create a new secret and give it a descriptive name like "devops". Once created the secret will be displayed once only, copy this secret to to appropriate variable group in devops.
