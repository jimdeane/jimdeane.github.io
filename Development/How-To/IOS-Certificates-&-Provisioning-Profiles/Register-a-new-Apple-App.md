# Register a new Apple App
(Skip these steps if you are only regenerating expired certificates.)<br/>

## 1. Register an App Identifier in the Developer Portal.
Reverse Domain Name syntax suggested to avoid duplicate Identifiers and also a way to to instill trust on the App Store.
Take note of the **App ID Prefix (Team ID)**
https://developer.apple.com/account/resources/identifiers/list

![image.png](/.attachments/image-460ac2e6-4f4b-4f9f-a114-e4152ba4de37.png)<br/>

## 2. Create a new App in the App Store Connect portal.
Click the + button to create a new App.
- Name: Descriptive name for the App.
- Bundle ID: Choose the identifier you created from the dropdown.
- SKU: Just a unique id, generate a new GUID for this.

https://appstoreconnect.apple.com/apps<br/>

## 3. Update MAUI files in Visual Studio
- Edit the MAUI project file (.csproj)
  - ApplicationId = App.BundleId
  - ApplicationGuid = App.SKU
- Update Constants.IosKeychainSecurityGroup with the BundleId
- Entitlements.plist
  - application-identifier = "_{TeamId}_.*"
  - keychain-access-groups = "$(AppIdentifierPrefix)_{BundleId}_"