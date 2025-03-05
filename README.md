# CSRInspector

## ℹ️ About
**CSRInspector** is a Windows GUI application designed to validate YubiKey PIV attestation. It allows PKI administrators to verify (attest) the authenticity of a YubiKey by checking its certificate chain and public key associations. The application requires three input files: 

- A **Certificate Signing Request (CSR)**
- An **Attestation Certificate** (from the YubiKey)
- The Yubico **Intermediate CA Certificate** (from the YubiKey F9 slot).

Based on these inputs, **CSRInspector** performs certificate chain validation to ensure the attestation certificate is correctly issued and trusted. It also verifies that the public key in the attestation certificate matches the one in the CSR. If all checks pass, the app confirms successful attestation and displays _detailed_ metadata about the YubiKey, including its firmware version, form factor, and security policies.

🙏🏻 A big 'thank you' to Oscar Virot (@virot] for showing what's possible!

![](/images/CSRInspector.gif)


## ⚠️ Disclaimer
This application is made available on an "as-is" basis, without any warranties or representations, whether express, implied, or statutory, including but not limited to implied warranties of merchantability, fitness for a particular purpose, or non-infringement.

## 💾 Setup intructions
_To install CSRInspector_:

1. Download the MSI here
2. Double-click the MSI package to begin installation
3. Follow on-screen instructions to complete installation.

## 📖 Usage
_To use CSRInspector_:

1. Double-click the ```CSRInspector``` desktop shortcut to run the app
2. Select the requisite input files (CSR, attestation certificate and intermediate certificate)<sup>1</sup>
3. Click the **Perform attestation checks** button
4. If attestation is successful, click **Details** to review attested YubiKey details
5. Issue or reject the CSR (out of scope).

<sup>1</sup> Yubico CA certficate is embedded within the application and is not a required input.
