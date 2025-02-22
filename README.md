# CSRInspector

## ℹ️ About
**CSRInspector** is a Windows GUI application designed to validate YubiKey PIV attestation. It allows PKI administrators to verify (attest) the authenticity of a YubiKey by checking its certificate chain and public key associations. The application requires three input files: 

- A **Certificate Signing Request (CSR)**
- An **Attestation Certificate** (from the YubiKey)
- The Yubico **Intermediate CA Certificate** (from the YubiKey F9 slot).

Based on these inputs, **CSRInspector** performs certificate chain validation to ensure the attestation certificate is correctly issued and trusted. It also verifies that the public key in the attestation certificate matches the one in the CSR. If all checks pass, the app confirms successful attestation and displays _detailed_ metadata about the YubiKey, including its firmware version, form factor, and security policies.

![](/images/CSRInspector.gif)

## ⚠️ Disclaimer
This application is provided "as-is" without any warranty of any kind, either expressed or implied.

## 💾 Setup intructions
N/A

## 📖 Usage
To attest a Certificate Signing Request (CSR), simply point the app to the requisite input files.
