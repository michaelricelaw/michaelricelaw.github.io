---
layout: post
title:  "Daily Smart Contract Update - Coinbase becomes a broker dealer and diving into some bytecode"
date:   2018-07-17 16:50:00 -0700
categories: solidity dailies
excerpt: Let's explore an interesting, day to day Solidity design pattern and talk about Coinbase as a broker dealer under the 1934 Exchange Act.
---

Let's explore an interesting, day to day Solidity design pattern and talk about Coinbase as a broker dealer under the 1934 Exchange Act.

## Solidity Buidl Updates

Interesting discussion on the Gitter solidity channel today (started by dwardu) to recap here.  In Solidity, create a Point structure to hold two uints of x and y. Now with the statement ```Point memory a = Point(1, 2);``` we know we'll allocate memory for a new Point struct and store it in variable a. Also, if we simply declare ```Point memory b``` it allocates a new Point struct with zeroed out values, which I find confusing since, in my experiences with other languages, b would be null.

Thus, it's logical to conclude that the following code would waste gas because it would start with a zeroed out initialization and then make the assignment:

```solidity
Point memory b;
b = Point(3, 4);
```

Before you draw that conclusion, however, it turns out both contracts in the following code compile to the exact same EVM bytecode:

![Gitter post]({{ "/assets/imgs/2018-07-17-gitter-screen-shot.png" | absolute_url }})

It's a small point, but the kind of day to day, line by line issue that might nag you when you're out there coding.

## Legl Notes

Remember when Coinbase bought Keystone Capital, Venovate Marketplace, and Digital Wealth? No? Well irregardless, it may be paying off for them. Yesterday's [Bloomberg headline news](https://www.bloomberg.com/news/articles/2018-07-16/coinbase-says-it-has-green-light-to-list-coins-deemed-securities) was leads to the conclusion that the SEC's recent approval of the purchase "provides Coinbase licenses to operate as a broker dealer, an alternative trading system and a registered investment adviser . . . [a]lternative trading systems operate outside traditional public stock exchanges.

That's cool but the broker/dealer business is **very highly regulated** all on its own -- maybe the most highly regulated business in America.

BTW, a **reverse ICO** is when a "traditional business take steps to venture into the decentralized realm of the digital currency world." [Investopedia](https://www.investopedia.com/tech/what-reverse-ico/#ixzz5LYwdYbat) Word.

Also, I finally got around to making use of the $6.50 I spent downloading Ripple's opposition to plaintiff's motion to remand the Ripple litigation from federal court to state court by writing [this short post]().  As I wrote on Medium, I was originally thinking that this procedural motion might set the stage for a larger, substantive finding on whether XRP was actually a security or not.  Now I'm not so sure the court will reach that issue... but it could still happen!

## Random Updates

"BENGALURU: Over 80% of blockchain developers in India will be forced to move abroad or work only on foreign projects if the government does not adopt a robust regulatory framework soon, according to a survey of over 100 developers." Thought [that lead was amusing](https://economictimes.indiatimes.com/articleshow/65019007.cms), especially considering they surveyed only devs. However, they raise an important point. Since many blockchain projects compensate developers in crypto, "An Indian developer may be able to receive tokens but if there is no legal way to convert it into Indian rupees." That's definitely a problem.
