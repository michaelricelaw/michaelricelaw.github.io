---
layout: post
title:  "Daily Solidity Update - PHP-based ERC20 token transfers, multi-sigs, Medium posts, the Berlin Council, and more!"
date:   2018-05-30 18:49:00 -0700
categories: solidity dailies
excerpt: Happy hump day developers! In today's edition, we've got PHP ERC20 transfers, multisig librariers, msg global variables, and the Council of Berlin.
---

Heya Developers!

Happy Wednesday. Just a few days until we can get to our side projects this weekend... how are you going going to decentralize?

## Solidity community updates

There's a nice question and answer on **how to make ERC20 token transfer in PHP** [on Stackoverflow](https://stackoverflow.com/questions/50600515/transfer-erc20-token-from-one-account-to-another-using-php). Apparently ~~someone~~ Furqan Siddiqui was kind enough to write a PHP library for it ([erc20-php](https://github.com/furqansiddiqui/erc20-php)). Love this community.  

On Github, dsys got a lot of love for the new **solidity library for verifying Ethereum message multi-signatures** ([dsys/solidity-sigutils](https://github.com/dsys/solidity-sigutils).)

Lots of good new stuff on Medium today. Here are just a couple: Doug Crescenzi [wrote](https://blog.upstate.agency/what-you-need-to-know-about-msg-global-variables-in-solidity-566f1e83cc69) an **in depth post on the msg object** with some surprising details you might have missed if all you did was copy and paste from some tutorials (e.g., when's the last time you used msg.sig, the "first four bytes of the calldata for a function that specifies the function to be called"?). Christian Reitwiessner ([@chriseth](https://twitter.com/ethchris)) [writes a dense but short post](https://medium.com/@chris_77367/explaining-unexpected-reverts-starting-with-solidity-0-4-22-3ada6e82308c) **explaining unexpected reverts starting with Solidity 0.4.22** -- especially useful for those implementing the ERC20 interface.

On Twitter Murilo Costa [says](https://twitter.com/murilobtc/status/1001919144244203520), "Can’t wait to see all the javascript/ #Ethereum #solidity programmers writing c++ $EOS smart contracts. This is going a 'out of bounds' festival." Seriously. And [if you're in Berlin](https://twitter.com/ethchris/status/1001866541602918401) there's **a meetup on the upcoming solidity 0.5.0 features**. Wish I had enough points to fly out.

The Council of Berlin [agenda](https://ethereum-magicians.org/t/wiki-proposed-agenda-for-the-council-of-berlin-set-for-july-14-15/377) is taking shape (or is it the [Berlin Council](https://ethereum-magicians.org/t/should-we-be-calling-it-the-berlin-council/323)?). Seems like a nice time to be in Germany....
