
Zur Abgabe:

Sei A die Adjazenzmatrix von G und ai,j = {$a_{1,1},a_{1,2},a_{n,n}$}
L = {$a_{1,1},a_{1,2},a_{n,n}$ $\#$bin(k)}



Ein- / Ausgabeverhalten der universellen TM

=> Kodierung anhand der Gödelnummer 

Gödelnummer ist präfixfrei, fängt mit 111 an und hört mit 111
=> Wichtig, um zu entscheiden wann die Gödelnummer endet und das Wort anfängt



Alphabet (0,1,B) => Kodierbar
(qo = 0) => (q1,0,R)

qo = 0
0 = 0
$0^{1}10^{1}10^{3}10^{1}10^{3}$ 


### Tutoriumsaufgabe 1 (Gödelnummer)

$<M> = 111code(1)11code(2)11...code(n)111$ 
$x_{1}$ = 0, $x_{2}$ = 1, $x_{3} = B$ 


b) 

(i) Invertierung einer Gödelnummer = (i)
=> (i) ist eindeutig und präfixfrei, da hier die gleiche Kodierung gilt, nur dass 0 und 1 vertauscht sind

(ii) Nein, da die angegebene Kodierung nicht eindeutig und nicht präfixfrei ist

Eindeutigkeit durch Kodierung $0^{1 \cdot bin(i)} 1 bin(i)$ 
=> Wäre deutlich kleiner als die normale Kodierung

(iii) Nein, da die angegebene Kodierung nicht präfixfrei ist

### Tutoriumsaufgabe 2  (Palindrom mit 1 - Band TM)


Schritt 1: Falls Eingabe leer, terminiere mit JA
Schritt 2: Prüfe ob die Eingabe gerade Länge hat. Falls nein, terminiere mit NEIN. Falls ja, bewege den Kopf ganz von links, wieder zum ersten Symbol der Eingabe
Schritt 3) Speicher ob das aktuelle Symbol 0 oder 1 im Zustand und ersetze es durch ein B
Schritt 4) Lauf zum Ende der Eingabe und verleiche das dort gepeicherte mit dem im Zustand gespeicherte Symbol.
Schritt 5) Lauf gegen --- und geh in Schritt 1

Schritt 1 = 1
Schritt 2= 2n
Schritt 3= 1
Schritt 4 = n
Schritt 5= n

$\mathcal{O} (n) *n = \mathcal{O} (n^{2})$  
Ein Durchlauf vom Algorithmus  ist in nO(n) nur n Wiederholungen, daher folgt füe Laufzeit $\mathcal{O} (n^{2})$. Da die TM nur auf den Speicherzellen der Eingabe (plus die 2 Speicherzellen, die die Eingabe ) arbeitet, ist der Speicherbedarf $\mathcal{O} (n)$ 


### Tutoriumssaufgabe 3 (RAM für den Zweierlogarithmus)


Idee: Berechnung des Zweierlogarithmus und vergleiche ob das n  ergibt.

$2^0 = 1 n = 2^0 ?, 2^1 = 1, n = 2^1?$ 

Pseudocode

i = 0, j = 1

while(j $\leq$ n) {

i = i+1;
j = j $\cdot$ 2
}
return i-1


1. CLOAD 0
2. STORE 2
3. CLOAD 1
4. STORE 3
5. $ while
6. LOAD 3
7. SUB 1
8. IF C(0) > 0 GOTO end
9. CLOAD 1
10. ADD 2
11. STORE 2
12. CLOAD 3
13. CMULT 2
14. STORE 3
15. GOTO while
16. $ end
17. LOAD 2
18. CSUB 1
19. STORE 1
20. END