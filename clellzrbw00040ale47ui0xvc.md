# The Future of Software Publishing

## Introduction

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1677350777579/6bb31633-71fc-4fbd-9466-bceabe4ea002.jpeg align="center")

Greetings everyone! I'm back after a very (very) long time! I know that most of the ones reading this are web/game developers, so I've gotta ask you: once you publish your software, how sure are you that it will always be there? How sure are you that the servers on which you published will never go down? If you're publishing for free, what will you do once they make their service paid as Heroku did? Are you happy paying out a 30% commission to whichever app store you deploy your app/game to?

Stumped you, didn't I? Well, there is a solution for the above problems and it's called **Valist**. Today I'm gonna be giving you all an overview of what Valist is and why you should use it.

## What is Valist?

Valist is a web3-native way of publishing your software. I know many of you cringe instantly when the term "web3" is mentioned because of all the scams and useless projects associated with it. Valist, however, is one of the rare pieces of gold hidden under the landfill. In an ideal world, you wouldn't even know something was going on in the blockchain when using Valist and the team is working towards such a dev experience.

Web3 native here means that there's a high degree of decentralization so that you as a developer do not have to rely on and trust any single party to take care of your deployment. You own your software and no one can take that away from you. You can monetize your software seamlessly and you won't have to pay the exorbitantly high fees that you pay when publishing using other app stores.

