## How to Get Started in Web3 as a Developer

## Introduction
![Web3](https://miro.medium.com/max/1400/0*gVQXZtBZGvmBHvgQ.png align="center")


If you haven't been living under a rock for the past four years, you've surely come across the terms Web3, blockchain, cryptocurrency and NFTs. If you're reading this here on hashnode, chances are, you are a developer. If you too are looking to break into the world of Web3, you need not look any further! In this blog, we'll go over the basics required to embark on a journey to become a Web3 developer.

*Note: this blog focuses on development on Ethereum using the JavaScript ecosystem.*



##  Fundamentals of Blockchain Technology
![Blockchain Technology](https://preferredbynature.org/sites/default/files/2021-06/iStock-953499010_0.jpg align="center")

### What is the difference between Web2 and Web3?
Ummmm this is kind of an incorrect question. I say this because Web3 is built on top of Web2. It isn't a competitor, it is a technology that leverages the power of Web2 and heavily improves upon it. In Web2, decisions about your data are taken by the companies. In Web3 they are taken by YOU! That's right, power to the people! Web3 aims to solve censorship and fight the centralization of data. To put it in a nutshell, Web3 is decentralized Web2. Slowly but surely, people are realizing the power of Web3 and have made it a priority to explore blockchain technology in order to stay above their rivals. However, at this point of time it is nearly impossible to achieve 100% decentralization and some percentage of centralization remains in the Web3 projects we see today. 

### Terms and Definitions:

- **node**: All computers who participate in the functioning of a blockchain are called nodes. A node receives incoming transactions and stores it. It then confirms with other nodes if they too have received the same data. This data is stored inside blocks. When more than 50% of all the nodes confirm this, the proposed block is added to the blockchain. But, who proposes these blocks? **Miners**.

- **miner**: A miner is a node who proposes new blocks. Miners are required to do complex computational tasks to earn eth rewards. So, all miners are nodes but not all nodes are miners.

- **consensus**: The meaning of the word in English is reaching a general agreement. That is what it means with respect to blockchain too. Reaching consensus in a blockchain means getting at least 51% of the  nodes to agree on the changes that are made to the blockchain.

- **consensus mechanisms**: They are also known as consensus protocols and consensus algorithms. There are different consensus mechanisms like proof-of-work, proof-of-stake, proof-of-burn etc. Consensus mechanisms allow the network to work together and stay secure. Ethereum is currently using proof-of-work but is making the switch to proof-of-stake as it is more energy efficient and thus more environment-friendly too. These mechanisms act as a safety measure to proactively fend off hackers who may try to tamper with the blockchain. Without diving in too deep, let's learn about proof-of-work and proof-of-stake. 


1. proof-of-work: In this mechanism, miners are required to complete a complex mathematical puzzle. Many miners try to mine at the same time. It's a race. The reward for mining, called the block reward, which is currently 2.56 eth, is given to the one who completes it first. Solving this puzzle is called proof-of-work. This is secure because one would need to have control of 51% of the network's nodes in order to commit fraud. They would end up losing more than they would gain.
2. proof-of-stake: it requires one to have skin in the game in order to propose new blocks. The game here is the Ethereum blockchain and skin here is ether. The nodes which stake eth are called validators. A validator is chosen at random to create a new block. This is a secure mechanism because one would need to have over 51% of the total staked eth in the network in order to do fraudulent activity. Also, if you try to do something malicious, your stake is slashed significantly.




- **block**:  ![Block structure](https://ethereum.org/static/85d784391401f89209d3bcc51e0ea677/302a4/tx-block.png align="right")A block is a **container data structure**.  Every block in the Ethereum blockchain contains the following:


1. timestamp: the time that block was mined
2. global/world state: the data which is already a part of the blockchain at a particular time.
3. blockNumber: the length of the blockchain till that block
4. baseFeePerGas: minimum gas fees required for a transaction to be included in the block
5. difficulty: the computational strength to mine the block
6. mixHash: hashing is a mathematic function which takes some input and returns another value of a given length. The result of a particular input will *always* be the same. mixHash is a 256 bit long hashed value and it is unique for each block. Hashes are generated using the combined data of that block and all its predecessor blocks.
7. parentHash: The hash of the previous block. The purpose of including this hash in the block is to be able to make sure that no one is trying to tamper with the blockchain. This value is very easy to identify and verify.
8. transactions: the changes made to the state of the blockchain. This is the data that is needed to be added to the blockchain after verifying the integrity of the block.
9. stateRoot: the entire state of the system: account balances, contract storage, contract code and account nonces are inside.
10. nonce: it stands for number only used once. mixHash is actually calculated using this value as an intermediate value! When both nonce and mixHash are combined, it is used to prove that the block has gone through proof-of-work.


- **blockchain**: It's exactly as it sounds: a chain of blocks. An ordered collection of blocks. The future (and, to some extent, present) of finance. THAT, my friend, is a blockchain.

- **wallet:**  Like a real-life wallet, crypto wallets are apps / digital wallets that allow a user to access and manage their digital currencies. When you create a new account, 
your wallet provider, behind the scenes, generates a key pair: a **public key** and a **private key**. The public key is mathematically derived from the private key. You get a unique **address**, which is a hashed version of the public key. This unique address will be used by you a lot. You can get the public key from the private key, but going the other way round is very difficult, even for a supercomputer. Examples of wallet providers are MetaMask, CoinbaseWallet, HyperLedger etc.

- **dApp**: It stands for decentralized application. Applications which leverage blockchain technology for one or more of the aspects they offer are called dApps.



- **smart contract**: they are pieces of code that run on the blockchain. For Ethereum development, these pieces of code are written in a programming language called Solidity. Smart contracts too have an address whose format is the same as that of a  wallet address.
-  
- **Metaverse**: The virtual world is called the metaverse. This metaverse consists of crypto, NFTs, digital land etc. Anything that you have proof of ownership of on the blockchain but not in real life is said to be a part of the metaverse

### How does a blockchain work?
A blockchain is a network of computers which, as described above, are called nodes. When a node receives a new transaction, it broadcasts it to all the other nodes in the network. This way, the miners in the network also receive the transactions and get to work for making a new block and recording a group of transactions permanently in the blockchain. In order to get ether rewards for mining new blocks, miners must perform complex computational tasks. These tasks involve hashing nonces one by one and finally achieving one which gives a hashed value which is less than that of the previous block. This is called proof-of-work and miners are currently rewarded around 2.56 eth for their hard work. The lower the value of the block, the more becomes the difficulty of making a new block.

*Read more about the fundamentals of blockchain technology here: [A Gentle Introduction to Blockchain Technology](https://bitsonblocks.net/2015/09/09/gentle-introduction-blockchain-technology/)* 

## Programming Experience
![Programmer Programming](https://cdn.mos.cms.futurecdn.net/9QTpESGBXa32D29J77VR3d.jpg align="center")
### "I Have no programming experience, can I still become a Web3 developer?"
Yes, definitely yes! But it requires knowing Web2 tech and so people far more experienced than I have strictly advised against jumping to Web3 tech with zero knowledge of Web2 development. So learn the fundamentals of Web3, see if you actually want to go all in on it and start learning Web2 development. Falling into tutorial hell is very unproductive as you won't realize where you wasted your time and why you can't really do the things you've learnt. In my opinion, learning by doing is simply the best method to learn as it gives you a sense of mastery over the tools you are using. I would recommend everyone reading this to do the same.  Don't worry though! You don't need to have a level 100 mafia boss type mastery over Web2 tech, you can learn as you go!

### "I have some experience in a programming language (which is not JS). Any advantage for me?"
Again, yes! The things that you have learnt in that other programming language will help you quickly grasp JS as there are some concepts which are common to all programming languages. Your logic building is going to be very useful to you as well and you'll soar through all the challenges that will come your way.



## Basic Tech Stack Required for Development
![Tech Stack Web2](https://phantomlandscapes.files.wordpress.com/2021/04/html-css-javascript.jpg align="center")
- HTML: for making the foundation of a webpage 
- CSS: for designing the webpage
- JS: for breathing life into the webpage
- Solidity: for making our smart contract
- Ethers.js: for connecting the frontend of our website to the smart contract
- Git/GitHub: knowing how to use a version management system like git will prove to be very helpful in the long run


**With these tools, you will be able to make a basic dApp.**

*Resources for learning the these tools are mentioned later in this blog*

### For more Advanced Development
The previous six plus
- **React.js**:  React truly makes a webpage functional and adds a plethora of features to Vanilla JS. You can learn this as you go.


- **Next.js**: Built on top of react, it allows you to integrate API routes right into your NextJS code.
- **TailwindCSS/Bootstrap**: These powerful tools make CSS less of a pain in the a$$ and allow you to quickly design websites. Personal preference is TailWindCSS.

*Note: Python can also be used instead of JS (discussed in the following section)*



## Development Environments

Note: Node.js is required for Truffle, HardHat and Brownie. Download Node.js [here](https://nodejs.org/en/download/)  

1. [Truffle Suite:](https://trufflesuite.com/) This is for JavaScript developers. Paired up with Ganache, this development environment helps you to write, test and deploy smart contracts. Ganache is a tool that starts a local blockchain network on the computer. We can deploy and test our contracts on this local network before doing anything on the main-net to see how your contract behaves. Truffle is widely said to be an outdated tool which can't keep up with the demands of a modern developer.

2. [HardHat: ![HardHat](https://hardhat.org/card.png align="center")](https://hardhat.org/)This too is for JS developers. It is faster than Truffle and gives more tools and features to the developers. That is the reason why people are switching over to HardHat. Like Truffle has Ganache for making a local network, HardHat has got Hardhat Network. It has got more documentation and support so it is easier for devs to fix errors

3. [Foundry: ![Foundry](https://www.paradigm.xyz/static/Foundry_Ink_2-1024x516.jpg align="center")](https://github.com/foundry-rs)It is the newest kid on the block. It is blazingly fast and new features are being added literally everyday! Since it is so new, the level of online support is very less and the docs are still under construction. I too am currently learning foundry. Its special feature is that EVERYTHING in this environment is done in solidity. Read the Foundry book [here](https://book.getfoundry.sh/).

*Note: For Python developers, there is a tool called [Brownie. ](https://github.com/eth-brownie/brownie). However, it is recommended for Python devs to switch over to JavaScript simply because of the new libraries that are making life easier for Web3 devs. Eg. web3.js, web3modal.js, ethers.js and the list goes on.



### Resources 

#### For learning HTML and CSS
- freeCodeCamp's [Responsive Web Design](https://www.freecodecamp.org/learn/2022/responsive-web-design/) course
- Udacity's [Intro to HTML and CSS](https://www.udacity.com/course/intro-to-html-and-css--ud001) course
- [This](https://www.codecademy.com/catalog/language/html-css) learning path by codecademy


#### For learning JavaScript
- Scrimba's [Learn JavaScript for Free](https://scrimba.com/learn/learnjavascript) course
- Udemy's [JavaScript Essentials](https://www.udemy.com/course/javascript-essentials/) course


#### For learning Solidity   
- **[CryptoZombies](https://cryptozombies.io/)**: Gamified way to learn Solidity with different learning paths
- **[Solidity Zero to Hero course](https://www.codiesalert.com/courses/free-solidity-course)** by @[Anni Maan](@AnniMaan)
- LearnWeb3DAO freshman track** [basic dapp](https://www.learnweb3.io/tracks/freshman/dapp-tutorial)** + sophomore track advanced solidity parts **[1](https://www.youtube.com/watch?v=Z5P3rKBRmEM)** and **[2](https://www.youtube.com/watch?v=ILY3fIbwjk0)** livestreams on YouTube
- **[pointer.gg](https://www.pointer.gg/tutorials/solid-solidity/a7ec3eff-fc59-481d-bcb2-1224b3e9c0f7)**: They also give you an NFT as a reward for completing this tutorial!
- **[Solidity by example](https://solidity-by-example.org/)**: A collection of solidity programs with multiple comments in between explaining what the code is doing

#### For learning git and GitHub
I would recommend [this video](https://www.youtube.com/watch?v=apGV9Kg7ics) by @[Kunal Kushwaha](@kunalk)

#### For learning ethers.js
follow [this tutorial](https://www.youtube.com/watch?v=yk7nVp5HTCk) by dApp University





## Helpful Websites and their Discord Servers
One of the best parts of web3 is the community. So far, I've only received unconditional support and positivity!
1. [![LearnWeb3DAO](https://i.imgur.com/GyTFKfz.png align="center")](https://www.learnweb3.io/)LearnWeb3DAO's website contains a clear roadmap with four tracks: Freshman, Sophomore, Junior, Senior and are to be done in that order. [Discord link](https://discord.gg/EyYep5DpTR)
2. [![Buildspace](https://cdn.hashnode.com/res/hashnode/image/upload/v1652434213967/Ta6FWmNY8.png align="center")](www.buildspace.so)Buildspace's website contains many tutorial projects which can help you build cool stuff and gain technical skills. [Discord link](https://discord.gg/buildspace)
3. [![Developer DAO](https://www.developerdao.com/social-banner.png align="center")](https://www.developerdao.com/) Developer DAO is paid, unless you apply for a scholarship. To gain access to Developer DAO by paying, you can acquire one of their genesis NFTs on the open market. You can also get one from another DAO member. [Discord Link](https://discord.gg/devdao)
4. [![odyssey-logo.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1652434044281/QuvTnPhhr.jpg align="center")](https://www.odysseydao.com/)Odyssey's website contains many articles and learning paths which can help you gain knowledge about how Web3 works and also advance your skills. [Discord link](https://discord.gg/82Ybt6BCFg)

## Slangs
![Catto Meme](https://www.memecreator.org/static/images/memes/5370944.jpg align="center")
*I think you'll come across these a lot*
- WAGMI: We're all gonna make it. It's a hype chant that is used by two different types of people in the Web3 community. When developers say this, they mean that they're confident of them and their friends landing a high paying job and ensuring a bright future for themselves. When investors say it, chances are that the crypto market is going through a crash and they are trying to assure themselves that they won't end up losing all their life savings.
- NGMI: Not gonna make it. Developers use this when they are demotivated and think of quitting. Investors use it when they realize they'll just HAVE to deal with the fact that they'll go broke.
- wen: very silly misspelling of when. Eg. wen new monké?
- LFG: Let's F#cking Go! Victory chant
- degens: people who spend their days and nights researching crypto and NFTs and don't have a life outside of the metaverse.


## 🥳 Congratulations 🥳
That's a wrap! Now you know what to do in order to become a Web3 developer! Thank you so much for reading this entire blog, I really appreciate it! Thank you for spending your valuable time here and I hope you learnt something new and helpful. If you ever feel like giving up, just remember: WAGMI!! (as developers, of course)


### Special Thanks
@[Eda](@edaa): For writing super-detailed yet super-easy-to-understand blogs. It was  because of her that I got inspired to start blogging. I aim to achieve her level of explaining things in my coming blogs. It'll surely be difficult but I think it is worth a shot!

[@abeltxor](https://twitter.com/abeltxor): for further inspiring me to write valuable and well-researched content.

@[Abbas Khan](@AbbasWeb3) : for being a great mentor and motivating me to write blogs.

@[Vatsal Awadhiya](@thevatsal) : for always being so supportive and enthusiastic about my efforts. Also for suggesting changes in this blog.

My elder sister [Bhumika Saxena](https://twitter.com/bhumika_0311): for guiding me, supporting me and always having my back. Also for proposing changes in this blog.

My friend [Sparsh](https://www.linkedin.com/in/sparsh-kumar-3a7390167/): for taking the time to read this blog and propose changes in it.

















