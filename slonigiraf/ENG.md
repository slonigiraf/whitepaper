# Slonigiraf - education through cooperation

_Denis Reshetov / E-mail:_ [_reshetovdenis@gmail.com_](mailto:reshetovdenis@gmail.com) _/ Telegram:_ [_@denisreshetov_](https://t.me/denisreshetov)

## Annotation

We explore how education influences on economic growth, and present an education system that seeks to outperform existing systems by threefold. The system is intended to reduce the forgetting of acquired skills, and has been implemented in several secondary schools with a reported success. It aims to address challenges in peer learning, such as lack of qualified educators and lack of motivation to teach among students, by providing financial compensation for teaching efforts and requiring mentors to issue recommendation letters. The system is expected to have a positive impact on the world economy, potentially adding 8 trillion USD to the world economy each year.

## Education and GDP

Education plays a vital role in the world economy. On average, education comprise [4.2%](https://data.worldbank.org/indicator/SE.XPD.TOTL.GD.ZS) of GDP - final goods and services produced and sold in a specific time period by countries. If the quality of education were to be improved threefold, it could potentially add approximately 8 trillion USD, or 8.4% of the global GDP, to the world economy each year with such effect size from the first year of an educational reform. 

Traditional schooling typically has a forgetting rate of [75%](https://link.springer.com/article/10.1007/s10643-022-01332-3) for acquired skills, while using private tutoring can reduce the forgetting rate by up to [25%](https://pubmed.ncbi.nlm.nih.gov/21574747/). However, private tutoring can be costly and requires a large number of educators. Peer learning, where students mentor each other, [doesn't outperform](https://pubmed.ncbi.nlm.nih.gov/23691355/) the traditional schooling because of [two main challenges](https://www.tandfonline.com/doi/full/10.1080/01443410500345172): the lack of motivation to teach among students and quality erosion due to the broken telephone effect.

To address these issues, we propose using money to incentivize students that act as mentors and require them to use recommendation letter system to ensure the quality of such lessons. By doing so, we can motivate students to act as educators while also maintaining educational standards. We have implemented this approach in several schools and have observed a reduce of the forgetting rate by up to 25%, with students having an ample time for both learning and teaching within their existing secondary education programs.

## Financial model

To calculate how much money we need for students in such system we should take into account:

- Wm - a minute wage of a mentor, which teach mentee and issues diploma on each skill
- Wt - a minute wage of an expert, who controls the quality of skills
- Ts - the mean time that a mentor spend to teach a skill
- Te - the mean time that an expert spend to revise a skill
- F - the skill forgetting rate after teaching
- R - the reimbursement that a mentor pays to an expert
- M - a mathematical expectation of mentor earnings for 1 skill:

A good proxy for a Wm is a minimum teacher wage per country, and a good proxy for a Wt is a maximum teacher wage per country. We can see the mean Wt/Wm ration per country is a 3.16 thus we will use this estimation of Wt in following calculations.
As an expert should get his wage during a diploma verification we can write that:

R = Te * Wt / F

During an early implementation of Slonigiraf in a private school we got the estimation of an expert time for revising a diploma as 1.5 min (Te). There is a published data that mean skill forgetting rate (F) [is about 0.25](https://link.springer.com/article/10.1007/s10643-022-01332-3), thus:

R = 1.5 * 3.16 * Wm / 0.25 = 18.96 * Wm

Presumably, a mentor should get enough payment for his work during teaching as well as the money to be able to pay premium to an expert in case a student forgets the skill. Thus:

M = Ts * Wm + F * R = Ts * Wm + F * Te * Wt / F = Ts * Wm + Te * Wt

During an early implementation of Slonigiraf in a private school we estimated thet the mentor time to teach a skill was 11 minutes. Thus:

M = 11 * Wm + 1.5 * Wt = 11 * Wm + 1.5 * 3.16 * Wm = (11 + 4.74) * Wm = 15.74 * Wm

R/M = (18.96 * Wm) / (15.74 * Wm) ~ 1.2

Any currency should be comfortable to use. Minumum whole numbers that are good for R and M are 6 and 5 respectively.

As part of our implementation strategy, we plan to prioritize the deployment of Slonigiraf in countries with high population density. Among these coutries we have identified a country with the lowest teacher wage - Ethiopia.

As M = 5,

5 = 15.74 * Wm

Wm = 0.31766201 SLON in Ethiopia.

A minimum teacher salary in Ethiopia is 30 USD.

Wm = 30 USD / (168*60) = 0.00297619 USD

0.00297619 USD = 0.31766201 SLON

1 SLON = 0.009369048 USD, thus 1 SLON ~ 1 USD cent.

Let's calculate the amount of SLON airdrop per person in Ethiopia.
Let's say that 1 out of 32 children knows the skill, then there must be 5 sessions during the lesson in pairs so that all 32 students master the skill. Those who gained the skill in the last session (16 people) spend 5 SLON each, but do not earn anything.
The probability to be among these 16 students is 0.5.

It is necessary to minimize such cases when a student ends up in the last training group in a row. We need 32 * 5 SLON so that this situation does not happen to any student in the world (1.967 B * 0.5^32 < 1). Thus 32 * 5 SLON = 160 SLON is enough amount to perform such lessons in Ethiopia.

Other countries have different teacher wages. Thus we need to adjust an airdrop for each country separately, see the table 1.
We need a total of 4.3 trln SLON for countries listed in the table 1, and 2.8 trln SLON for others. Thus 7.1 trln SLON is required in total just for an airdrop.

In the proposed system, is the total demand for SLON estimated to be just 7 trillion? To answer this question, it is important to note that the supply of cryptocurrencies, such as Bitcoin, is typically compared to M1 supply or narrow money. However, the supply of stacking cryptocurrencies is more closely aligned with M2 supply. The M2 money supply is [roughly equivalent to the GDP](https://data.worldbank.org/indicator/FM.LBL.BMNY.GD.ZS). As the additional GDP is estimated to be 8 trillion USD, the M2 SLON supply should be approximately 8 trillion USD or 800 trillion SLON.

## Long lasting effect of education improvement

GDP is closely tied to the workforce. Using a conservative estimate that 1% of labor growth leads to a [0.36% increase in GDP](https://dergipark.org.tr/tr/download/article-file/364734), the improvement in education resulting in a 3Х (or 200%) growth in the workforce would lead to a 72% increase in GDP, equivalent to approximately [69.5](https://data.worldbank.org/indicator/NY.GDP.MKTP.CD) trillion USD in the long term. Based on this calculation, our initial estimation for the total demand for SLON tokens at 8 trillion USD should be revised upwards to 77.5 (69.5+8) trillion USD that could potentially lead to the cryptocurrency 10X price growth (77.5/8). Additionally the demand for SLON tokens could rise due to usage the system for corporate education and HR processes. In order to ensure the price stability, we plan to implement an inflation rate of approximately 10%. This inflation is achieved by generating additional SLON through the process of "stacking" and is a common practice in the current cryptocurrency market as a reward for the hardware maintenance.

## System software architecture

The proposed system, Slonigiraf, is composed of two interconnected components: [SLON](https://github.com/slonigiraf/whitepaper/blob/main/slon/ENG.md), which functions as a reputation system, and [GIRAF](https://github.com/slonigiraf/whitepaper/blob/main/giraf/ENG.md), which serves as a lobbying and legislation system. Both systems are implemented as distinct blockchains that are linked together through a relay chain. This design allows for the deployment of multiple SLON and GIRAF modules, enabling the system to handle a large scale of users and meet the diverse needs of the population. The GIRAF component is used to facilitate consensus on the types of skills that are necessary for education and the methods for teaching them. The term "SLON" is used both as the name of a Slonigiraf cryptocurrency and as the name of the module that stores information about recommendation letters.