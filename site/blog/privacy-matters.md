---
_archived: false
_draft: false
featured: false
published-date-month: "July 2021"
name: "Privacy matters"
published-date-2: "08"
read-time-in-min: "8 min."
post-summary: "Tired of public ledgers and front-running? - Sienna fixes this!"
thumbnail-image:
  url: "https://uploads-ssl.webflow.com/60621456954600aa473c3cd0/60dd90cc27489bd0f2ce5acf_Privacy%20matters%20Blog%20Thump.jpg"
  alt: ""
main-image:
  url: "https://uploads-ssl.webflow.com/60621456954600aa473c3cd0/60dd90c54bf78862a7580ad8_Privacy%20matters%20Blog.jpg"
  alt: ""
slug: "privacy-matters"
updated-on: "2022-01-10T10:02:16.296Z"
created-on: "2021-07-08T08:03:55.481Z"
published-on: "2022-01-10T10:02:16.296Z"
tags: "blog"
layout: "single-blog.html"
---

#### 1\. Background

Privacy is a fundamental human right - or it should be. It is a basic individual right to choose whom to share with - not just information, but other important aspects of life such as financial transactions.

But here a problem arises - while cash has relevant anonymous uses - larger transactions should not be anonymous because no system should enable money-laundering or the funding of bad actors. This is especially relevant at a time when the de facto opinion of policy-makers has transmuted into a surveillance economy, with market actors required to police and report with severe penalties for failures. Whether we like it or not.

So, privacy matters. It is a mechanism for individuals and institutions to decide to control their data - sometimes transactionally, at other times to prove or disclose information or financial actions by choosing to share that data with relevant and selected Third Parties.

However,  in a decentralized dis-intermediated DeFi world, where Third Parties are rapidly becoming irrelevant, things are very different - Nevertheless changing laws will almost certainly catch loopholes and clever work-arounds so in this document we will look at the core aspects of this rapid change and how Sienna fixes this.

‍

‍

#### 2\. What privacy is about

The fight for privacy goes back a very long way; through most of modern history some form of encryption has been used to protect information from prying eyes.

Sienna Network was founded from the core belief that privacy should also apply in financial transactions. Most of the current cryptocurrency protocols, coins and assets as well as institutions such as exchanges suffer from the lack of privacy that allows others to see what users are doing and arbitrage on those transactions with front-running. This is unwanted by the user and isn't viable in the long-term, so Sienna Network has built a way to fix it.  
  
The debate over anonymity vs privacy can be left to others - here we will focus on why privacy matters and why it should apply in the adoption of blockchain as bearers of value. Many argue that anonymity should be preferred over privacy. Legislation in aspects of personal data PII such as the EU’s GDPR makes anonymity easier to choose than privacy - as the data minimization principle makes storing any PII data, even encrypted data, problematic and due to the data minimization principle not possible on chain.

Several attempts at replicating cash in crypto exist already, but will serve a different use case where the maximum transaction size will, most likely, be regulated to be only for smaller transactions. This isn’t in opposition to the arguments in this note about privacy - it’s just a very niche use case for low value transactions.

‍

‍

#### 3\. Why Privacy matters

Privacy really does matter and as mentioned above anonymity as in crypto cash isn’t the full answer. If a crypto user sends a beneficiary an amount of an Ethereum-based coin such as US dollars, both wallets are consequently linked via that transaction. This seems like a basic and fair exchange, but it also means that the beneficiary can now see the complete transactional history of that person’s wallet. This is patently an infringement of privacy and needs to be fixed.

Now replace beneficiary with an exchange (which is a misnomer as exchanges are now also providers of access to sophisticated financial products such as NFTs and derivatives and should be called marketplaces). So now the exchange can see the entire transaction history. And by extrapolation that of your friends and your friends’ friends - not very comfortable, right?

