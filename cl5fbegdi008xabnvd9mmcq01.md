## Fraud, Theft, and Hacks in DeFi Ecosystems and How to Avoid them

# Introduction
We've all been told that blockchain technology is revolutionizing finance by being a more secure and transparent medium of transactions. However, hacks, thefts, and frauds have stained this image in the past and can potentially keep doing so in the future. In fact, the world of DeFi is rife with scams. In this blog, we'll go over why and how such fraudulent activities take place.

# The Blockchain Trilemma
![Scalability.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657435720138/6Q_S6h-t_.png align="left")
The 'Blockchain Trilemma' refers to the notion that blockchains can only hold strong in two of the three following aspects: security, scalability and decentralization. For example, if a blockchain is decentralized and secure, it isn't as scalable as one would want it to be. Because of this issue, one needs to compromise on the aspect they consider the least valuable out of the three.  

# Compromising Decentralization
*(Spoiler alert: NOT a good idea)*

If you must use a centralized medium for decentralized finance, you know the system in inherently flawed. Centralized exchanges like Binance, Gemini, KuCoin and Coinbase make it very easy for their users to trade cryptocurrencies. They are able to achieve this by compromising on decentralization. Though these websites serve their purpose very well, there is always a risk of them getting hacked and losing a ton of money. Let's understand this with the example of the Binance Hack (2019)

### Binance Hack (2019)
![Binance-coin-bnb-logo.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657454622035/xoGVAjoIi.png align="left")
Centralized exchanges keep two types of wallets: hot and cold
- hot wallet:  Hot wallets are used for storing cryptocurrencies which are actively used in trade and thus only there for a short period of time. They are always connected to the internet
- cold wallet: Functionally similar to a cold storage in real life, a cold wallet is used for storing cryptocurrencies for a long period of time. They are offline unless prompted to come online. 


Centralized exchanges store some amount of money in their hot wallet to enable fast and seamless trade. The rest of the volume gets stored in a matrix of cold storages in order to keep it secure. Hot wallets are at a much greater risk than cold wallets as they are easier to hack. Alas, that is exactly what happened in the Binance Hack of 2019. The hackers were able to get access to Binance's hot wallet and stole 40 bitcoins (worth around 40 million USD at that time). This hack is one of the most notable hacks among them all because of the huge amount of money that got stolen and because of the fact that this happened to a well-reputed company.


# Phishing
![sebastiaan-stam-RChZT-JlI9g-unsplash.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1657448507282/EkwnhM9EH.jpg align="left")
The good ol' impostor act. Phishing has been existent for quite a long time now and is one of the oldest ways of scamming on the Internet. This method of stealing funds requires the least amount of effort and can be done by potentially anyone who knows how to use a computer. The scammer pretends to be a famous and/or reputed company or person and gains the user's trust, eventually stealing assets from them. The most notable phishing scam in the world of DeFi was the phishing attack OpenSea, the largest digital marketplace for crypto collectibles and NFTs, which took place in February 2022. Let's understand how the entire fiasco took place.

### Phishing Attack on OpenSea (2022)
Earlier, OpenSea used to run on the 'Wyvern' protocol for management, storage and transfer of NFTs from the user's wallets. In February, they decided to upgrade their [smart contract](https://www.techtarget.com/searchcio/definition/smart-contract). This meant that they would also have to move the listings of tokens to the new contract. Scammers saw a window of opportunity here. They pretended to be representatives from OpenSea and sent mails to the users, asking them to sign a transaction to a partially written smart contract and thus getting their authorization. They then used that authorization to steal the users' NFTs. In other words, they got the users to sign a blank cheque and filled in the details themselves. Over 1.7 million USD worth of NFTs were stolen. Now, OpenSea has migrated to the 'Seaport' Protocol.


# Ponzi Schemes
![imgonline-com-ua-Negative-Rsu6xMtNsi4Pm.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1657454224239/FwYADie05.jpg align="left")
A Ponzi scheme is defined as: a form of fraud in which belief in the success of a non-existent enterprise is fostered by the payment of quick returns to the first investors from money invested by later investors.

I'm sure you've heard people describe DeFi in general as a Ponzi Scheme. Fortunately (or unfortunately, depending on who you ask), that is not the case as DeFi truly is the future of finance and it solves many more problems than it creates. But let's play the Devil's Advocate and for now, focus on how bad actors are ruining the image of cryptocurrencies by running Ponzi Schemes.

### Who Pulled the Rug?
Influencers are infamous for running pump and dump Ponzi Schemes using cryptocurrencies and NFTs. This is very easy to do as some blockchains allow anyone to create new tokens. For example, Ethereum allows people to create their own cryptocurrencies and merely asks them to abide by the ERC-20 token standard. Bad actors misuse this permission. They create a token and keep the majority of the supply to themselves. Then, they generate hype using their massive network and induce FOMO (Fear of Missing Out). That is pretty much all they have to do. They can then just sit back, relax and watch the price of their cryptocurrency go up. When they think it has reached its peak, they withdraw all the tokens they hold, thus shattering the market completely and leave all the investors with a hole in their pockets. This method of pumping a cryptocurrency to a certain extent and then withdrawing all of one's holdings is popularly known as a 'rug pull'. Essentially, anyone with a huge network and strong marketing tactics can perform a rug pull. Here is a video of Simon Zawa, a streamer on Twitch, reacting to a token (SQUID) being rug-pulled: 

%[ https://www.youtube.com/watch?v=CpR2kMxy7O8 ]
*(warning: explicit language, loud volume)*








# Preventive Measures

![6mc05d.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1657456337798/cZMA-DzQ9.jpg align="left")
After reading all this, I'm sure you're wondering how you can keep your assets safe. Well, here are a few good measures that you can undertake:

1. **'Private' keys**: The most trivial one. As the name suggests, your 'private' keys should remain private. NEVER, ever disclose your account's private key to anyone. When developing dApps on testnets like Rinkeby and Goerli, make sure you use a burner account and not your main one. Also, always be careful enough to not push your private keys to your GitHub repository.

2. **Careful what you sign!**: When signing a transaction, make sure it is of the desired website in order to avoid getting phished. Your signature can potentially be used to drain your assets so always keep an eye out.

3. **DEx-es over CEx-es**: Prefer using Decentralized Exchanges over Centralized Exchanges. The best example of a Decentralized Exchange is Uniswap. Governance in Uniswap is done using their token 'UNI' where its holders can create proposals by themselves and can also vote on other holders' proposals. So, Uniswap is a good example of DAOs (Decentralized Autonomous Organizations) as well.

4. **Freeze!** : Use cold wallets for storing assets that you don't generally use. Even though it is still possible to hack them, they are much harder to hack than hot wallets. Hardware wallets are the best examples of cold storage.

5. **I don't even know who you are**: If someone is trying to access sensitive information while claiming to be from a reputed source, make sure you check and recheck their credentials.

# Summary
In this blog we have discussed: 
- how compromising on decentralization can prove to be a bane to both the users and the creators of such protocols and apps. 
- how hackers stole a huge amount of money from Binance by hacking their hot wallet and draining it of 40 bitcoins. 
- how scammers took advantage of OpenSea's smart contract upgrade by phishing users and stealing NFTs worth more than 1.7 million USD, all with the help of an incomplete smart contract and a fake email. 
- Ponzi schemes in the world of DeFi and how influencers use FOMO to persuade people to buy their token, only to rug pull them later on.
- ways in which we can keep our crypto assets protected

## That's a Wrap!
Thank you so much for reading to the end! I really appreciate your time and I hope you found this blog helpful!


