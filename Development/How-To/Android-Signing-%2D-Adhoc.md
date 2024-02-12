# Create a new KeyStore
(Skip this step if you are re-generating a key).

Use Android Studio to create a new keystore in a safe place. **NB: Not source control.**

![image.png](/.attachments/image-401d30e2-f4f4-430a-8bca-b794eef4c159.png)

Generate a secure password, you have to use the same password for both the key and keystore.
Also store password in the shared keyvault for retrieval later.
You will also have to update any DevOps variables.

Upload the keystore file to the SecureFiles section in Azure Devops.

# Refresh a signing Key

Use Android Studio and select an existing keystore.
Press Next, and either create a new key. You will have to recall the keystore password from keyvault, use the same password for the new key.

Upload the keystore file to the SecureFiles section in Azure Devops.
(You will have to delete the existing one).

