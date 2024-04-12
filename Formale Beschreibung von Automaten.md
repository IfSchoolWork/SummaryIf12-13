[[Automaten]] werden duch bis zu 7 Komponenten beschrieben

![[007_Automat.svg]]

Man beginnt damit zu beschreiben welche der 7 Komponenten genutz werden. Z.B. ein Akzeptor (keine Ausgabe) benötigt nur 5/7 Komponenten

AK = {Σ, A, Q, Q0, QE, δ, α}

###### endliche Menge der Eingabesymbole:
Σ = {0,1,2,3,4,5,6,7,8,9}
###### endliche Menge der Ausgabesymbole:
A = {Nichts gefunden, 0 gefunden, 00 gefunden, kein 007, 007 gefunden, 007 bereits gefunden}

###### endliche Zustandsmenge:
Q = {Nothing, 0, 00, 007}
###### Anfangszustand:
Q0 = Nothing

###### endliche Menge der Endzustände:
QE = {007}

###### Zustandsübergangsfunktion:
δ = Q x Σ -> Q

| <br>Q╲Σ <br> | 0       | 7       | 1,2,3,4,5,6,8,9 |
| ------------ | ------- | ------- | --------------- |
| Nothing      | 0       | Nothing | Nothing         |
| 0            | 00      | Nothing | Nothing         |
| 00           | Nothing | 007     | Nothing         |
| 007          | 007     | 007     | 007             |

###### Ausgabefunktion:
α = Q x Σ -> A

| <br>Q╲Σ <br> | 0                    | 7                    | 1,2,3,4,5,6,8,9      |
| ------------ | -------------------- | -------------------- | -------------------- |
| Nothing      | 0 gefunden           | Nichts gefunden      | Nichts gefunden      |
| 0            | 00 gefunden          | kein 007             | kein 007             |
| 00           | kein 007             | 007 gefunden         | kein 007             |
| 007          | 007 bereits gefunden | 007 bereits gefunden | 007 bereits gefunden |



