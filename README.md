# Privacy Guide Pirate Chain

<img src="https://github.com/Seko1900/privacy-guide-pirate-chain/blob/main/images/pg-banner.png" alt="Pirate Chain Privacy Guide" title="Pirate Chain Privacy Guide">

An open source privacy guide specifically for the Pirate Chain project and its users.

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-privacy-guide">About The Privacy Guide</a>
    <li>  
      <a href="#why-pirate-chain?">Why Pirate Chain?</a>
      </ul>
    </li>
    <li>
      <a href="#privacy-vs-anonymity-vs-security">Privacy VS Anonymity VS Security</a>
      <ul>
        <li><a href="#what-is-privacy?">What is Privacy?</a></li>
        <li><a href="#what-is-anonymity?">What is Anonymity?</a></li>
        <li><a href="#what-is-security?">What is Security?</a></li>
      </ul>
    </li>
    <li>
      <a href="#wallets">Wallets</a>
      <ul>
        <li><a href="#lite-wallet">Lite Wallet</a></li>
        <li><a href="#full-node-wallet">Full Node Wallet</a></li>
        <li><a href="#paper-wallet">Paper Wallet</a></li>
        <li><a href="#mobile-wallet">Mobile Wallet</a></li>
        <li><a href="#hardware-wallet">Hardware Wallet</a></li>
      </ul>
    <li>
      <a href="#aquiring-arrr">Aquiring ARRR </a>
      <ul>
        <li><a href="#centralized-exchanges">Centralized Exchanges</a></li>
        <li><a href="#decentralized-exchanges">Decentralized Exchanges</a></li>
        <li><a href="#over-the-counter">Over the Counter</a></li>
        <li><a href="#mining">Mining</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#location-of-files-on-different-operating-systems">Location of files on different Operating Systems</a>
    <ul>
      <li><a href="#windows">Windows</a></li>
        <li><a href="#mac">Mac</a></li>
        <li><a href="#linux">Linux</a></li>
        </ul>
    </li>
  </ol>
</details>

<!-- ABOUT THE PRIVACY GUIDE -->
## About The Privacy Guide

This guide aims to help the user understand how to use the Pirate Chain infastrucure to suit their privacy needs. 

<p align="right">(<a href="#privacy-guide-pirate-chain">back to top</a>)</p>



## Why Pirate Chain?

Pirate Chain is a blockchain that uses zero knowledge proofs, by default, to prove and verify encrypted transactions.  This allows for Anonymous peer 2 peer transcations.  

<p align="right">(<a href="#privacy-guide-pirate-chain">back to top</a>)</p>


<!-- Privacy VS Anonymity VS Security -->
## Privacy VS Anonymity VS Security

The use of the word Privacy sometimes gets misunderstood, in the context of this guide, privacy is the combination of Privacy, Anonymity and Security in whatever meets the needs of the user. The analogy of writng a diary can illustrate this.

### What is Privacy?

PRIVACY is the quality or state of being apart from company or observation.

The contents of the diary are private when only you know.

### What is Anonymity?

ANONYMITY is the quality or state of being anonymous.

The contents of the diary can be known, but whom wrote the contents is not known.

### What is Security?

SECURITY is the quality or state of being secure.

The level of difficulty someone would need to overcome to access the contents of the diary.

