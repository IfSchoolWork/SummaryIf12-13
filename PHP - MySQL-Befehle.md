Befehle in der Programmiersprache [[PHP]] um [[MySQL]]-Queries auszuführen

<table border = 1>
<tr><th>Syntax</th><th>Funktion</th></tr>
<tr><td>$connection = mysqli_connect($host, $user, $passwd, $database); </td><td>Stellt eine Verbindung zu einer Datenbank her</td></tr>
<tr><td>$result = mysqli_query($connection, $query);</td><td>Führt eine SQL-Query aus und gibt das Ergebnis dieser zurück</td></tr>
<tr><td>$mysqli_close($connection, $query); </td><td>Schließt eine Verbindung zu einer Datenbank</td></tr>
</table>

