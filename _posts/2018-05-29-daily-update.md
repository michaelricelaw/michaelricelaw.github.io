---
layout: post
title:  "Daily Solidity Update - Dual struct mappings, local remixd, modifiers, and more!"
date:   2018-05-29 19:11:00 -0700
categories: solidity dailies
excerpt: In today's edition we talk about about how to look up Solidity struct values, local folders using remixd or remix-ide, Infura, solidity modifiers, and so much more....!
---

## Here’s your daily Solidity update...

...May 29 edition!

### Community updates

Over on StackOverflow, there are a few interesting conversations going on. The first is how to **efficiently look up struct values** [without having to loop](https://stackoverflow.com/questions/50569984/how-to-query-a-struct-by-multiple-attributes-in-solidity). The thing I quite liked about one answer is how to avoid unnecessary copies of structs. I know people say "Solidity is like Javascript," but really it's not in my mind. There's also an [unanswered question on how to deploy a smart contract on a recently constructed Amazon Blockchain Template](https://stackoverflow.com/questions/50578696/how-to-write-applications-on-ethereum-netwrok-deployed-using-the-aws-blockchain) -- I'm super curious about the answer, myself.

A person on Gitter was asking about how to arrange folders on Remix when someone recommended **running Remix locally using remixd or remix-ide**: "you could : use remixd to access local file from remix -ide. or install https://www.npmjs.com/package/remix-ide , run remix-ide in the folder you want to be accessible from remix-ide and browser 127.0.0.1:8080" Thought that was a useful idea.

Someone else on Gitter was **complaining about deploying via Infura**. I haven't tried it myself yet. But here's what he said: "I'm trying to deploy my truffle project to the mainnet using Infura, but ran into several still unsolved (!!!) issues: nonce too low, please check your gas amount etc. and kept loosing money." No response in the community, but now I'm curious too.

There's a brief discussion on Reddit about [function modifiers](https://www.reddit.com/r/solidity/comments/8ku89r/what_are_function_modifiers/). I think **modifiers are great** -- kind of like aspect-oriented programming imho.

### Random bits and recommended reads...
**Token Foundry** wrote [a thoughtful Medium](https://medium.com/@tokenfoundry/a-solidity-implementation-of-the-state-machine-design-pattern-25de8b1dfbc5) on using the state machine pattern for decreasing bugs in your Solidity contracts.

**Cardano** [launched](https://iohk.io/blog/first-cardano-testnet-launches-for-smart-contracts/) late yesterday. Not sure what it is quite yet but figured it was worth noting. "Plutus" might be a new word to add to your vocabulary if this thing goes anywhere.

There's a Medium post seeking to explain Solidity to Java developers, but the author **compares Solidity to Eiffel** because it's a "contract first" language. That can't be quite right is it? [Source](https://blog.infullmobile.com/journey-of-learning-solidity-tips-and-tricks-from-java-developers-perspective-8d429f502c31)

### See you tomorrow

Been a long day so that's all I've got for you for now. Tune in tomorrow for another episode!

Got a comment, concern, or comment? Send it to me via email! [michael@michaelricelaw.com](mailto:michael@michaelricelaw.com)
.
