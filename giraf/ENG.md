# GIRAF - Legislation for communities

_Denis Reshetov / E-mail:_ [_reshetovdenis@gmail.com_](mailto:reshetovdenis@gmail.com) _/ Telegram:_ [_@denisreshetov_](https://t.me/denisreshetov)

## Annotation

The paper suggests using the process of lawmaking as a model for coordinating small groups of people to jointly create documents that would be economically beneficial to them.

## Acknowledgements

Thanks to Aleksey Pastutsan for discussing the concepts of this document and suggesting the idea of "weaking of the law".

The author of this paper would like to thank the creators of ChatGPT for providing a tool that was used to help polish the language in this paper.

## What is "law"

Laws are a fundamental part of human civilization and are generally understood to be a set of instructions or rules that people have agreed to follow. Examples of laws include the Bill of Rights in the United States, the Wikipedia article on DNA, history schoolbook, and the balance of a specific bitcoin wallet. However, the exact definition of the term "law" is a matter of debate. In this document, we will use the above definition for the purposes of our discussion.

| Legislator | Law | Why is it the law | How to fix |
| ----------- | ----------- | ----------- | ----------- |
| US Congress | Bill of rights (USA) | is used in courts | pay a lot of money to legislators (lobby) |
| Wikipedia | article about DNA | is used as a standard of truthful information in society | make edits yourself and convince other editors |
| Schoolbook author | history schoolbook | used in schools to teach children | bribe the author and publisher |
| Bitcoin | balance of a specific bitcoin wallet | it is possible to pay with this balance | pay miners for a transaction |

## How laws are written

The process of lawmaking is closely tied to economic activity. For example, politicians in the United States often rely on [funding from lobbyists](https://en.wikipedia.org/wiki/Lobbying_in_the_United_States) to run for office and push for legislation that benefits those lobbyists. Similarly, editors of Wikipedia articles may spend their valuable time and resources [fighting for the content](https://en.wikipedia.org/wiki/Wikipedia:Edit_warring) of an article, and the author of a schoolbook or a publishing house may receive funding from individuals or groups who wish to promote [their point of view](https://meduza.io/feature/2019/10/21/ministerstvo-prosveschenie). In the case of Bitcoin, miners [are paid](https://bitcoin.org/bitcoin.pdf) for their work in changing the balances of wallets. In some cases, foreign countries may even intervene in the lawmaking process of another country [with money](https://www.reuters.com/article/politicsNews/idUSN2450753720071024).

It can be argued that the practice of buying and selling laws, also known as lobbying, is a global norm that is generally accepted and serves as an important tool for creating consensus in society. This in turn can lead to economic well-being, as seen in the United States with its well-established lobbying practices.

## Is lobbying bad or good?

Lobbying is the act of attempting to influence decisions made by government officials, typically by private interest groups, individual citizens, or organizations. Lobbying can take many forms, including contacting government officials directly, providing information to support a particular position, and participating in public campaigns to promote a particular cause.

There are both potential positive and negative aspects to lobbying. Some of the potential benefits of lobbying include:

- Advocating for causes that align with the values and interests of the group or individual doing the lobbying
- Providing a way for individuals or groups to have a voice in the political process and shape public policy
- Offering a way for groups to bring important issues to the attention of decision-makers

However, there are also potential negative aspects to lobbying, including:

- The potential for special interests to exert disproportionate influence on the political process, potentially at the expense of the general public
- The potential for lobbying to be used to advance the interests of certain groups over others, leading to inequality and injustice
- The potential for lobbying to create a sense of cynicism among the public, as people may feel that their voices are not being heard and that decisions are being influenced by powerful interests

Overall, the effects of lobbying can be both positive and negative, depending on the specific circumstances and how it is conducted. It is important for lobbying to be transparent and accountable in order to ensure that it serves the public interest and does not undermine democracy.

## Direct democracy and laws

This paper proposes a solution for using legislation and transparent lobbying to coordinate small groups of people in the creation of documents that are beneficial for them. The proposed approach involves several key steps:

- Any person can publish a new law by specifying the cost of the law, or the amount of money that the author is willing to distribute to the rest of the group.
- Other members of the group can weaken the law by reducing its value through their own contributions of money to the group.
- Any person can repeal a published law by weakening it to zero cost through the distribution of money to other members of the group.
- The distribution of money during the lawmaking process takes place according to a proportional scheme, where individuals with more money receive a greater share of the funds than those with less money.

This approach to lawmaking uses the established practice of lobbying, or the buying and selling of laws, to coordinate people in small groups. The proportional distribution of funds is necessary to maintain market incentives and prevent individuals from simply living off the contributions of others without contributing anything useful to society.

The distribution of money and the registration of laws can be conveniently implemented using a blockchain technology, as this would allow for transparent and honest transfers of funds, as well as the maintenance of a public record of laws.

## Application architecture

I propose a general system architecture for the creation and lobbying of laws in small groups. The proposed system would involve the use of a database to store entries for each law, with each entry containing:

- A unique identifier for the law, such as a serial number.
- A hash of the text of the law, which could be generated using a system such as the [IPFS](https://ipfs.tech/).
- The amount of money that was distributed when the law was created.

The use of hashes for the text of laws would allow for the efficient storage of laws using a system like IPFS, while also providing protection against unauthorized changes to the text of the laws. 

The distribution of funds could be accomplished by reducing the balance of the wallet of the law's creator and proportionally increasing the balances of other members' wallets, or by "burning" the specified amount from the creator's wallet balance. These approaches are [economically equivalent](https://www.coindesk.com/learn/what-does-it-mean-to-burn-crypto/), as "burning" money leads to an increase in the value of the remaining funds. Additionally, "burning" is a simpler computational operation on the blockchain.