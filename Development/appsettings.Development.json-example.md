Remember to update _{secrets}_ below.
Secret names match secrets stored in KeyVault **kv-malue-shared-westeu**.


```
{
  "ConnectionStrings": {
    "Malue": "Server=tcp:sql-maluepoc-dev-westeu.database.windows.net,1433;Initial Catalog=maluepoc;Persist Security Info=False;User ID=maluepoc;Password={sql-password-dev};MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=False;Connection Timeout=30;"
  },
  "AzureAdB2C": {
    "Instance": "https://maluepocorg.b2clogin.com/",
    "Domain": "maluepocorg.onmicrosoft.com",
    "ClientId": "f4b6178a-752e-4328-abc5-c2f8872292ab",
    "CallbackPath": "/signin-oidc",
    "SignOutCallbackPath": "/signout",
    "SignUpSignInPolicyId": "B2C_1A_GenericSignUpSignInPolicy",
    "ResetPasswordPolicyId": "",
    "EditProfilePolicyId": "",
    "TenantId": "007cd68f-5674-4d6f-8011-a2e58c2f7798"
  },
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft.AspNetCore": "Warning"
    }
  },
  "Feedback": {
    "DevOpsApiSecret": "{PAT-Feedback-Workitems}",
    "WorkItemParentId": "491"
  },
  "AllowedHosts": "*",
  "CustomAppSettings": {
    "SuppressRoutingForAdminOnly": true, // suppresses role checkingn and allows all pages for authoriosed useers
    "SuppressMandatoryFieldChecking": false // 
  },
  "DetailedErrors": true,
  "Environment": "Local",
  "APPLICATIONINSIGHTS_CONNECTION_STRING": "InstrumentationKey=58657e34-6ea6-47b6-8c3a-17f9518da11f;IngestionEndpoint=https://westeurope-5.in.applicationinsights.azure.com/;LiveEndpoint=https://westeurope.livediagnostics.monitor.azure.com/"
}
```
