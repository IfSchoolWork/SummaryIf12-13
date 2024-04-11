Ein RS-Latch ist ein [Komplexer Baustein](<Komplexe Bausteine>) der aus zwei NAND-Gates besteht und bei dem der Output nicht nur von den Inputs sonder auch vom letzten Output abhängen kann.

![[RS_Latch.svg]]

<table border = 1>
<tr><th>R</th><th>S</th><th>Q t</th><th>!Q t</th></tr>
<tr><td>0</td><td>0</td><td>1</td><td>1</td></tr>
<tr><td>0</td><td>1</td><td>0</td><td>1</td></tr>
<tr><td>1</td><td>0</td><td>1</td><td>0</td></tr>
<tr><td>1</td><td>1</td><td>Q t-1</td><td>!Q t-1</td></tr>
</table>

Durch die Abhängigkeit vom vorherigen Zustand entsteht ein Speicherzustand R=1, S=1. Es entsteht allerdings auch ein Verbotener Zustand R=0, S=0 da in diesem Q t = !Q t gilt.