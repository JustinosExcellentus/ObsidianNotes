
---
aliases: [Norm]

tags:
- Numerik_I
---

Definition

Ein Algorithmus heißt gutartig oder stabil, wenn die durch ihn im Laufe der Rechnung erzeugten Fehler in der Größenordnung des durch die Kondition des Problems bedingten unvermeidbaren Fehlers bleiben.

Kondition ist Eigenschaft des Problems,
Stabilität is Eigenschaft des Algorithmus

Wenn ein Prblem schlecht konditioniert ist, kann man nicht erwarten, dass eine numerische Methode (ein stabiler Algorithmus) ein besseres Ergebnis liefert.

Rückwärtsstabilität. Das Ziel (Relativer Fehler im Ergebnis) in Größenordnung eps ist zu ehrgeizig

Das Verfahren heißt rückwärts stabil, wenn
fsch(x) = f(xschl)
Für ein xsch mit relativem Fehler in der Eingabe in der Größenordnung der Maschinengenauigkeit

Ein rückwärts stabiler Algorithmus gibt die exakte Lösung des Problems mit nahezu richtigen Eingabedaten (d.h x = xsch = x(1+epsilon), |epsilos| \leq eps).

$\tilde{f}(x_{1},x_{2}, x_{3}) = ((x_{1} + x_{2}) (1 + \epsilon_{2} ) + x_{3} )(1+ \epsilon_{3})$ $\Rightarrow x_{1} (1+ \epsilon_{2})(1 + \epsilon_{3}) + x_{2} (1 + \epsilon_{2})(1 + \epsilon_{3}) + x_{3} (1 + \epsilon_{3})$ $\dot{=} \: x_{1} (1 + e_{2} + e_{3}) + x_{2} ( 1+ \epsilon_{2} + \epsilon_{3}) + x_{3} ( 1+ \epsilon_{3})$  
$= x_{1} ( 1+ \delta_{1}) + x_2(1 + \delta_{2}) + x_{3}(1+ \delta_{3})$ 
$= \tilde{x_{1}} + \tilde{x_{2}} + \tilde{x_{3}}$ 
f(x,y,z) = ((x+y)(1+ epsilon2) + x3) (1+ epsilon3)
=> x1 (1+e2)(1+e3) + x2(1+e2)(1+e3) + x3(1+e3)
=. x1(1+e2 + e3) + x2(1+e2+e3)+x3(1 + e3)
= x1(1+d1) + x2(1+d2) + x3(1+d3) 

d(2) \leq 2 eps
d(1) \leq 2 eps
d(3) \leq eps


Rückwärtsanalyse