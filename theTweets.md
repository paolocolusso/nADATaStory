---
layout: page
title: The Words
subtitle: Looking into the 140 characters.
---

If, as we claim, Russian trolls aim at spurring political instability in Europe, it is natural that they should focus on disruptive events showing the weaknesses of our society. Also, they would be likely to touch upon themes that are key in the political agenda of populist parties (*Leaugue* and *Five-Star Movement*), making Europe more frail and threatening the stability of international relationships. They would naturally encourage political debate, creating divisiveness in the country.

What we see is indeed that they are more active during periods coinciding with peaks of terrorism in Europe, migratory crisis and political events.


### Content analysis
We now delve into the content of tweet themselves, starting by a general overview. Which words are occurring the most? 

![](../img/word1.png){: .align-center}

Italian readers will notice that most of the words are names of **newspapers** and news agencies, with a peculiarity: it is hard to spot the the presence of radical papers. *la Repubblica* is the best selling Italian paper, followed by *Corriere della Sera* and *La Stampa*, while *ANSA* is the main press agency. Although *la Repubblica* is rather centre-left wing, all of these are generally perceived to be as moderate and reliable by the majority of the population: this is probably also the impression trolls want to give.

If we now exclude papers and press agencies from the cloud, a clearer picture emerges: politics is clearly on top when it comes to favourite topics for trolls. 

![](../img/word2.png){: .align-center}

If we look at **national politics**, all the themes which have determined the results of the most recent elections are there: *migrants*, *Europe*, *security*. The name of the main parties is also present, together with some leaders' name. Although *Renzi* and *Democartic Party*, *PD*, are of larger size than their political opponents, other parties are more represented in terms of political priorities: *migrants* and *security* are the main target of the *League*, for example. Taking a further look at the output of the word cloud, one will notice that words associated to the *PD* crisis feature highly (corruption scandals, internal fight for the leadership of the party...).

Shifting to **international politics**, Trump is the big name. More generally, the words mainly refer to the weaknesses of the European Union: **terror attacks**, **Brexit**, the **common currency**... The lexicon seem to be dominated by negative words, which conveys the idea of the current situation in Europe being doomed. But there is more to it. Except for Germany and France, the countries mentioned have one common feature: they are ruled by authoritarian leaders: **Turkey** (Erdogan), **Syria** (Assad), **Russia** (Putin). Of course, a similar idea holds for **Trump**, which is typically perceived as strong and tough, especially in terms of migration. Also, notice that Syria is the one of the main interests of the Russian foreign politics.

Laslty, words as **fear**, **terror**, **risk**, **terrorism**, **massacre**, **attack** clearly want to stress a situation of instability.

It is hardly surprising that Russia would try to provide a negative picture of our institutions: lack of faith in traditional parties and institutions has already lead towards increased success of populist parties all across Europe, making it weaker. All of this creates sympathy towards more authoritative figures, like Putin and Trump, who present themselves as strong in defending their country's interests.

### Words often appearing together
We now use data mining, and specifically association rules, to confirm some intuitions.

In Italian politics there is a big difference from the traditional Democratic Party, who is associated to its internal fights and scandals, and the populist Five-Star Movement, who often goes together with references to the official blog of the party.


| Antecedent   | Consequent     | Confidence    |
| :---         |     :---:      |          ---: |
| elections    | pd             | 0.888889      |
| consip       | renzi          | 0.297297      |
| grillo       | m5s            | 0.272727      |
| grillo       | blog           | 0.265152      |


International politics is again dominated by the big leaders: interestingly, Trump is associated with Putin. Notice also that there is a frequent association between Macron and Lepen, whose political story somewhat mirrors that of Renzi and Salvini.


| Antecedent   | Consequent     | Confidence    |
| :---         |     :---:      |          ---: |
| lepen        | macron         | 0.790698      |
| putin        | trump          | 0.290909      |
| missiles     | syria          | 0.586207      |


As we were noticing, trolls never cease to stress instability: Stockholm, for instance, gets matched with the truck which caused a massacre in the 2017 terror attack.

| Antecedent   | Consequent     | Confidence    |
| :---         |     :---:      |          ---: |
| westminster  | london         | 0.763636      |
| stockholm    | truck          | 0.392857      |
| at least     | deaths         | 0.394958      |
| deaths       | injured        | 0.201258      |


