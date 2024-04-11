Atomare Werte sind Werte die sich nicht weiter aufteilen lassen.

![1. Normalform](assets/images/1NF.png)

z.B. Straße kann in Straßenname und Hausnummer aufgeteilt werden, weshalb es kein Atomarer Wert ist

#### Probleme Nichtatomarer Werte:
<ul>
<li>Das bearbeiten der Daten ist umständlicher, da innerhalb des Feldes gearbeitet werden muss</li>
<li>Daten können eventuell nur in einem weniger effizienten Datentyp gespeichert werden. Hausnummer könnte als Integer gespeichert werden, muss aber in Verbindung mit Straße als String gespeichert werdem</li>
</ul>