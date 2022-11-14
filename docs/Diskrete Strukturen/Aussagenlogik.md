---
aliases: []

tags:
- Analysis_fuer_Informatik
- Diskrete_Strukturen
---

## Aussagen 

#### Definition
>Eine Aussage oder sprachlicher Ausdruck kann entweder wahr oder falsch sein.

#### Beispiele
- Es ist heute warm
- Es gibt unendlich viele Primzahlen
- Heute fällt die Vorlesung aus



## Zusammengesetzte Aussagen

#### Definition
>Aussagen können logisch miteinander verknüpft werden.
Dabei hängt der Wahrheitswert von zusammengesetzten Aussagen von der logischen Struktur und der Wahrheitswerte der Einzelaussagen ab. Diese können in einer sogenannten Wahrheitstabelle dargestellt werden.

#### Beispiele
- Es ist warm und sonnig
	$\Rightarrow$ Es ist warm
	$\Rightarrow$ Es ist sonnig
- Wenn es regnet, dann sind die Straßen nass
	$\Rightarrow$ Es regnet.
	$\Rightarrow$ Die Straßen sind nass.


#### Wahrheitstabelle
In der Wahrheitstabelle schreiben wir 0 für den Wahrheitswert falsch und 1 für den Wahrheitswert wahr

| A   | B   | $\lnot$A | A $\land$ B | A $\lor$ B | A xor B | A $\rightarrow$ B | A $\Leftrightarrow$ B |
| --- | --- | -------- | ----------- | ---------- | ------- | ----------------- | --------------------- |
| 0   | 0   | 1        | 0           | 0          |   0      |   1                |           1            |
| 0   | 1   | 1        | 0           | 1          |   1      |   1                |           0            |
| 1   | 0   | 0        | 0           | 1          |   1      |   0                |           0            |
| 1   | 1   | 0        | 1           | 1          |   0      |   1                |           1            |



#### Verknüpfung von Aussagen

| Art                   | Name                           | Notation                                                                  | Aussage                                                 |
| --------------------- | ------------------------------ | ------------------------------------------------------------------------- | ------------------------------------------------------- |
| Negation              | Verneinung                     | $\lnot$A                                                                  | Ist genau dann wahr, wenn A falsch ist                  |
| Konjugation           | UND - Verknüpfung              | A $\land$ B                                                               | Ist genau dann wahr, wenn sowohl A als auch B wahr ist  |
| Disjunktion           | ODER - Verknüpfung             | A $\land$ B                                                               | Ist genau dann wahr, wenn mindestens A oder B wahr ist  |
| Exklusive Disjunktion | EXKLUSIVE - ODER - Verknüpfung |A xor B| Ist genau dann wahr, wenn genau einer der beiden Wahrheitswerten wahr ist |                                                         
| Subjunktion           | WENN - DANN - Verknüpfung      | A $\rightarrow$ B                                                         | Ist genau dann falsch, wenn A wahr ist und B falsch ist |
| Bijunktion                      |         GENAU - DANN - Verknüpfung                       |   A $\leftrightarrow$ B                                                                       | Ist genau dann wahr, wenn A und B den gleichen Wahrheitswert besitzen                                                         |


## Alphabet der Aussagenlogik


#### Definition

Das Alphabet der Aussagenlogik besteht aus:

- Variablen (A, B, C, ..)
- Konstanten (0, 1)
- Symbole ($\lnot , \land , \lor , \rightarrow , \Leftrightarrow$)
- Klammern ( '(' , ')' )

Hieraus können Wörter gebildet werden. Variablen und Konstanten sind Wörter. Für ein Wort A und ein Wort B können wir folgende Wörter konstruieren:

- ($\lnot A$)
- (A) $\land$ (B)
- (A) $\lor$ (B)
- (A) $\rightarrow$ (B)
- (A) $\leftrightarrow$ (B)

Diese bilden dann [[Logische Terme]]