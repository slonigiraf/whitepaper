# GIRAF - legislation for communities

_Denis Reshetov / E-mail:_ [_reshetovdenis@gmail.com_](mailto:reshetovdenis@gmail.com) _/ Telegram:_ [_@denisreshetov_](https://t.me/denisreshetov)

## Annotation

This paper proposes an approach on how to use the established practice of writing laws to coordinate people in small groups so that they can jointly create documents whose content is economically beneficial to them.

## Acknowledgements

Thanks to Aleksey Pastutsan for discussing the concepts of this document and suggesting the idea of "weaking of the law".

## What is "law"

The laws have been known since the beginning of human civilization. As the exact definition of the term "law" is debatable, we will use the following: a law is a set of instructions that people have agreed to follow, and also oblige to follow. Examples of what we understand by laws include: the Bill of Rights (USA); article on DNA on Wikipedia; history schoolbook; the balance of a specific bitcoin wallet.

| Legislator | Law | Why is it the law | How to fix |
| ----------- | ----------- | ----------- | ----------- |
| US Congress | Bill of rights (USA) | can be achieved through the court of their rights | pay a lot of money to legislators (lobby) |
| Wikipedia | article about DNA | is used as a standard of truthful information in society | make edits yourself and convince other editors |
| Schoolbook author | history textbook | used in schools to teach children | bribe the author and publisher |
| Bitcoin | balance of a specific bitcoin wallet | it is possible to pay with this balance | spend a lot of money (perform a 51% attack) |

## How laws are written

Law writing is linked to economic activities, for example, US congressional campaigns for politicians are [funded by lobbyists](https://en.wikipedia.org/wiki/Lobbying_in_the_United_States) who push for legislation to improve their well-being; editors of articles on Wikipedia spend their time, which is a valuable asset, [fighting for the content of the article](https://en.wikipedia.org/wiki/Wikipedia:Edit_warring); the author of the textbook and the publishing house can receive funding from a group of people who are interested in promoting [their point of view](https://meduza.io/feature/2019/10/21/ministerstvo-prosveschenie); and the miners of the Bitcoin network [take money](https://bitcoin.org/bitcoin.pdf) for changing the balances of wallets. There are even cases when a foreign country changes the laws of another country, [spending money on it](https://www.reuters.com/article/politicsNews/idUSN2450753720071024).

It can be argued that the purchase of laws (lobbying) is a generally accepted global norm, and the law itself is a commodity that can be bought and sold. Lobbying is an important tool for creating consensus in society, and leads to economic well-being (see US lobbying practices).

## Direct democracy and laws

Legislation is important for coordinating people, however, in small projects its use is problematic: it is clumsy and requires a large number of players: voters, legislators and lobbyists.

I propose a solution for how to use legislation and lobbying to coordinate people in small groups so that they can co-create documents whose content is cost-effective for them:

- anyone can publish a new law by specifying the cost of the law: how much money the author will voluntarily distribute to the rest of the group
- any person can weaken the law by reducing its value by the amount of money that he distributes to the rest of the group
- anyone can repeal a published law by weakening the law to zero cost
- the distribution of money during the creation of the law takes place in a proportional scheme: a member of the group who has more money receives more than the one who has little money.

Giving money is lobbying for a group of people. When a person distributes his money, he "buys the law", and, as we found out, "purchase of laws" is a working practice of legislation that has been established for thousands of years.

A proportional scheme for distributing money is needed to maintain market incentives. If distributed equally to everyone, then inevitably there will be people who live on the money from the distribution, but at the same time they themselves do not create anything useful for society.

The distribution of money and registration of laws at the moment can be conveniently implemented as a blockchain application, because this approach allows you to honestly transfer money, as well as maintain a public register of laws.

## Application architecture

I propose a general system architecture for the creation and lobbying of laws. Each entry in the database must contain:

- a unique identifier of the law, for example, its serial number
- hash of the text of the law, for example, cid of the text of the law in the [IPFS system](https://ipfs.tech/)
- the amount of money distributed when the law was created

The text hash is a string of several tens of letters long, for example hash-[cid](https://docs.filebase.com/ipfs/ipfs-cids) is 46 letters long. If at least one additional letter is added to the text of the law, then the hash will turn out to be radically different. We need hashes of laws so that, in order to save space, we store the text of the law not on the blockchain, but in the [IPFS system] (https://ipfs.tech/), and at the same time not be in danger of someone quietly rewriting the text.

The distribution of money can be carried out by reducing the balance of the wallet of the creator of the law and proportionally increasing the balances of the wallets of other people, or by "burning" the named amount from the balance of the wallet of the creator of the law. These approaches are [economic equivalents](https://www.coindesk.com/learn/what-does-it-mean-to-burn-crypto/) as “burning” leads to an increase in the value of the remaining money, in addition, “burning” is a simpler computational operation on the blockchain.