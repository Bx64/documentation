---
id: import-neo-wallet
title: How to import NEO wallets or accounts from nOS 0.5 or earlier
sidebar_label: Import NEO or nOS 0.5 Wallet
---

1. Create a new master wallet in the latest nOS Client.
2. Click the 👜 Wallet icon.
3. Click on  **Key Management**  , next to  **Portfolio**  :

![|313x54](https://miro.medium.com/max/313/1*BrF5y2Z0IaCjMXPCTXfPgQ.png)

4. Click  **Import Account**  in the top right, next to My Account.
5. Click  **Import Legacy Account.**
6. Select the 0.5 account you wish to import and enter that account’s passphrase, and your new 0.6 wallet’s passphrase.
7. Your wallet is now imported!

## Q: I don't have the "Import Legacy Account" button. What do I do?

**A:** If you have a back-up of your 0.5 `profiles_v1.json` file, you can copy it to one of the following locations, depending on your OS:

* **Windows** :  `%AppData%/nOS/storage`
* **MacOS** :  `~/Library/Application Support/nOS/storage`
* **Ubuntu/Debian Linux:**   `~/.config/nOS/storage`

Restart the client and you should get the option when following the import steps.

## Q: I only have access to my encrypted keys or a different json file. How do I import my wallet?

**A:**

If you already have your wallet's encrypted key, skip to step 3.
1. If you have a json file containing wallet details, open it.
2. You should see your wallets' details in text format, including a field that's called `EncryptedKey` (or something similar). Copy this key without the apostrophes.
3. Go to https://snowypowers.github.io/ansy/. This is an [open-source tool](http://github.com/snowypowers/ansy) that lets you export wallet details and private keys from an encrypted key and passphrase.
4. Enter your encrypted key in the `Private Key` field and your encrypted key's passphrase in the `Password` field. Then click `Convert`.
5. You should see two panels, one with your Address and Public Key, one with your HEX and WIF. Copy the WIF value (the input box below it).
6. In nOS Client 0.6, click "Import Wallet", paste your copied WIF in "Private Key", enter the passphrase of your Client 0.6 wallet (not from the encrypted wallet that you just exported), and click **Import**.
7. Your wallet should now be available in your new nOS Master Wallet!