As Valist's docs read, it is like an App Store / Play Store / Steam but for web3. If you really wanted to, you could host Valist by yourself and all you would need is a Polygon RPC node, an IPFS node and an endpoint to Valist's subgraph. [Valist.io](https://valist.io) is just a version that is hosted by the Valist team. You can find their GitHub repos [here](https://github.com/valist-io).

## A Brief History of Valist

%[https://www.youtube.com/watch?v=7ak6PQPDBkk] 

Valist was started by [Alec Wantoch](https://twitter.com/alecw) and [Zachary Pelkey](https://twitter.com/0xPelkey) as a hackathon project. They had identified that even though there was a lot of focus on decentralization in web3, it was still quite centralized at the distribution layer. For example, let's say you want to buy an NFT using your mobile. Well and good. That will require you to have a wallet in your phone, like MetaMask. If one day out of the blue, Google Play Store / Apple App Store decided to remove it from their stores without any prior information or warning, there is nothing that you, as a user, can do since they are completely entitled to add/remove apps as they wish. Recently, Coinbase got into a feud with Apple for blocking their wallet's NFT trading feature. Apple wanted 30% of the gas fees on every NFT sent and Coinbase refused to comply. This is clearly a problem that needed to be solved.

Alec and Zach also realized that trusting a single party for your software can lead to disastrous results and they explained their analogy using the precedent of the SolarWinds hack. You can read more about the hack [here](https://www.techtarget.com/whatis/feature/SolarWinds-hack-explained-Everything-you-need-to-know).

In its initial days, Valist was supposed to be a decentralized version of GitHub. But you are probably already familiar with how quickly startups have to pivot and alter their vision. The startup space is a very volatile space indeed. So, the team then pivoted to become a decentralized version of Vercel. After some time they pivoted again and now they are mainly focusing on games and apps and present Valist as a decentralized version of Play Store / Steam / App Store. As I write, the team is building in silence and is about to drop a whole lot of updates in the coming few months.

## How it Works

### The Four Pillars of Valist

Valist has 4 technologies at its foundation layer - Polygon, IPFS, Filecoin and The Graph. I'll give you a one-line explanation for all 4:

1. IPFS (Inter-Planetary File System): It is a decentralized, peer-to-peer version of HTTP and it works on content-based addressing instead of location-based addressing. You can read more about it here.
    
2. Filecoin: It is a blockchain that guarantees data permanence on IPFS with the help of storage deals. Read more about it [here](https://docs.filecoin.io/).
    
3. Polygon: It is a Layer-2 blockchain which uses Ethereum as a security layer and makes transactions faster and cheaper. You can read more about it [here](https://polygon.technology/).
    
4. The Graph: It is used for querying events emitted by Valist's smart contracts since it is very impractical to store everything inside the contracts. Read more about it [here](https://thegraph.com/en/).
    

### How These Pillars Combine

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1677347847753/9b05437e-8ff6-451f-b2ea-f938bc91c7e0.png align="center")

When you first create an account on Valist, your info, which includes your name, a username of your choice, a website and a description, is stored on-chain.

Storing data in smart contracts is an expensive task. Thus, it is quite illogical to store large amounts of data there. We should only store what is needed. So we shouldn't upload built software on-chain. Therefore, when you want to upload a game or a website or any piece of software for that matter, Valist uses:

* IPFS to store your files, the release info ie. the software version and the build info, ie. compatible platforms,
    
* Filecoin to guarantee their permanence
    
* Polygon to emit an event that contains info about the deployer, the build info of the software they have deployed and the Content Identifier (CID) of the actual files which are stored on IPFS. So the smart contracts are just registry contracts
    
* The Graph for querying all the events and linking a user account with the software that they have deployed. along with the compatible platforms and the software version.
    

When a user wants to download some software, Valist automatically detects their platform (Android, iOS, Web, Windows, Linux) and serves them the respective build.

NFTs are used as software licenses and a developer can price their software as they wish to and token gate access to it.

Whenever you perform an action that happens on-chain like editing or publishing a new version of your software, it goes as a transaction on the Polygon chain. However, Valist uses meta-transactions (thanks to OpenZeppelin) throughout, which means you won't have to pay any gas fees, you'll just have to sign a message with your wallet!

*Note: I'll be writing a blog about how you can deploy to Valist soon. It will also contain a more detailed explanation of meta-transactions.*

## Vibes at Valist

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1677342873228/ec7b7db9-85fe-4f40-bb6d-05e5034af5c2.jpeg align="center")

I've been a part of the Valist Discord since July 2022 and it is without question a part of my top 3 most-chill-and-helpful servers. I have been on several community calls and also private calls with Alec and [Vanshika Rana](https://twitter.com/aahiknsv) (their lead DevRel engineer). Everyone is helpful and eager to support. In fact, even what you're reading right now involves some role of both Alec and Vanshika lol. They've helped me out in my dev journey even in the problems which weren't pertaining to Valist.

My favourite channel in their server is the showcase channel where devs can post what they've built. The community is very supportive and provides both praise and constructive criticism.

We often have community calls where we get some alpha from the founders, play games like Skribble and catch up with each others' lives. Overall it is a very friendly and chill experience 💜

## Why Should YOU 🫵 Use Valist?

If you are a developer, there are multiple reasons why you should switch to Valist:

1. It is completely **decentralized**, which implies that no one (not even the Valist devs themselves) can mess with your software once you have deployed it. Even if there was an apocalypse, you could essentially host your own instance of Valist and your software would show up there. Not sure if there are gonna be a lot of people using it in a post-apocalyptic world though lol
    
2. **Software License NFTs** easily allow you to set a price for your software and token-gate it. This helps in battling software piracy as only someone with cryptographic proof of owning your software's NFT can use it.
    
3. Both the **DX and the UX** are very good. It is very easy for a developer to deploy their game/binary/package/static website to Valist. It is also a seamless experience for the user to buy or access published projects. If you are publishing a static site, just use Valist's GitHub action which tracks your repo and **publishes a new website every time you make a push to the main branch**. Isn't that amazing!
    
4. **The fee charged to the dev is minimal.** There is a 2.5% public-good funding fee, which will help accelerate the onboarding of more projects on Valist and a 2.5% protocol fee. So, a total of just 5% compared to ~30% in other stores.
    

So, the correct question is actually why should you NOT publish to Valist and you can let me know when you find a valid answer 😆

## Concluding Thoughts

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1677342983524/b6b4b232-7757-4622-be10-dd87c60de749.jpeg align="center")

### Which protocols/organizations can (and should) partner

* thirdweb is making an effort to push web3 games to new heights. If they partnered with Valist, it will help them go full throttle on it and benefit both of them greatly
    
* GodWoken is a layer-2 blockchain that is built on top of the Nervos network. Their focus is web3 gaming as well and I'm very easily able to see a potential partnership forming between the two. As far as I'm aware, they're already in touch with each other.
    
* Akash network should be a helpful protocol for providing Valist decentralized infrastructure
    
* HyperPlay is a web3-focused game launcher. Another good potential partner that I would love see come to life.
    
* Biconomy helps in providing wallet-less logins and meta transactions. Although Valist already has the aforementioned features, I think Biconomy might be able to provide a better experience.
    

### Some things that can be improved

I've been a long-time user of Valist and so I know that they are actively trying to combat an infrastructure problem. Their IPFS pinning providers have had some issues at the most crucial moments and so team Valist is figuring out a viable solution.

Even though the UX and DX are already pretty good, they can definitely be improved to deliver a more impressive and impactful experience. This is vital for onboarding devs and users alike.

We need more calls!! We need some community events to increase engagement, connect with more people and turn connections into friendships!

I wrote a thread about what my 30-60-90 day plan would be if I joined Valist as a DevRel:

%[https://twitter.com/awesamarth_/status/1628378786445291522] 

## Thank You!

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1677349880366/103328ea-5bd4-4218-a4d7-929e52741ba8.png align="center")

Thank you so much for reading this blog to the end! I really hope you enjoyed reading and learnt something new and useful! In the (very) near future, I'm gonna be writing a blog about how you can deploy your static site to Valist. In that blog, I'll also explain meta transactions better and take a deeper dive into how Valist works. Stay tuned and once again, thanks a lot for reading. See you in the next one, ciao 👋