# GIRAF - legislation for communities

_Denis Reshetov / E-mail:_ [_reshetovdenis@gmail.com_](mailto:reshetovdenis@gmail.com) _/ Telegram:_ [_@denisreshetov_](https://t.me/denisreshetov)

## Annotation

The paper suggests using the process of lawmaking as a model for coordinating small groups of people to jointly create documents that would be economically beneficial to them.

## Acknowledgements

Thanks to Aleksey Pastutsan for discussing the concepts of this document and suggesting the idea of "weaking of the law".

The author of this paper would like to thank the creators of ChatGPT for providing a tool that was used to help polish the language in this paper.

## What is "law"

Laws are a fundamental part of human civilization and are generally understood to be a set of instructions or rules that people have agreed to follow. Examples of laws include the Bill of Rights in the United States, the Wikipedia article on DNA, history textbooks, and the balance of a specific bitcoin wallet. However, the exact definition of the term "law" is a matter of debate. In this document, we will use the above definition for the purposes of our discussion.

| Legislator | Law | Why is it the law | How to fix |
| ----------- | ----------- | ----------- | ----------- |
| US Congress | Bill of rights (USA) | can be achieved through the court of their rights | pay a lot of money to legislators (lobby) |
| Wikipedia | article about DNA | is used as a standard of truthful information in society | make edits yourself and convince other editors |
| Schoolbook author | history textbook | used in schools to teach children | bribe the author and publisher |
| Bitcoin | balance of a specific bitcoin wallet | it is possible to pay with this balance | spend a lot of money (perform a 51% attack) |

## How laws are written

The process of lawmaking is closely tied to economic activity. For example, politicians in the United States often rely on [funding from lobbyists](https://en.wikipedia.org/wiki/Lobbying_in_the_United_States) to run for office and push for legislation that benefits those lobbyists. Similarly, editors of Wikipedia articles may spend their valuable time and resources [fighting for the content](https://en.wikipedia.org/wiki/Wikipedia:Edit_warring) of an article, and the author of a textbook or a publishing house may receive funding from individuals or groups who wish to promote [their point of view](https://meduza.io/feature/2019/10/21/ministerstvo-prosveschenie). In the case of Bitcoin, miners [are paid](https://bitcoin.org/bitcoin.pdf) for their work in changing the balances of wallets. In some cases, foreign countries may even intervene in the lawmaking process of another country [with money](https://www.reuters.com/article/politicsNews/idUSN2450753720071024).

It can be argued that the practice of buying and selling laws, also known as lobbying, is a global norm that is generally accepted and serves as an important tool for creating consensus in society. This in turn can lead to economic well-being, as seen in the United States with its well-established lobbying practices.

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