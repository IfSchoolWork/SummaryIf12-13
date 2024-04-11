Basiert auf einem [[RS-Latch]] bei dem die Eingänge nicht R und S sonder D und !D und somit voneinander abhängig sind. Damit wird der verbotene Zustand verhindert.

![[D_Latch.svg]]

<table border = 1>
<tr><th>D</th><th>Q t</th><th>!Q t</th></tr>
<tr><td>0</td><td>0</td><td>1</td></tr>
<tr><td>1</td><td>1</td><td>0</td></tr>
</table>

Ein D-Latch verliert allerdings auch den Speicherzustand eines [[RS-Latch]], weshalb es um eine [[Clock]] erweitert werden kann.

![[D_Latch_Clock.svg]]

<table border = 1>
<tr><th>Cl</th><th>D</th><th>Q t</th><th>!Q t</th></tr>
<tr><td>0</td><td>0</td><td>Q t-1</td><td>!Q t-1</td></tr>
<tr><td>0</td><td>1</td><td>Q t-1</td><td>!Q t-1</td></tr>
<tr><td>1</td><td>0</td><td>0</td><td>1</td></tr>
<tr><td>1</td><td>1</td><td>1</td><td>0</td></tr>
</table>

Bei einem D-Latch mit [[Clock]] lässt sich zwar festlegen wann etwas gespeichert werden soll, allerdings tritt ein Problem auf wenn man versucht in einem D-Latch mit dem Output X versucht !X zu speichern, da man hier sehr prezise timen müsste wann man die Clock an und ausschaltet, damit kein zweites Mal der Wert des D-Latches überschrieben wird. Dieses Problem wird durch einen [[D-FlipFLop]] gelößt.