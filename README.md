# CSRInspector

## ℹ️ About
**CSRInspector** is a Windows GUI application designed to validate YubiKey PIV attestation. It allows PKI administrators to verify (attest) the authenticity of a YubiKey by checking its certificate chain and public key associations. The application requires three input files: 

- A **Certificate Signing Request (CSR)**
- An **Attestation Certificate** (from the YubiKey)
- The Yubico **Intermediate CA Certificate** (from the YubiKey F9 slot).

Based on these inputs, **CSRInspector** performs certificate chain validation to ensure the attestation certificate is correctly issued and trusted. It also verifies that the public key in the attestation certificate matches the one in the CSR. If all checks pass, the app confirms successful attestation and displays _detailed_ metadata about the YubiKey, including its firmware version, form factor, and security policies.

![](/images/CSRInspector.gif)

🙇🏻‍♂️ A big 'thank you' to Oscar Virot (@virot) for showing what's possible!

## ⚠️ Disclaimer
This application is made available on an "as-is" basis, without any warranties or representations, whether express, implied, or statutory, including but not limited to implied warranties of merchantability, fitness for a particular purpose, or non-infringement.

## 💾 Setup intructions
_To install CSRInspector_:

1. Download the MSI [here](https://github.com/JMarkstrom/CSRInspector/releases/download/0.0.1/CSRInspector.msi)
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

## 🥷🏻 Contributing
You can help by getting involved in the project, _or_ by donating (any amount!).   
Donations will support costs such as domain registration and code signing (planned).

[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/donate/?business=RXAPDEYENCPXS&no_recurring=1&item_name=Help+cover+costs+of+the+SWJM+blog+and+app+code+signing%2C+supporting+a+more+secure+future+for+all.&currency_code=USD)

## ™️ Trademark notice
YubiKey is a trademark of Yubico. This project is independent of and is not affiliated with, endorsed by, or sponsored by Yubico.

## ⚖️ License
This software is proprietary. Copyright (c) 2026 swjm.blog. All rights reserved. See [LICENSE](LICENSE) for details.
