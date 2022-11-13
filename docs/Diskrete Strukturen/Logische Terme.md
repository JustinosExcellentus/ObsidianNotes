---
aliases: []

tags:
- Analysis_fuer_Informatik
- Diskrete_Strukturen
---


## Logische Terme

#### Definition

>Ein logischer Term bzw. eine aussagenlogische Formel ist ein sinnvoll aus dem Alphabet der [[Aussagenlogik]] zusammengesetztes Wort. Durch Belegung der Variablen mit Wahrheitswerten bekommt der Term selbst einen Wahrheitswert



#### Beispiele
- 0 $\land$ 1
- $\lnot (A \land B)$
- $A \land ( B \land (\lnot C))$


## Logische Äquivalenz und Tautologien


#### Definition
> Seien S und T logische Terme, definiert auf derselben Variablenmenge. Dann sind S und T **logisch äquivalent**, geschrieben S $\equiv$ T , wenn S und T denselben Wahrheitswert haben für jede Belegung der Variablen. T heißt **Tautologie** , wenn T $\equiv$ 1.


#### Beispiele

- $\lnot ( \lnot A) \equiv A$
- $A \rightarrow B \equiv \lnot A \lor B$ 
- $A \lor \lnot A$ ist eine Tautologie