

---
aliases: [Zahlen, komplex, Zahlenmengen]

tags:
- Analysis_fuer_Informatik
---




Die komplexen Zahlen bilden eine Zahlenmenge.
Diese erweitert die reellen Zahlen. Dies ist keine Erweiterung im Sinne der Verdichtung oder Linksseitigkeit von Zahlenmengen, sondern bildet  einen Erweiterungskörper der reellen Zahlen.



### Idee der komplexen Zahlen

Im Bereich der reellen Zahlen findet man Probleme, die keine Lösung in den reellen Zahlen haben.

Beispiele sind:

- $x^2 +1 = 0$ 
- $x^3 -15x - 4 = 0$

Für das Beispiel $x^2 + 1 = 0$ gilt $x^2 = -1$ . Jedoch $\nexists x \in \mathbb{R} : x^2 = -1$ . Man braucht also eine neue Art von Zahlen, um diese Gleichung zu lösen. Also definiere man eine Zahl $i$ mit $i^2 = -1$. So existiert die Lösung $x^2 = i^2$ und damit $x = \pm i$. Diese Zahl $i$ wird als imaginäre Einheit bezeichnet.


### Definition der komplexen Zahlen 

Die Menge der komplexen Zahlen $\mathbb{C}$ haben folgende Eigenschaften:

- Die rellen Zahlen liegen in den komplexen Zahlen, also ist jede reelle Zahl eine komplexe Zahl
- In den komplexen Zahlen gilt das Kommutativ-, Assoziativ- und das Distributivgesetz.
- Für jede komplexe Zahl $z$ existiert eine komplexe Zahl $-z$, sodass $z + (-z) = 0$ gilt
- Für jede von 0 verschiedene komplexe Zahl $z$ existiert eine komplexe Zahl $\frac{1}{z}$ , sodass $z \cdot \frac{1}{z} = 1$  gilt
- Es existiert eine komplexe Zahl $i$ mit der Eigenschaft $i^2 = -1$ .
- Der Bereich der komplexen Zahlen ist minimal zu den oben genannten Eigenschaften, also muss jede komplexe Zahl als $z = a + bi \mid a,b \in \mathbb{R}$ darstellbar sein

### Darstellung von komplexen Zahlen

Eine komplexe Zahl wird meistens in der Form z = a + bi angegeben, wobei a, b $\in \mathbb{R}$ und i die imaginäre Einheit darstellt. Für den Fall b = 0 stellen die komplexen Zahlen die reellen Zahlen dar. 


### Konjugation von komplexen Zahlen

Sei $z = a + bi$ , dann existiert eine komplexe Zahl $\bar{z} = a -bi$ . $\bar{z}$ wird dann die Konjugation / die Konjugante von $z$ genannt.


### Arithmetik komplexer Zahlen

Mit komplexen Zahlen können arithmetische Rechenschritte dargestellt werden. Wir betrachten im Folgenden die komplexen Zahlen $z_1$ = a + bi und
$z_2$ = c + di.

#### Addition von komplexen Zahlen

Für die Zahlen $z_1$ und $z_2$ ist $z_1 + z_2$ definiert als : $z_1 + z_2 = (a+bi) + (c+di) = a+ bi+c+di = a+c +bi +di = (a+c) + i \cdot (b + d)$
Wie man sieht, addiert man jeweils den Real- und  Imaginärteil der jeweiligen Zahlen miteinander. 



#### Subtraktion von komplexen Zahlen

Für die Zahlen $z_1$ und $z_2$ ist $z_1 - z_2$ definiert als : $z_1 - z_2 = (a+bi) - (c+di) = a+ bi-c-di = a-c +bi -di = (a-c) + i \cdot (b - d)$
Wie man sieht, subtrahiert man jeweils den Real- und  Imaginärteil der jeweiligen Zahlen miteinander. 



#### Multiplikation von komplexen Zahlen

Für die Zahlen $z_1$ und $z_2$ ist $z_1 \cdot z_2$ definiert als : $z_1 \cdot z_2 = (a+bi) \cdot (c+di) = ac + adi + bci + bdi^2 = (ac -bd) + i \cdot (ad + bc)$
Man mltipliziert jeden Term aus und fasst diese zusammen. Man bedenke $i^2 = -1$ und fasst Real- und Imaginärteil zusammen



Da dieser Körper keine Ordnung besitzt, können komplexe Zahlen nicht verglichen werden, d.h. die Operatoren <,> existieren nicht in den komplexen Zahlen. 

#### Division von komplexen Zahlen

Für die Zahlen $z_1$ und $z_2$ ist $\frac{z_1}{z_2}$ definiert als : $\frac{z_1}{z_2} =  \frac{(a + bi)}{(c + di)} = \frac{(a + bi)(c-di)}{(c + di)(c-di)} = \frac{(ac -adi +bci - bdi^2)}{c^2 - (di)^2}$ 
$= \frac{(ac + bd) + i (bc -ad)}{c^2 - d^2 i^2} = \frac{(ac + bd) + i (bc -ad)}{c^2 + d^2} = \frac{ac+bd}{c^2 + d^2} + i \frac{bc-ad}{c^2 + d^2}$.
Wie man sieht, erweitert man mit der Konjuganten von $z_2$ und fasst Real- und Imaginärteil zusammen.