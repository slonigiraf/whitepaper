# Slonigiraf - education improvement using market instruments

_Denis Reshetov / E-mail:_ [_reshetovdenis@gmail.com_](mailto:reshetovdenis@gmail.com) _/ Telegram:_ [_@denisreshetov_](https://t.me/denisreshetov)

## Annotation

We explore how education influences on economic growth, and present an education system that seeks to outperform existing systems by threefold. The system is intended to increase the number of acquired skills, and has been implemented in several secondary schools with a reported success. It aims to address challenges in peer learning, such as lack of qualified educators and lack of motivation to teach among students. The system is expected to have a positive impact on the world economy, potentially adding 8 trillion USD to the world economy each year.

## Education and GDP

Education plays a vital role in the world economy. On average, education comprise [4.2%](https://data.worldbank.org/indicator/SE.XPD.TOTL.GD.ZS) of GDP - final goods and services produced and sold in a specific time period by countries. If the quality of education were to be improved threefold, it could potentially add approximately 8 trillion USD, or 8.4% of the global GDP, to the world economy each year with such effect size from the first year of an educational reform.

One way to measure the efficiency of an education system is by determining the average number of skills acquired by a group of students, divided by the total number of skills they were expected to acquire.

Traditional schooling typically has an efficiency about of [25%](https://link.springer.com/article/10.1007/s10643-022-01332-3), while using private tutoring the efficiency can be increased up to [75%](https://pubmed.ncbi.nlm.nih.gov/21574747/). However, private tutoring can be costly and requires a large number of educators. Peer learning, where students tutor each other, [doesn't outperform](https://pubmed.ncbi.nlm.nih.gov/23691355/) the traditional schooling because of [two main challenges](https://www.tandfonline.com/doi/full/10.1080/01443410500345172): the lack of motivation to teach among students and quality erosion due to "the broken telephone effect".

To address these issues, we propose using money to incentivize students to act as tutors and require them to use recommendation letter system to ensure the quality of such lessons. By doing so, we can motivate students to act as educators while also maintaining educational standards. We have implemented this approach in several schools and observed an increase of the education efficiency up to 75%, with students having an ample time for both learning and teaching within their existing secondary education programs.

## Proposed educational model

<img alt="Image" src="https://github.com/slonigiraf/slon-whitepaper/blob/main/img/lesson.png?raw=true" width="500">

*Figure 1. Proposed educational model named as "Slonigiraf"*

### Tutoring and diploma issuing

The **"Slonigiraf" lesson** doesn't contain any lecture part. Instead it begins with working in pairs. Each student can name himself as a **tutor** of the specific skill or be a tutee. A **tutee** selects his tutor based on the personal preference. Tutors are peers of students - they study the same class but somehow knew a **skill** before their tutee. A tutor charges his tutee money for the tuition. As a result of each tuition the tutor issues a diploma.

Each **diploma** is a unique electronic document, that can be canceled in any time if a tutee will show it to an expert and the expert will say that the tutee doesn't posses the skill. The expert gets a **reimbursement** for identifing a fake diploma. The reimbursement is paid by the tutor who issued such diploma. The amount of reimbursement is defined at the stage of diploma issuing. Thus each diploma contains the information: which skill was trained, who was a tutor, who was a tutee and what is an amount of the possible reimbursement.

Often at the beginning of the lesson there are several tutors of the skill, because they studied this skill by themselves or know it outside of the lesson from their parents or from previous tuition, thus the lesson starts with a number of tutor-tutee pairs.

Let's see how lesson takes place when only one tutor exists. At the fig. 1. such tutor is marked with letter "A" at the leftmost pane. The tutor selects a tutee who proposed him the maximum amount of money or based on any other criterion that he decides by himself. This tuition is marked as "session 1" in the Fig. 1. After such tuition his tutee can decide to be a tutor by himself. And then these 2 tutors can teach the skill two more students. This action is named "session 2". Each session doubles number of tutors. After session 1 we have 2 students with diploma, after second - 4, after third - 16. This can be shortly written as following:

$2^{sessions} = diplomas$

For example: $2^{5} = 32$: after 5 sessions we expect to have 32 diplomas, meaning that 32 students acquired the skill. What if the lesson takes part not in a school but in an university and we need to teach 512 students that came to our course? How many sessions are needed to spread a skill? Using the formula above we can write: $2^{x} = 512$. By simple internet search or by using logarithm we can find that $x=9$. Thus we need only 9 sessions to teach 512 peoples a skill.

### Tutors have different number of tutees

<img alt="Image" src="https://github.com/slonigiraf/slon-whitepaper/blob/main/img/tutees_count.png?raw=true" width="500">

*Figure 2. Tutees count*

To estimate what tutor roles student can play in the Slonigiraf educational model and what are probabilities of playing such roles let's examine a class consisting of 32 students. We will explain later why probabilities of different roles are more of less the same in any student group size.

**Tutor of 0 tutees role**: as shown on a fig. 2. a half of students (16 from 32) gains a skill in a last session. That means they will pay for tutoring and geting a diploma but will not earn money by tutoring such skill as there will be no student left that need a skill. If the class consists of 32 students there will be 16 such students (depicted with a digit "0" on a fig. 2).

**Tutor of 1 tutees role**: $1/4$ of students (8 from 32) gain a skill in a preterminal session. These students have 1 tutor and 1 tutee each, which results in a 0 profit result as they compensate money paid to their tutors by money acquired by being a tutor.

**Tutor of 2 tutees role**: $1/8$ of students (4 from 32) have 2 tutees.

**Tutor of 3 tutees role**: $1/16$ of students (2 from 32) have 3 tutees.

**Tutor of 4 tutees role**: $1/32$ of students (1 from 32) have 4 tutees.

**Tutor of 5 tutees role**: $1/32$ of students (1 from 32) have 5 tutees.

With growing number of mentees the probability of such role is decreasing sugnificantly. We will not discuss the probability of having  more than 5 tutees in larger classes, as probabilites of such roles are too small to generally affect calculations of our model economy.

Growing class number doesn't much affect probabilites of different roles. For example 32 from 64 students class will play "tutor of 0 tutees" role. It's the same 0.5 probability of the role in class of 32 students. We can assume that our estimations of role probabilities are good in general.

All students have a tutor as all need to get a diploma. The student that have 5 tutees probably gets his diploma by communicating with a tutor outside the group. It can be the teacher of parent or any other type of the tutor. As we discussed before it's allowed to be a tutor while not having a diploma about the skill but for sure it rises the risk for the tutor to fail his work thus students tend to study the skill first, then get a diploma and only after this teach others.

### Students are allowed to become experts

A fact that a student got the diploma doesn't mean he has mastered the skill. It just means that his tutor believes in it. However the tutor can be wrong. For example, if the tutor himself doesn't posess such skill, or he didn't verified the skill proficiency of tutee by the adequete number of tasks, or the tutee can simply forget the skill. To maintain the good quality of education our system uses experts who verify diplomas and have a right to reward students with "A" grade or with any other type of reward. At the beginning of the lesson there is only one expert - the master teacher who runs and controls all the lesson. He is not able to verify all diplomas as it requires too much times. But he can delegate such position to few experts from students that got the diploma on the studied skill. The teacher verify that students that want to be experts posses the skill. If some of them fail the verification the teacher gets reimbursement from a tutor who issued the diploma. Those who passed such verification start to play **an expert role**.

### Experts earn money via searching for low quality skills

Why students do want to become experts? The expert status allows them to verify a lot of diplomas and eventually find bad ones and get reimbursement from tutors who issued such dimplomas. For sure an expert want to name all diplomas coming to him as bad ones to get as much reward as possible. To prevent such situation we allow students to select which expert to deal with. This creates a competition between experts and makes them to behave honestly.

The teacher is allowed to re-verify diplomas verified by an expert if he suspects that the expert is cheating: for example if the expert verified the diploma issued by himself. In the case of cheating the teacher can prohibit the student to be an expert for certain amount of time and also the teacher gets the reimbursement from the tutor who issued the diploma used in cheating.

### Teacher salary can be adjusted to the quality of teaching

**The teacher role** differs in three ways from students:

- he is an adult with pedagogical education
- the teacher plays an expert role by default
- he can allow students to become experts

This allows us to propose two diffent models of teacher salary calculation. The first is conservative and doesn't change how things are done in classic way: the teacher just gets salary from the school budget. We think that such way will prevale during a transition from traditional educational model to the Slonigiraf. When this option is applyed the teacher doesn't get money from students for tutoring and diploma issuing. He just teaches 1 - 2 students for free and they spread the skill to other students for money. However the teacher is allowed to get reimbursement from bad mentors in a way as any expert is allowed but the money he got in such a way then are collected to the school budget and are returned back to all students on an equal basis monthly.

The second way of teacher salary calculation has more market spirit. It assumes that the teacher will not get any salary from the school budget. In such way he is allowed to earn money both as a mentor and as an expert. The school budget money that were intended to be addressed to teacher are spread instead of it to students on an equal basis each month.

## Financial model

### It targets 2 billions of people in the world

As we propose such system for an education in groups we need to estimate the world population of students. To be conservative let's speak that only **7 - 21 yo strata** will use our educational model. We've found a data about total population size of each country as of [2021.01.01](https://population.un.org/wpp/Download/Standard/MostUsed/), and the data of [percent of 0-14 yo people](https://www.theglobaleconomy.com/rankings/percent_children/) as of 2021. We think that a percent of 7 - 21 yo strata can be approximated by the 0 - 14 yo strata. Thus to calculate the target audience per country we should multiply a population size on a percent of 7 - 21 yo strata and divide by 100%. The resulting data is shown in the table 1. You can see that India has the biggest target audience of 361 million people, and the total world target audience is **2 billion people**.

|             | Total Population | 7-21 years old % | 7-21 years old |
| ----------- | ------------- | ------ | ------------- |
| India       | 1,402,807,867 | 25.78% | 361,643,868   |
| China       | 1,425,861,543 | 17.60% | 250,951,632   |
| Nigeria     | 210,874,214   | 43.31% | 91,329,622    |
| Pakistan    | 229,280,621   | 34.63% | 79,399,879    |
| Indonesia   | 272,890,093   | 25.62% | 69,914,442    |
| USA         | 336,495,769   | 18.24% | 61,376,828    |
| Ethiopia    | 118,743,462   | 39.56% | 46,974,914    |
| Bangladesh  | 168,414,908   | 26.31% | 44,309,962    |
| Brazil      | 213,827,672   | 20.45% | 43,727,759    |
| Egypt       | 108,391,549   | 33.83% | 36,668,861    |
| Philippines | 113,094,332   | 29.53% | 33,396,756    |
| Mexico      | 126,386,142   | 25.49% | 32,215,828    |
| Russia      | 145,472,994   | 18.49% | 26,897,957    |
| Japan       | 124,946,751   | 12.30% | 15,368,450    |
| Rest world  | 2,911,807,000 | 26.51% | 771,920,036   |
| TOTAL       | 7,909,294,917 |        | 1,966,096,793 |

*Table 1. Target audience (7-21 years old people). The value of 7-21 strata percent for rest world was calculated as an average for countries from the list above.*

### Work force price

To discuss a work force price of tutors and experts we should remember that a student that understood how to be a tutor can potentially go to a educational market out of the school or university and get money for helping other students than his peers. Thus we can approximate the wage of a tutor with the lowest wage of teacher in the country that he lives.

The expert wage should be larger than the tutor wage to motivate most qualified students to become experts. As qualified students can find a good position in an online tutoring we can assume that the maximum teacher wage in the country where the expert lives could be a good approximation of the market expert wage.

We collected teacher wage data per country from [salaryexplorer.com](http://www.salaryexplorer.com/?loc=23&loctype=1&job=123&jobtype=3#browsesalaries) on 2023.01.08. From the Table 2 you can see that maximum teacher wage on average is 3.16 times higher that minimum teacher wage. Thus **an expert should get 3.16 times more money per 1 minute of his work than a tutor**. Teacher wage is minimal in Ethiopia so a tutor will get in Ethiopia the smallest wage in comparison to other countries listed in the table 2.

|             | Min | Max | Max/Min |
| ----------- | ------- | ------- | ------- |
| India       | 143.42  | 458.21  | 3.19    |
| China       | 1637.81 | 4796.44 | 2.93    |
| Nigeria     | 282.07  | 831.02  | 2.95    |
| Pakistan    | 142.57  | 419.79  | 2.94    |
| Indonesia   | 313.31  | 922.63  | 2.94    |
| USA         | 3040.00 | 9680.00 | 3.18    |
| Ethiopia    | 30.20   | 104.50  | 3.46    |
| Bangladesh  | 86.84   | 300.38  | 3.46    |
| Brazil      | 604.68  | 2085.76 | 3.45    |
| Egypt       | 126.68  | 401.40  | 3.17    |
| Philippines | 268.36  | 929.35  | 3.46    |
| Mexico      | 679.37  | 2168.76 | 3.19    |
| Russia      | 528.28  | 1558.63 | 2.95    |
| Japan       | 1620.17 | 4762.09 | 2.94    |
| Average     |         |         | 3.16    |

*Table 2. Teacher monthly wages in USD per country.*

### $D$ - diploma price and $R$ - reimbursement amount

Let's calculate a reimbursement amount and a mean diploma price. We will use Ethiopia as a country with a minimal teacher wage to deal with small numbers during calculations.

A reimbursement is a money amount that a tutor pays to an expert who found that a tutee doesn't posses a skill which was underwritten in the diploma. An expert verifies several dimplomas before he can find one with forgotten skill thus we need to estimate such number of diplomas. It's known that tutees forget [1 skill from 4 studied](https://link.springer.com/article/10.1007/s10643-022-01332-3) thus an expert should spend a time to verify 4 dimplomas on average to get 1 reimbursement. We identified experimentally that an expert need 1.5 minutes to verify 1 diploma, thus an expert spend 6 minutes (4*1.5) to get 1 reimbursement. So we can say that a reimbursement is equal to a price of 6 minutes work of an expert. As we wrote previously an expert wage on average is 3.16 higher than minimum teacher wage.

Ethiopian minimum teacher wage is 30.20 USD per month. A minute of such work costs 0.003 USD:

$30.20 / (21 * 8 * 60) = 0.003$

Thus 1 minute of an expert work price should equal to 0.00948 USD:

$0.003 * 3.16 = 0.00948$

And 6 minutes of an expert work is equal to 0.05688 USD:

$0.00948 * 6 = 0.05688$

So, **the reimbursent amount should be around 0.05688 USD in Ethiopia** to motivate students to perform an expert work.

During 4 years of Slonigiraf educatinal model testing in different schools we have experimentally identified that a tutor needs on average 11 minutes to teach a tutee. As a minute of the tutor work costs 0.003 USD in Ethiopia than the tutor work per 1 skill should cost 0.033 USD:

$0.003*11 = 0.033$

The tutor gets money from tutee not only for his time but also for issuing a diploma that can be canceled by an expert. If the tutor will not get some premium for issuing the diploma he will lose money as it's not possible to completely exclude the situtation when tutee will forget the skill. As we mentioned tutees forget 1 skill from 4 studied, thus a tutor should add a premium of 1 reimbursement amount to each 4 skills that he teaches, or simply $1/4$ of such amount to each diploma issuing, thus **the total price of a diploma will be 0.04722 USD in Ethiopia**:

$0.033+0.05688*1/4=0.04722$

If we will divide the calculated reimbursement amount by a diploma price than we can conclude that the reimbursement is 1.2 times bigger than the diploma price:

$0.05688/0.04722$

As all issued diplomas go through the verification it's NOT profitable to a tutor to cheat the system just issuing a lot of number of diplomas because he will lose 1.2 times more money than earning.

### Situations leading to earning and spending money

As we discussed above there are following roles in the Slonigiraf educational system: a teacher, an expert, a tutor of 0 tutees, a tutor of 1 tutees ...

Experts don't risk, they just earn. The teacher can lose some money if some of his mentees will forget the skill. But as he teaches only 1 student per a skill and also works as an expert he is always makes more money than he loses.

Any tutor spend money to learn a skill, earns money teaching others, and spend money if any his tutees forgets the skill. Thus a tutor profit can be written in formula:

$Profit = -D + D * N{_t} - R * N{_f}$

Where:

- $D$ - diploma price
- $R$ - reimbursement amount
- $N{_t}$ - tutees count of the tutor
- $N{_f}$ - number of tutees who have forgetten the skill.

If the a student doesn't have tutees then $N{_t}$ and $N{_f}$ are equal to $0$, and the formula gives us a profit value for these student equal to $-D$: they only pay for diploma to their tutors but don't earn anything.

As we calculated above the $R$ is 1.2 times bigger than $D$, so we can substitute $R$ in the equation above with $1.2*D$:

$Profit = -D + D * N{_t} - 1.2 * D * N{_f}$

Then we will put the price of the diploma out of brackets:

$Profit = D * (-1 + N{_t} - 1.2 * N{_f})$

You can see that $Profit < 0$ only if $(-1 + N{_t} - 1.2 * N{_f}) < 0$, or simply when $N{_t} - 1.2 * N{_f} < 1$

Table 4 summarizes when it can happen.

| Role              | $N{_t}$ | $N{_f}$ | $N{_t}-1.2*N{_f}$ | Losing money |
| ----------------- | -- | -- | ------------ | ------------ |
| Tutor of 0 tutees | 0  | 0  | 0            | Yes          |
| Tutor of 1 tutees | 1  | 0  | 1            | No           |
| Tutor of 1 tutees | 1  | 1  | \-0.2        | Yes          |
| Tutor of 2 tutees | 2  | 0  | 2            | No           |
| Tutor of 2 tutees | 2  | 1  | 0.8          | Yes          |
| Tutor of 2 tutees | 2  | 2  | \-0.4        | Yes          |
| Tutor of 3 tutees | 3  | 0  | 3            | No           |
| Tutor of 3 tutees | 3  | 1  | 1.8          | No           |
| Tutor of 3 tutees | 3  | 2  | 0.6          | Yes          |
| Tutor of 3 tutees | 3  | 3  | \-0.6        | Yes          |
| Tutor of 4 tutees | 4  | 0  | 4            | No           |
| Tutor of 4 tutees | 4  | 1  | 2.8          | No           |
| Tutor of 4 tutees | 4  | 2  | 1.6          | No           |
| Tutor of 4 tutees | 4  | 3  | 0.4          | Yes          |
| Tutor of 4 tutees | 4  | 4  | \-0.8        | Yes          |
| Tutor of 5 tutees | 5  | 0  | 5            | No           |
| Tutor of 5 tutees | 5  | 1  | 3.8          | No           |
| Tutor of 5 tutees | 5  | 2  | 2.6          | No           |
| Tutor of 5 tutees | 5  | 3  | 1.4          | No           |
| Tutor of 5 tutees | 5  | 4  | 0.2          | Yes          |
| Tutor of 5 tutees | 5  | 5  | \-1          | Yes          |

*Table 4. Cash flow outcomes of different roles*

### Losing money probability

If the student constantly faces money losses he will be bankrupt. Table 4 gives us insights which situtations lead to money lost. Let's bring together the probability of playing each role and probability of losing money in each role. We will focuse on the situtations that lead to money loss. For example a "tutor of 5 tutees" paying 3 reimburses has a positive profit and we will not discuss that probability of such events in this section.

The probability of playing each role can be taken from fig. 2 and was calculated as number of students in each role divided by total number of students.

If student plays a role of a tutee and doesn't become a tutor he will lose money each time so the probability to lose money while playing a role of "a tutor with 0 tutee" is 1.

A tutee pays to his tutor not only to study a skill but also to get a diploma. Diploma is very similar to an insurance police because the tutor promises to pay a reimbursement to an expert if the tutee will forget the skill. As in insurance business bad things can happen by chance more often than expected and the tutor can run out of money due to reimbursements. The probability that a tutee forgets a skill is [0.25](https://pubmed.ncbi.nlm.nih.gov/21574747/). Thus if a tutor has only 1 tutee he he faces 0.25 probability to pay a reimbursement.

The tutor having 2 tutees has 2 outcomes when he will lose money:

- both tutees forget the skill
- any one student forgets the skill

To calculate the probability both tutees forget the skill, we will think of them as independent events. So we need to [multiply probability of first event on the probability of the second](https://en.wikipedia.org/wiki/Independence_(probability_theory)). Thus the probability that a tutor having 2 tutees will pay 2 reimbursements is equal to $0.25 * 0.25 = 0.0625$.

The probability for such tutor that only first tutee will forget the skill is calculated in a similar way: $0.25 * (1 - 0.25) = 0.1875$, where $(1 - 0.25)$ is the probability that second tutee will retain the skill. The probability that only second mentee will forget the skill is the same: $(1 - 0.25) * 0.25 = 0.1875$. Thus a total probability that any one student forgets the skill is $2 * 0.1875 = 0.375$.

Other values in the column "Such reimbursement count probability for a role" of table 5 are calculated with the same approach. We will not provide the description of these calculations to be succint.

To calculate the probability that a student learning a skill will face a money loss due to a specific role facing N reimbursements we need to multiply the probability of playing such a role on a probability of such reimbursement count for a role, for example for "tutor of 2 tutees" that pays 1 reimbursements it is: $0.125 * 0.375 = 0.046875$. If we will sum all probabilities for such bad luck situations we will get that a student with a **probability of 0.629** will lose some money during any skill learning.

| Role | Count of reimbursements | Role probability | Such reimbursement count probability for a role | Probability of such situation |
| ----------------- | ---- | ------- | ---------- | ----------- |
| Tutor of 0 tutees | 0    | 0.5     | 1          | 0.5         |
| Tutor of 1 tutees | 1    | 0.25    | 0.25       | 0.0625      |
| Tutor of 2 tutees | 1    | 0.125   | 0.375      | 0.046875    |
| Tutor of 2 tutees | 2    | 0.125   | 0.0625     | 0.0078125   |
| Tutor of 3 tutees | 2    | 0.0625  | 0.140625   | 0.008789063 |
| Tutor of 3 tutees | 3    | 0.0625  | 0.015625   | 0.000976563 |
| Tutor of 4 tutees | 3    | 0.03125 | 0.046875   | 0.001464844 |
| Tutor of 4 tutees | 4    | 0.03125 | 0.00390625 | 0.00012207  |
| Tutor of 5 tutees | 4    | 0.03125 | 0.01464844 | 0.000457764 |
| Tutor of 5 tutees | 5    | 0.03125 | 0.00097656 | 3.05176E-05 |
|Total              |      |         |            | **0.62902832**  |

*Table 5. Probability to lose money playing a certain role*

### If we know that student lost money - what happened?

We have calculated the probability to lose money for a student while learning a skill. What if we know he already lost money, can we identify the reason of it? The answer is "No" but we can describe the probability of different scenarios. It's more likely the student was a tutor of 0 mentees, because the probability to play such a role and lose money is 0.5 (see the last column of table 5). And the 0.5 takes the most [share](https://calcworkshop.com/probability/bayes-theorem/) of total 0.629 probability to lose money. This situation is happen in 0.794876771 part of bad cases:

$0.5 / 0.62902832 = 0.794876771$

All such shares are calculated and represented in a table 6.

| Role | Count of reimbursements | Probability of such situation | Part that such situtation takes in all bad luck cases |
| ----------------- | - | ---------- | ---------- |
| Tutor of 0 tutees | 0 | 0.5        | 0.79487677 |
| Tutor of 1 tutees | 1 | 0.0625     | 0.0993596  |
| Tutor of 2 tutees | 1 | 0.046875   | 0.0745197  |
| Tutor of 2 tutees | 2 | 0.0078125  | 0.01241995 |
| Tutor of 3 tutees | 2 | 0.00878906 | 0.01397244 |
| Tutor of 3 tutees | 3 | 0.00097656 | 0.00155249 |
| Tutor of 4 tutees | 3 | 0.00146484 | 0.00232874 |
| Tutor of 4 tutees | 4 | 0.00012207 | 0.00019406 |
| Tutor of 5 tutees | 4 | 0.00045776 | 0.00072773 |
| Tutor of 5 tutees | 5 | 3.0518E-05 | 4.8515E-05 |

*Table 6. Probability that a specific situation leaded to the money loss*

### $A$ - a student starting capital

Our educational approach forces a tutee  to pay their tutor for skill-teaching and the issuance of a diploma, and requires the tutor to be responsible for the issued diploma by providing reimbursement when a tutee  forgets the skill certified by the diploma. To make this happen we need to assure that students have enough money for such economic interaction. As we discussed above there is a 62.9% chance that a student will spend more money during learning a skill that earn. For sure in rest 37.1% cases the student gets in sum the same profit as he losing in 62.9% cases, so his profit during years of learning should be near 0. But what if the student has a bad luck and all skills that he studies he is playing roles that lead to losing money? In such case he will start to pay for an education while we still suppose that the education should be a free resource for any person in on the Earth. To solve this problem we need to provide each each student at the beginning of such approach enough money to prevent bankruptcy happening at all. Let's calculate how many person in the world will get any of bad luck sequences.

The probability to get back luck studying the first skill is a 0.629. Thus if our target audience is 1,966,096,793 people than $0.629 * 1,966,096,793 = 1,236,730,563$ of them will face it. The sequence of 2 bad luck cases will affect 0.629 part of 1,236,730,563 that is $0.629 * 1,236,730,563 = 777,938,548$ people and so on (see the Appendix 2, for all values calculations). About 19 million people will face with a sequence of 10 bad luck cases.

Only 1 person in the world is expected to face a sequence of 48 bad luck cases, and nobody is supposed to face 49 bad luck cases.

As we mentioned we think that the education should be free so amount of money that we give to each student should be enough to wait out a sequence of 49 bad luck cases.

For now we know the probability of each event for skill, we know which events lead to money loss. Also we know the total probability to face a money loss learning a skill. As we are going to discuss sequences of bad luck cases let's calculate an additional probability that shows if we know that bad luck case happen what is a probability that a specific event happen? For example, if the student lost money during a skill learning what is a probability that he is "a tutor of 2 tutees" that pays 1 reimbursement? That can be calculated using [Bayes' theorem](https://en.wikipedia.org/wiki/Bayes%27_theorem) by multipling the probability to become "a tutor of 2 tutees" on probability that such tutor pays 1 reimbursent and dividing it on total bad luck probability: $0.125 * 0.375 / 0.62902832 = 0.074519697$

The amount of lost money can be calculated with the formula already discussed:

$Profit = D * (-1 + N{_t} - 1.2 * N{_f})$




R/M = (18.96 * $W{_t}$) / (15.74 * $W{_t}$) ~ 1.2

Any currency should be comfortable to use. Minumum whole numbers that are good for R and M are 6 and 5 respectively.

As part of our implementation strategy, we plan to prioritize the deployment of Slonigiraf in countries with high population density. Among these coutries we have identified a country with the lowest teacher wage - Ethiopia.

As M = 5,

5 = 15.74 * $W{_t}$

$W{_t}$ = 0.31766201 SLON in Ethiopia.

A minimum teacher salary in Ethiopia is 30 USD.

$W{_t}$ = 30 USD / (168*60) = 0.00297619 USD

0.00297619 USD = 0.31766201 SLON

1 SLON = 0.009369048 USD, thus 1 SLON ~ 1 USD cent.

Let's calculate the amount of SLON airdrop per person in Ethiopia.
Let's say that 1 out of 32 children knows the skill, then there must be 5 sessions during the lesson in pairs so that all 32 students master the skill. Those who gained the skill in the last session (16 people) spend 5 SLON each, but do not earn anything.
The probability to be among these 16 students is 0.5.

It is necessary to minimize such cases when a student ends up in the last training group in a row. We need 32 * 5 SLON so that this situation does not happen to any student in the world (1.967 B * 0.5^32 < 1). Thus 32 * 5 SLON = 160 SLON is enough amount to perform such lessons in Ethiopia.

Other countries have different teacher wages. Thus we need to adjust an airdrop for each country separately, see the Appendix 1.
We need a total of 4.3 trln SLON for countries listed in the Appendix 1, and 2.8 trln SLON for others. Thus 7.1 trln SLON is required in total just for an airdrop.

In the proposed system, is the total demand for SLON estimated to be just 7 trillion? To answer this question, it is important to note that the supply of cryptocurrencies, such as Bitcoin, is typically compared to M1 supply or narrow money. However, the supply of stacking cryptocurrencies is more closely aligned with M2 supply. The M2 money supply is [roughly equivalent to the GDP](https://data.worldbank.org/indicator/FM.LBL.BMNY.GD.ZS). As the additional GDP is estimated to be 8 trillion USD, the M2 SLON supply should be approximately 8 trillion USD or 800 trillion SLON.



## Long lasting effect of education improvement

GDP is closely tied to the workforce. Using a conservative estimate that 1% of labor growth leads to a [0.36% increase in GDP](https://dergipark.org.tr/tr/download/article-file/364734), the improvement in education resulting in a 3Х (or 200%) growth in the workforce would lead to a 72% increase in GDP, equivalent to approximately [69.5](https://data.worldbank.org/indicator/NY.GDP.MKTP.CD) trillion USD in the long term. Based on this calculation, our initial estimation for the total demand for SLON tokens at 8 trillion USD should be revised upwards to 77.5 (69.5+8) trillion USD that could potentially lead to the cryptocurrency 10X price growth (77.5/8). Additionally the demand for SLON tokens could rise due to usage the system for corporate education and HR processes. In order to ensure the price stability, we plan to implement an inflation rate of approximately 10%. This inflation is achieved by generating additional SLON through the process of "stacking" and is a common practice in the current cryptocurrency market as a reward for the hardware maintenance.

## System software architecture

The proposed system, Slonigiraf, is composed of two interconnected components: [SLON](https://github.com/slonigiraf/whitepaper/blob/main/slon/ENG.md), which functions as a reputation system, and [GIRAF](https://github.com/slonigiraf/whitepaper/blob/main/giraf/ENG.md), which serves as a lobbying and legislation system. Both systems are implemented as distinct blockchains that are linked together through a relay chain. This design allows for the deployment of multiple SLON and GIRAF modules, enabling the system to handle a large scale of users and meet the diverse needs of the population. The GIRAF component is used to facilitate consensus on the types of skills that are necessary for education and the methods for teaching them. The term "SLON" is used both as the name of a Slonigiraf cryptocurrency and as the name of the module that stores information about recommendation letters.

## Appendix 1. Global economy indicators

|             | 7-21 years old people\* | Times min teacher wage  is larger than Ethiopian counterpart | Min money a student need | Diploma price (SLON) | Reimbursement amount (SLON) | Airdrop per person (SLON) | Airdrop per country (SLON) |
| ----------- | ----------------------- | ------------------------------------------------------------ | ------------------------ | -------------------- | --------------------------- | ------------------------- | -------------------------- |
| India       | 361,643,868             | 4.75      | $7.59                    | 23                   | 28                          | 759                       | 275 B                      |
| China       | 250,951,632             | 54.23     | $81.30                   | 271                  | 325                         | 8677                      | 2178 B                     |
| Nigeria     | 91,329,622              | 9.34      | $14.00                   | 46                   | 56                          | 1494                      | 137 B                      |
| Pakistan    | 79,399,879              | 4.72      | $7.07                    | 23                   | 28                          | 755                       | 60 B                       |
| Indonesia   | 69,914,442              | 10.37     | $15.54                   | 51                   | 62                          | 1659                      | 116 B                      |
| USA         | 61,376,828              | 100.66    | $150.89                  | 503                  | 603                         | 16105                     | 989 B                      |
| Ethiopia    | 46,974,914              | 1.00      | $1.50                    | 5                    | 6                           | 160                       | 8 B                        |
| Bangladesh  | 44,309,962              | 2.88      | $4.31                    | 14                   | 17                          | 460                       | 21 B                       |
| Brazil      | 43,727,759              | 20.02     | $30.01                   | 100                  | 120                         | 3203                      | 141 B                      |
| Egypt       | 36,668,861              | 4.19      | $6.29                    | 20                   | 25                          | 671                       | 25 B                       |
| Philippines | 33,396,756              | 8.89      | $13.31                   | 44                   | 53                          | 1421                      | 48 B                       |
| Mexico      | 32,215,828              | 22.50     | $33.72                   | 112                  | 134                         | 3599                      | 116 B                      |
| Russia      | 26,897,957              | 17.49     | $26.21                   | 87                   | 104                         | 2798                      | 76 B                       |
| Japan       | 15,368,450              | 53.65     | $80.41                   | 268                  | 321                         | 8583                      | 132 B                      |
| SUM         | 1,194,176,758           |           |                          |                      |                             |                           | 4316 B                     |
| Rest world  | 771,920,036             |           |                          |                      |                             |                           | 2790 B                     |
| TOTAL       | 3,160,273,551           |           |                          |                      |                             |                           | 7106 B                     |

*Target audience (7-21 years old people) was estimated by multiplying [all people count](https://population.un.org/wpp/Download/Standard/MostUsed/) on a fraction of [0-14 yo people](https://www.theglobaleconomy.com/rankings/percent_children/) for 2021 year. We assume that in near future it's a good approximate of 7-21 yo group.*

*Teacher wage data in was collected from [salaryexplorer.com](http://www.salaryexplorer.com/?loc=23&loctype=1&job=123&jobtype=3#browsesalaries) on 2023.01.08*