<p align="right">(<a href=#privacy-guide-pirate-chain>back to top</a>)</p>

<!-- Wallets -->
## Wallets

The term wallet is misguided, typically we think of a wallet as a place where we keep money.  Pirate Chain being a [UTXO](https://medium.com/cryptoapis/utxo-and-account-based-blockchains-d1d3c638524) based blockchain, all ARRR is associated with an address which is are unspent transctions.  A wallet is the access point to the blockchain, it holds your addresses and keys that are necassary to interact with the blockchain.  

Prior to downloading a wallet, there are some important aspects of using a wallet that need to be known, these are primarily for security.  

(VPN and FIREWALL) 

When creating a wallet a seed phrase is generated, that seed phrase is based off of [BIP39](https://www.blockplate.com/blogs/blockplate/list-of-bip39-wallets-mnemonic-seed).  It is extremely important to preserve this seed phrase.  This seed phrase will allow you to restore a wallet from newly installed software.  It also allows you to access addresses that are asociated to the wallet, into other wallets eg.(Full Node, Lite or Mobile wallet).  The seed phrase will not restore any addresses that were not generated by that wallet eg. imported addresses will not be restored.

Each address generated in your wallet will have a Spending Key or also known as a Private Key, this key allows you to spend ARRR.  Backing up your Private Key and keeping it secure is the most important thing to do. [How to Import and Export Private Keys](https://youtu.be/MmVR4QtjrU4).  You can import this key into any Pirate Chain wallet and access your ARRR.  To save all the spending keys in the wallet you can also save your wallet.dat file.

Each address generated in your wallet will have a Viewing Key, this allows you to view the UTXO(ARRR) associated with the address.  The viewing keys can only be imported into the Full node Wallet.  Viewing keys are only for viewing and give no access to the ARRR belonging to that address, these keys are safe to give out, if you have the need to prove ARRR associated with that address. [How to use Viewing Keys](https://youtu.be/IZUyjihAz04)



Pirate Chain has different wallets that you can use to access the blockchain.

### Lite Wallet

The fastest and simplest way to interact with the Pirate Chain blockchain.  The lite wallet accesses a server that has a copy of the blockchain hosted on it.  The lite wallet has some limitation compared to the Full Node wallet (ELABORATE ON DETAILS). The lite wallet offers the lowest level of privacy of all the wallets, using a VPN is suggested to increase the anonymity.  Running on a Linux based Operating System will also increase the security. 

[Download Lite Wallet](https://pirate.black/wallets/desktop-lite/)

[Lite Wallet Tutorial](https://youtu.be/279QzgHU-wk)

### Full Node Wallet

The Full Node Wallet(Treasure Chest) is the most secure and recommended wallet to use, it will occupiy sbout 10GB od disk space. Installing a Full Node included a complete copy of the Pirate Chain blockchain from genesis block up to the current block.  This is done most effieciently through a process called bootstrapping.  Bootstrapping is a method of compressing the blockchain data and allowing the user to download and install the blocks and index.  Running a full node helps to strengthen the network by having multiple instances of the same blockchain available for confirmations.  The Full Node has the option of password protecting the wallet for an added level of security.  You can import viewkeys to the node to view the balances of addresses.  

[Download Full Node Wallet](https://pirate.black/wallets/treasure-chest/)

[Full Node Tutorial](https://youtu.be/qNV_uC2BHyg)

### Paper Wallet

The Paper Wallet is the most secure method of storing your ARRR.  This wallet allows you to generate an address and then you can export the spending key and the view key offline.  You can send your ARRR to this address and the spending key has never been exposed to a internet connection.  The viewkey can be imported to the Full Node wallet to see that your ARRR is at that address. 

[Download Paper Wallet](https://github.com/PirateNetwork/piratepaperwallet/releases/tag/v0.5.0)

[Paper Wallet Tutorial](https://youtu.be/zAIdQNhB6Z4)

### Mobile Wallet

The Mobile Wallet allows for use on Android and IoS(IOS 14.1+) devices with more that 3GB of RAM.  This wallet is the least secure and should be used with a VPN to maximize anonymity.  The covience and flexibilty of the mobile wallet is a nice addition to using a Full Node for on the go use. 

[Download Mobile Wallet](https://pirate.black/wallets/skull-island/)

[Mobile Wallet Tutorial](https://youtu.be/zAIdQNhB6Z4)

### Hardware Wallet

The Pirate Hardware Wallet is the only device that is capable of processing zkSNARKs transactions, required by Pirate Chain (Arrr). Access to the unit is protected with a root-of-trust setup that starts in the boot ROM at power up, through all the boot phases, up to the pirate authenticator application. The small unit is portable, which offers convenience over the 2 PC online/offline split transaction capability in Treasure Chest. On the roadmap is to integrate the user interface with the smart phone Pirate wallets.

[Hardware Wallet](https://www.barrrter.com/ad/details/pirate-chain-hardware-wallet)

<p align="right">(<a href=#privacy-guide-pirate-chain>back to top</a>)</p>

<!-- Aquiring ARRR -->
## Aquiring ARRR 

### Centralized Exchanges

### Decentralized Exchanges

### Over the Counter

### Mining

See the [open issues](https://github.com/github_username/repo_name/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href=#privacy-guide-pirate-chain>back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href=#privacy-guide-pirate-chain>back to top</a>)</p>


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href=#privacy-guide-pirate-chain>back to top</a>)</p>



<!-- CONTACT -->
## Contact




<!-- Location of files on different Operating Systems -->
## Location of files on different Operating Systems

These are the locations of files for the different Operating Sysytems

### Windows

Windows %appdata%\komodo\PIRATE\

### Mac

Mac ~/Library/Application\ Support/pirate/ 

### Linux

Linux ~/.pirate/


<p align="right">(<a href=#privacy-guide-pirate-chain>back to top</a>)</p>
