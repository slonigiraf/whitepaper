# GIRAF - legislation for communities

_Denis Reshetov / E-mail:_ [_reshetovdenis@gmail.com_](mailto:reshetovdenis@gmail.com) _/ Telegram:_ [_@denisreshetov_](https://t.me/denisreshetov)

## Annotation
This paper proposes an approach on how to use the established practice of writing laws to coordinate people in small groups so that they can jointly create documents whose content is economically beneficial to them.

## Что такое "закон"
The laws have been known since the beginning of human civilization. As the exact definition of the term "law" is debatable, we will use the following: a law is a set of instructions that people have agreed to follow, and also oblige to follow. Examples of what we understand by laws include: the Bill of Rights (USA); article on DNA on Wikipedia; history schoolbook; the balance of a specific bitcoin wallet.

| Legislator | Law | Why is it the law | How to fix |
| ----------- | ----------- | ----------- | ----------- |
| US Congress | Bill of rights (USA) | can be achieved through the court of their rights | pay a lot of money to legislators (lobby) |
| Wikipedia | article about DNA | is used as a standard of truthful information in society | make edits yourself and convince other editors |
| Schoolbook author | history textbook | used in schools to teach children | bribe the author and publisher |
| Bitcoin | balance of a specific bitcoin wallet | it is possible to pay with this balance | spend a lot of money (perform a 51% attack) |

## How laws are written
Law writing is linked to economic activities, for example, US congressional campaigns for politicians are [funded by lobbyists](https://en.wikipedia.org/wiki/Lobbying_in_the_United_States) who push for legislation to improve their well-being; editors of Wikipedia articles either contribute their time, which is a valuable asset, or may receive funding from a group of individuals who are interested in advancing their point of view; and the miners of the Bitcoin network take money for changing the balances of wallets.

There are cases when a foreign country changes the laws of another country, spending money on it.

It can be argued that the purchase of laws (lobbying) is a generally accepted global norm, and the law itself is a commodity that can be bought and sold. Lobbying is an important tool for creating consensus in society, and leads to economic well-being (see US lobbying practices).

редакторы статей на Википедии либо тратят свое время, которое является ценным активом, либо могут получать финансирования от группы лиц, которая заинтересована в продвижении [своей точки зрения](https://en.wikipedia.org/wiki/Wikipedia:Edit_warring); а майнеры сети Bitcoin [берут деньги](https://bitcoin.org/bitcoin.pdf) за изменения балансов кошельков.

Известны случаи, когда зарубежная страна изменяет законы другой страны, [тратя на это деньги](https://www.reuters.com/article/politicsNews/idUSN2450753720071024).

Можно утверждать, что покупка законов (лоббирование) является общепринятой мировой нормой, а сам закон является товаром, который можно купить и продать. Лоббирование является важным инструментом создания консенсуса в обществе, и ведет к экономическому благополучию (см. практику лоббирования в США).

## Прямая демократия и законы
Издание законов важно для координации людей, однако, в небольших проектах его использование проблематично: оно неповоротливо и требует наличия большого количества игроков: избирателей, законодателей и лоббистов.

Я предлагаю решение, как использовать законодательство и лоббирование для координации людей в маленьких группах, чтобы они могли совместно создавать документы, содержание которых экономически выгодно для них:

- любой человек может опубликовать новый закон, указав сколько денег он добровольно раздает остальным членам группы
- любой человек может отменить опубликованный закон, раздавая столько же денег, сколько его создатель
- раздача денег при создании закона происходит в пропорциональной схеме: член группы, у которого больше денег, получает больше, чем тот у которого денег мало.

Раздача денег - это лоббирование обращенное к группе людей. Когда человек раздает свои деньги, он "покупает закон", а, как мы выяснили, "покупка законов" - это устоявшаяся тысячелетями рабочая практика законодателства.

Пропорциональная схема раздачи денег нужна для поддержания рыночных стимулов. Если раздавать всем поровну, то неизбежно появятся люди, которые живут на деньги от раздачи, но сами при этом ничего не создают полезного для общества.

Раздача денег и регистрация законов на данный момент удобно может быть реализована в виде блокчейн-приложения, потому что такой подход позволяет честно вести передачу денег, а также вести открытый реестр законов.

## Архитектура приложения

Я предлагаю общую архитектуру системы для создания и лоббирования законов. Каждая запись в базе данных должна содержать в себе:

- уникальный идентификатор закона, например его порядковый номер
- хэш текста закона, например, cid текста закона в [системе IPFS](https://ipfs.tech/)
- количество денег, розданнных при создании закона

Хэш текста - это строчка длинной в несколько десятков букв, например хэш-[cid](https://docs.filebase.com/ipfs/ipfs-cids) имеет длинну 46 букв. Если в текст закона добавить хотя бы одну дополнительную точку, то хэш получится кардинально другим. Нам нужны хэши законов, чтобы в целях экономии места хранить текста закона не на блокчейне, а в [системе IPFS](https://ipfs.tech/), и при этом не подвергаться опасности, что текст кто-то незаметно перепишет.

Раздача денег может быть осуществлена путем уменьшения баланса кошелька создателя закона и пропорционального увеличения балансов кошельков остальных людей, либо путем "сжигания" названной суммы с баланса кошелька создателя закона. Эти подходы [эквиваленты с точки зрения экономики](https://www.coindesk.com/learn/what-does-it-mean-to-burn-crypto/), т.к. "сжигание" ведет к повышению ценности оставшихся денег, кроме того "сжигание" является более простой вычислительной операцией на блокчейне.