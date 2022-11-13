---
aliases: [Hoare, Hoare-Kalkül, Hoare-Tripel, partielle Korrektheit]

tags:
- Programmierung
---


Das Hoare-Kalkül ist ein Beweis, um zu zeigen, dass ein Programm syntaktisch korrekt ist, und partiell korrekt ist


#### Hoare-Tripel $<\phi > P < \psi >$ 

- $< \phi >$ ist die Vorbedingung, diese gilt von Anfang an
- P sei das Programm, was ausgeführt wird
- $< \psi >$ ist die Nachbedingung, diese gilt nach Ablauf des Programms
$\Rightarrow$ Wenn $< \phi >$ gilt, dann muss nach dem Ablauf des Programmes $< \psi>$ gelten.

Dafür gibt es verschiedene Arten von Kalkülen, um dies zu beweisen.

