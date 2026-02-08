# Analyse der Performance
## Intialisierung
Bei der Intialisierung des Codes fällt mir sehr stark auf, dass die Accuracy zu Beginn meist bei ziemlich genau 10% liegt, das heißt, dass das Netz wirklich keine Ahnung hat und zufällig die Ausgabe ausgibt. Dieser Wert schwankt meist zwischen 9 und 11%.

## Genauigkeitsrate
Um die Genauigkeitsrate etwas genauer zu analysieren, werden beide Programmiervarianten verglichen. Die x-Achse zeigt immer die Anzahl der Wiederholungen und die y-Achse multipliziert mit 100 die Genauigkeit.
Zu Beginn starten beide Codes mit **1000** Wiederholungen und einer Lernrate von **0,1**:  
<table>
  <tr>
    <th>mnist-1</th>
    <th>mnist-2</th>
  <tr>
    <td><img width="547" height="413" alt="om, wh 1000, lr 0,1, insg 63,7" src="https://github.com/user-attachments/assets/859f88e4-c157-499f-9f50-aecaf4a95012" /></td>
    <td ><img width="556" height="416" alt="3b1b, wh 1000, lr 0,1, insg 25,8" src="https://github.com/user-attachments/assets/cdc78d74-b66c-47fd-9870-fb8b8f5bc40c" /></td>
  </tr>
  <tr>
    <td>Genauigkeit Testdatensatz: 63,7%</td>
    <td>Genauigkeit Testdatensatz: 25,8%</td>    
  </tr>
</table>
Hier man klar sehen, dass mnist-1 mit einer kleinen Lernrate und wenigen Wiederholungen bereits relativ gut auf dem Testdatensatz abschneidet. Außerdem fällt auf, dass beider in den ersten paar Wiederholungen sich wenig verbessern, anschließend sprunghaft und dann mit einer gleichmäßigen Steigung.


Als nächstes gibt es noch den Vergleich mit **5000** Wiederholungen und einer Lernrate von **0,2**.
<table>
<tr>
<th>mnist-1</th>
<th>mnist-2</th>
  </tr>
  <tr>
    <td><img width="547" height="413" alt="om, wh 5000, lr 0,2, insg 91,1" src="https://github.com/user-attachments/assets/5362a3e0-5904-4b36-9c4d-1f4228ea175d" />
</td>
    <td><img width="547" height="413" alt="3b1b, wh 5000, lr 0,2, insg 84,3" src="https://github.com/user-attachments/assets/7deac7b0-1894-4deb-b0ab-c52f5b3f08ce" />
</td>
  </tr>
  <tr>
    <td>Genauigkeit Testdatensatz: 91,1%</td>
    <td>Genauigkeit Testdatensatz: 84,3%</td>
  </tr>
</table>
Hier kann man ganz klar sehen, dass auch mnist-1 bei mehr Wiederholungen und einer höheren Lernrate deutlich besser performt. Außerdem fällt auf, dass nach einer gewissen Zeit bei beiden die Steigungen der Performance stark abflachen. Wenn man bei mnist-1 noch 2000 Wiederholungen mehr macht, verbessert sich die Performance auf dem Testdatensatz um etwas weniger als einen Prozentpunkt.</br> </br>
Außerdem kann es auch passieren, dass das Netz zwar anfangs sich in der Performance auf den Trainingsdaten verbessert, sich dann aber wieder verschlechtert: Dies ist mir bei mnist-2 mit 2000 Wiederholungen und einer Lernrate von 0,1 passiert:
<img width="556" height="413" alt="3b1b, wh 2000, lr 0,1, insg 33,8" src="https://github.com/user-attachments/assets/3ae2be64-ec15-4250-a83c-ff2d0c753ca5" />

# Verwendung von anderen Aktivierungsfunktionen
Um die Performance des Netzes mit anderen Aktivierungsfunktionen auch noch auszuprobieren, werden diese hier implementiert:
## Tanh-Aktivierungsfunktion




### Quellen
