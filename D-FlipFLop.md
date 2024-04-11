Ein D-FlipFLop ist ein [Komplexer Baustein](<Komplexe Bausteine>), welcher aus 2 [D-Latches](D-Latch) besteht und damit das Problem des [D-Latches](D-Latch) behebt, dass man ohne prezises timen des an- und ausschaltens der Clock keine auf dem Output des [D-Latches](D-Latch) basierenden Werte im selben [[D-Latch]] speichern kann.

![[D-FlipFlop.svg]]
Die Speicherung in einem D-FlipFlop ist [[Flankengetriggert]]. Das heißt dass sich der Output zu dem Zeitpunkt ändern bei dem die Clock auf 0 geht -> negative Flanke.