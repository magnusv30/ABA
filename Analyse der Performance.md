# Analyse der Performance
## Intialisierung
Bei der Intialisierung des Codes fällt mir sehr stark auf, dass die Accuracy zu Beginn meist bei ziemlich genau 10% liegt, das heißt, dass das Netz wirklich keine Ahnung hat und zufällig die Ausgabe ausgibt. Dieser Wert schwankt meist zwischen 9 und 11%.

## Genauigkeitsrate
Um die Genauigkeitsrate etwas genauer zu analysieren, werden beide Programmiervarianten verglichen. Die x-Achse zeigt immer die Anzahl der Wiederholungen und die y-Achse multipliziert mit 100 die Genauigkeit.
Zu beginn starten beide Codes mit **1000** Wiederholungen und einer Lernrate von **0,1**:  
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
