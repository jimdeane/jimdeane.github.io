# Generating an Apple Certificate

You'll use development certificates to run your app on devices and use app capabilities, and distribution certificates to distribute your app for testing and to upload it to App Store Connect.
https://developer.apple.com/help/account/create-certificates/certificates-overview/
<br/>

## 1. Create a Signing Request
This step will produce a SigningRequest file that will be used to generate the certificate in the Apple Developer Portal.

Follow these steps on a dedicated Mac to create a **private key** in the Mac Keychain:

https://developer.apple.com/help/account/create-certificates/create-a-certificate-signing-request/

Suggest saving the file to a secure OneDrive folder to be retrieved from your development laptop.
**Since this is the private key it needs to be kept safe, suggest deleting after use.**
<br/>

## 2. Create a p12 Certificate

https://medium.com/@gobi.ios.dev/ios-creating-a-distribution-certificate-and-p12-2f4d3b63ea9b

### 2.a Create a Server Certificate (.cer) via the Apple Developer Portal.

- Create a certificate using the SigningRequest file in the Developer Portal
- Download the Certificate (.cer) file 
- Install in the dedicated Mac's Keychain by clicking on login\certificates


For a development certificate you will need to generate an development certificate.
See the different types here: https://developer.apple.com/help/account/reference/certificate-types/

### 2.b Export Client Certificate (.p12)

- Match the name of the of the Certificate you just installed and click Export.
- Choose a secure password and save to the Shared Keyvault as **Apple-DistributionCertificate-Password**
- You will also have to update the DevOps variables where required.
- Download the file and keep in a safe place. This is a .p12 Certificate containing both the private/public key.
- Upload the .p12 to the **Library\Secure Files** section in DevOps, update any yaml/variables where needed.