The problem began when public ledger blockchains were built at a time where the trust partly came from the public ledger, but with recent innovations in programmable privacy and other proof methods this is no longer necessary.

In addition to the unwanted consequences of a public ledger that is also being misused for front-running of the market, which can cost users significant sums, these legacy blockchains were slow and are now expensive in transaction (aka GAS) fees.

‍

‍

#### 4\. Sienna Network and Privacy

With Sienna Network transactions are private. Which means that the user - and no intermediary - decides if any of the data exchanged should be shared with anybody else. By default, and using strong encryption to protect the data. To share data users need to generate a viewing key, which allows them to decrypt the contents of the data they’ve sent to contracts on Secret Network. Only the user can decide if they want to share this key and their viewing key only corresponds to their own transactions and cannot be used to monitor a Third Party’s wallet transactions (as can be easily done on Ethereum).

Sienna Network is built on technology that permits so-called Programmable Privacy with Secret Network’s protocol and has found a way to turn legacy public smart contracts into Secret Contracts, which allow private interactions where Third  Parties cannot monitor what’s going on. This is because the data remains inside TEEs - Trusted Execution Environments; not even the node operators of the underlying network.

What does it mean for a user? On public ledger chains where anyone with a wallet address could see others’ entire transaction history and that of their friends, with Sienna’s token and via the SiennaSwap the wrapped ‘secret’ tokens such as secretETH the transaction history cannot be looked up and seen. This fixes several core issues including the aforesaid blight of front-running.

The gas to fund transactions on Secret Network is paid in SCRT - the Secret Network native token, which, unlike the underlying network, isn't itself private. To use Sienna Network, users need to acquire some SCRT from a decentralized or centralized exchange and the important aspect here is that the interaction is completely encrypted.

The beauty of the encrypted environment Sienna utilises from Secret Network is that data is concealed from the nodes in the network where consensus and trust is generated via proof-of-stake.The output of the computation can be trusted and verified without revealing the data itself.

Herein lies Sienna’s true innovation. It works by allowing the validator to receive data from a user (sending a transaction) encrypted - then decrypt this data only inside the TEE - perform the relevant computations - and output the result encrypted.

This output is then proposed in a block and requires two-thirds of validators to reach consensus about the encrypted output (and state), which is then committed onchain and can therefore  be trusted.

Notice that the code of the secret contract making Sienna functionality possible isn’t itself encrypted - this is needed to make sure it is possible to see what is  being done - and in Sienna Network’s case to allow a Third Party (CertiK) to audit the code before it was published on-chain. Also the code is open-sourced under the GNU public license.

‍

‍

#### 5\. Conclusions

By separating the consensus from the compute layer and by introducing an encrypted execution environment where input is only viewable inside the TEE, the output can be validated and trusted without revealing the original data.

Consequently, Sienna Network building on the Secret Network has achieved privacy in the interactions with contracts - for transactions user to user, and user to SiennaSwap and so on. Non-public tokens can be mirrored to their privacy-preserving equivalents via the bridges - linked already to Ethereum,Binance Smart Chain and others.

A user can, using a viewing key, view the data and share the view key that only works in combination with that user's wallet with a Third Party. But it is not possible to see a wallet's transaction history with only the wallet address (as it is on Ethereum), making Sienna Network fully privacy-preserving while the user can choose to share the transaction log if relevant.

Sienna Network’s privacy-preserving Token and Swap with attractive staking rewards for liquidity pairs of previously non-private tokens fixes the core issues of the legacy chains while making it possible to remain compliant for private and corporate users.

That’s why we think Sienna has fixed it - we hope users and potential users agree.

‍

  

#### 6\. Further reading

Secret network  
[https://scrt.network/](https://scrt.network/)

Transaction explorer (requires a viewing key)  
[https://btn.group/secret\_network/transactions](https://btn.group/secret_network/transactions)

Secret contracts for developers  
[Secret Contract Devs](https://build.scrt.network/dev/developers.html)
