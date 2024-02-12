 **"Creating a self-signed certificate authority (CA)"**

makecert -r -pe -n "CN=Malue" -ss CA -sr CurrentUser -a sha256 -cy authority -sky signature -sv MalueCA.pvk MalueCA.cer -p $(CertificatePassword)

**"Convert the certificate and key into a PFX file"**
pvk2pfx -pvk MalueCA.pvk -spc MalueCA.cer -pfx malue-win-cert2.pfx -po $(CertificatePassword)