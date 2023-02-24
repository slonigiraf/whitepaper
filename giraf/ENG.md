# GIRAF - Legislation for communities

_Denis Reshetov / E-mail:_ [_reshetovdenis@gmail.com_](mailto:reshetovdenis@gmail.com) _/ Telegram:_ [_@denisreshetov_](https://t.me/denisreshetov)

## Annotation

The paper suggests using the process of lawmaking as a model for coordinating small groups of people to jointly create documents that would be economically beneficial to them.

## What Is “Law”?

Laws are a fundamental part of human civilization and are generally understood to be a set of instructions or rules people have agreed to follow. Examples of laws include the Bill of Rights in the United States, the Wikipedia article on DNA, the history schoolbook, and the balance of a specific bitcoin wallet. However, the exact definition of "law" is debatable. In this document, we will use the above definition for our discussion.

| Legislator | Law | Why is it the law | How to fix |
| ----------- | ----------- | ----------- | ----------- |
| US Congress | Bill of rights (USA) | is used in courts | pay a lot of money to legislators (lobby) |
| Wikipedia | article about DNA | is used as a standard of truthful information in society | make edits yourself and convince other editors |
| Schoolbook author | history schoolbook | used in schools to teach children | bribe the author and publisher |
| Bitcoin | balance of a specific bitcoin wallet | it is possible to pay with this balance | pay miners for a transaction |

## How Laws Are Written

The process of lawmaking is closely tied to economic activity. For example, politicians in the United States often rely on [funding from lobbyists](https://en.wikipedia.org/wiki/Lobbying_in_the_United_States) to run for office and push for legislation that benefits those lobbyists. Similarly, editors of Wikipedia articles may spend their valuable time and resources [fighting for the content](https://en.wikipedia.org/wiki/Wikipedia:Edit_warring) of an article. The author of a schoolbook or a publishing house may receive funding from individuals or groups who wish to promote [their point of view](https://meduza.io/feature/2019/10/21/ministerstvo-prosveschenie). In the case of Bitcoin, miners [are paid](https://bitcoin.org/bitcoin.pdf) for changing the balances of wallets. In some cases, foreign countries may even intervene in the lawmaking process of another country [with money](https://www.reuters.com/article/politicsNews/idUSN2450753720071024).

The practice of buying and selling laws, also known as lobbying, is a global norm that is generally accepted and serves as an essential tool for creating consensus in society. It can lead to economic well-being, as seen in the United States with its well-established lobbying practices.

## Is Lobbying Bad or Good?

Lobbying is the act of attempting to influence decisions made by government officials, typically by private interest groups, individual citizens, or organizations. Lobbying can take many forms, including contacting government officials directly, providing information to support a particular position, and participating in public campaigns to promote a specific cause.

There are both potentially positive and negative aspects to lobbying. Some of the potential benefits of lobbying include the following:

- Advocating for causes that align with the values and interests of the group or individual doing the lobbying
- Providing a way for individuals or groups to have a voice in the political process and shape public policy
- Offering a way for groups to bring important issues to the attention of decision-makers

However, there are also potential negative aspects to lobbying, including:

- The potential for special interests to exert a disproportionate influence on the political process, potentially at the expense of the general public
- The potential for lobbying to be used to advance the interests of certain groups over others, leading to inequality and injustice
- The potential for lobbying to create a sense of cynicism among the public, as people may feel that their voices are not being heard

Overall, the effects of lobbying can be both positive and negative, depending on the specific circumstances and how it is conducted. It is crucial for lobbying to be transparent and accountable to ensure that it serves the public interest and does not undermine democracy.

## Direct Democracy and Laws

This paper proposes a solution for using legislation and transparent lobbying to coordinate small groups of people in creating valuable documents for them. The proposed approach involves several key steps:

- Any person can publish a new law by specifying the cost of the law or the amount of money the author is willing to distribute to the rest of the group.
- Other group members can weaken the law by reducing its value through their monetary contributions to the group.
- Anyone can repeal a published law by weakening it to zero cost by distributing money to other group members.
- The distribution of money during the lawmaking process occurs according to a proportional scheme, where individuals with more money receive a more significant share of the funds than those with less money.

This approach to lawmaking uses the established practice of lobbying, or the buying and selling of laws, to coordinate people in small groups. The proportional distribution of funds is necessary to maintain market incentives and prevent individuals from simply living off the contributions of others without contributing anything useful to society.

The distribution of money and the registration of laws can be conveniently implemented using blockchain technology, as this would allow for transparent and honest transfers of funds and the maintenance of a public record of laws.

## Application Architecture

I propose a general system architecture for creating and lobbying laws in small groups. The proposed system would involve the use of a database to store entries for each law, with each entry containing the following:

- A unique identifier for the law, such as a serial number.
- A hash of the text of the law, which could be generated using a system such as the [IPFS](https://ipfs.tech/).
- The amount of money that was distributed when the law was created.

Using hashes for the text of laws would allow efficient storage of laws utilizing a system such as IPFS while protecting against unauthorized changes.

The distribution of funds could be accomplished by reducing the balance of the wallet of the law's creator and proportionally increasing the balances of other members' wallets or by "burning" the specified amount from the creator's wallet balance. These approaches are [economically equivalent](https://www.coindesk.com/learn/what-does-it-mean-to-burn-crypto/), as "burning" money leads to an increase in the value of the remaining funds. Additionally, "burning" is a more straightforward computational operation on the blockchain.