# Slonigiraf - education through cooperation

_Denis Reshetov / E-mail:_ [_reshetovdenis@gmail.com_](mailto:reshetovdenis@gmail.com) _/ Telegram:_ [_@denisreshetov_](https://t.me/denisreshetov)

## Annotation

We discuss the relationship between education and economic growth, and propose a system for incentivizing student-led instruction using cryptocurrency and recommendation letters. The system is intended to improve the retention of acquired skills, and has been implemented in several schools with reported success. The system aims to address challenges in peer learning, such as the lack of qualified educators and lack of motivation to teach among students, by providing financial compensation for teaching efforts and requiring mentors to issue recommendation letters. The system is also expected to have a positive impact on the economy, potentially adding 8 trillion USD or 8.4% of the global GDP to the world economy each year immediately.

## Education and GDP

Education plays a vital role in the economy. On average, countries [spend 4.2% of their GDP on education](https://data.worldbank.org/indicator/SE.XPD.TOTL.GD.ZS). If the quality of education were to be improved threefold, it could potentially add approximately 8 trillion USD, or 8.4% of the global GDP, to the world economy each year immediately. Traditional schooling typically has a retention rate of [25%](https://link.springer.com/article/10.1007/s10643-022-01332-3) for acquired skills, while using private tutoring can result in a retention rate of 75%. However, private tutoring can be costly and requires a large number of educators. Peer learning, where students mentor each other, [has been attempted in the past](https://en.wikipedia.org/wiki/Peer_learning) but faces two main challenges: the lack of qualified educators and lack of motivation to teach among students. To address these issues, we propose using a combination of cryptocurrency and a recommendation letter system to incentivize and ensure the quality of student-led instruction. By providing financial compensation for their teaching efforts and requiring mentors to issue recommendation letters for the skills they have taught, we can motivate students to act as educators while also maintaining educational standards. We have implemented this approach in several schools and have observed an increase in skill retention up to 75%, with students having ample time for both learning and teaching within their existing secondary education programs.

## SLON tokenomics

To calculate how much SLON do we need for students we should take into account:

Wm - minute wage of a mentor
Wt - minute wage of an expert
Ts - mean time that a mentor spend to teach a skill
Te - mean time that an expert spend to revise a skill
F - skill forgetting rate after teaching
R - reimbursement that a mentor pays to an expert
M - mathematical expectation of mentor earnings for 1 skill:

A good proxy for a Wm is a minimum teacher wage per country, and a good proxy for a Wt is a maximum teacher wage per country. We can see than mean Wt/Wm ration per country is a 3.16 thus we will use this estimation of Wt in a following calculations.
As an expert should get his wage during diploma verification we can write that:
R = Te * Wt / F
During an erly implementation Slonigiraf in private school we got estimation of an expert time for revising a diploma as: Te = 1.5 min
There is a published data that mean skill forgetting rate (F) [is about 0.25](https://link.springer.com/article/10.1007/s10643-022-01332-3), thus:
R = 1.5 * 3.16 * Wm / 0.25 = 18.96 * Wm

We should assume that a mentor should get enough payment for his work during teaching and also money to be able to pay premium to an expert in the case if student will forget the skill. Thus:
M = Ts * Wm + F * R = Ts * Wm + F * Te * Wt / F = Ts * Wm + Te * Wt

During an erly implementation Slonigiraf in private school we got estimation of a mentor time to teach a skill is 11 minutes. Thus:
M = 11 * Wm + 1.5 * Wt = 11 * Wm + 1.5 * 3.16 * Wm = (11 + 4.74) * Wm = 15.74 * Wm

R/M = (18.96 * Wm) / (15.74 * Wm) ~ 1.2

Any currency should be comfortable to use. The minumum integers that are good for R and M are 6 and 5 respectively.

As we plan to use Slonigiraf in big countries first we should select a country with minimal teacher wage and use R=6 and M=5 in it. We select Ethiopia as such country.

As M = 5,
5 = 15.74 * Wm
Wm = 0.31766201 SLON in Ethiopia.

Minimum teacher salary in Ethiopia is 30 USD.
Wm = 30 USD / (168*60) = 0.00297619 USD
0.00297619 USD = 0.31766201 SLON
1 SLON = 0.009369048 USD, thus 1 SLON ~ 1 USD cent.

Let's calculate the amount of SLON airdrop per person in Ethiopia.
Let's say 1 out of 32 children knows the skill, then there must be 5 lessons in pairs so that all 32 master the skill. Those who got the skill in the last lesson (16 people) only spend 5 SLON, but do not earn anything.
The probability of getting into these 16 people is 0.5.
This means that it is necessary to minimize such cases when a student ends up in the last training group in a row.
You need 32 * 5 SLON so that this situation does not happen to any student in the world (1.967 B * 0.5^32 < 1).
Thus 32 * 5 SLON = 160 SLON is enough amount to perform such lessons in Ethiopia.

Other countries have different minimum teacher wage. Thus we need to adjust an airdrop for each country separately, see the table 1.
We need total 4.32E+12 SLON for countries listed in the table 1, and 2.79E+12 SLON for others. Thus 7.11E+12 SLON in total just for an airdrop.

In the proposed system, is the total demand for SLON estimated to be just 7 trillion? To calculate this, it is important to note that the supply of cryptocurrencies, such as Bitcoin, is typically compared to M1 supply or narrow money. However, the supply of stacking cryptocurrencies is more closely aligned with M2 supply. The M2 money supply is [roughly equivalent to the GDP](https://data.worldbank.org/indicator/FM.LBL.BMNY.GD.ZS). As the additional GDP is estimated to be 8 trillion USD, the M2 SLON supply should be approximately 8 trillion USD, or 800 trillion SLON.

## Long lasting effect of education improvement

GDP is closely tied to the workforce. Using a conservative estimate that 1% of labor growth leads to a [0.36% increase in GDP](https://dergipark.org.tr/tr/download/article-file/364734), an improvement in education resulting in a 300% growth in the workforce would lead to a 108% increase in GDP, equivalent to approximately [96.51](https://data.worldbank.org/indicator/NY.GDP.MKTP.CD) trillion USD in the long-term. Based on this calculation, our initial estimation for the total demand on SLON tokens at 8 trillion USD should be revised upwards to 96.51 trillion USD, or an increase of about 12 times that could potentially lead to the cryptocurrency price growth.

## System software architecture

The proposed system, Slonigiraf, is composed of two interconnected components: [SLON](https://github.com/slonigiraf/whitepaper/blob/main/slon/ENG.md), which functions as a reputation system, and [GIRAF](https://github.com/slonigiraf/whitepaper/blob/main/giraf/ENG.md), which serves as a lobbying and legislation system. Both systems are implemented as distinct blockchains that are linked together through a relay chain. This design allows for the deployment of multiple SLON and GIRAF modules, enabling the system to handle a large scale of users and meet the diverse needs of the population. The GIRAF component is used to facilitate consensus on the types of skills that are necessary for education and the methods for teaching them. The term "SLON" is used both as the name of a Slonigiraf cryptocurrency and as the name of the module that stores information about recommendation letters.