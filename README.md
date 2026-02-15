# MNIST Neuronales Netz mit Jupyter - Anleitung zur Verwendung des Blogs
Neuronales Netz zur Ziffernerkennung (MNIST) mit Jupyter, Numpy, Matplotlib und Pandas.

## 1: Nur Code
Um zu starten, beginne bei folgendem Dokument, es erklärt den Code für das Projekt:
[Projekt mit Erklärung](https://github.com/magnusv30/ABA/blob/3089c31152b6a0d6d64a790f2974ee9670e74251/MNIST-1.ipynb)
(In diesem Code wurde eine andere Version des Backpropagation-Algorithmus verwendet, der einfacher zu programmieren ist)
## 2: Der Code ausgeführt zum Verständnis, was passiert
Anschließend ist es ratsam, sich anzusehen, wie das Programm von oben aussieht, wenn es ausgeführt wurde. Dadurch kann man viel besser verstehen, was passiert ist. [Ausgeführter Code](https://github.com/magnusv30/ABA/blob/3089c31152b6a0d6d64a790f2974ee9670e74251/MNIST%201.1%20-%20ausgef%C3%BChrt.ipynb)
  
## 3: Vergleich von zwei verschiedenen Backpropagation-Algorithmen
Eine Alternative Implementierung von Backpropagation, die Google NotebookLM basierend auf [3blue1brown](https://www.3blue1brown.com) geschrieben hat. [Alternatives Backpropagation](https://github.com/magnusv30/ABA/blob/3089c31152b6a0d6d64a790f2974ee9670e74251/mnist-2%20alternatives%20Backpropagation.ipynb)
  
## 4: Analyse der Performance
Hier wird die Performance im Lauf der Zeit analysiert und verschiedene Kombinationen von Wiederholungen und Lernraten ausprobiert. [Analyse der Performance](https://github.com/magnusv30/ABA/blob/86a138ea6a4b12fdeba7a3f4f7827119d833fe10/Analyse%20der%20Performance.md)
  
# Eigene Implementation
Nun kann das Programm selbst auf dem eigenen Rechner bzw. auf Google Colab ausgeführt werden. Einfach der [Anleitung](http://htmlpreview.github.io/?https://github.com/magnusv30/ABA/blob/3089c31152b6a0d6d64a790f2974ee9670e74251/Anleitung%20Google%20Colab.html) folgen.
  
# Nächster Schritt: handgeschriebene Buchstaben erkennen!
Der nächste Schritt wäre, den Datensatz von MNIST auf EMNIST umzustellen und den Code dementsprechend zu verändern. EMNIST ist ähnlich wie MNIST, nur besteht es aus handgeschriebenen Buchstaben. Die Architektur müsste nur in der letzten Schicht zu 62 Neuronen erweitert werden (je 26 Klein- und Großbuchstaben und 10 Ziffern). Der EMNIST-Datensatz ist auf [Kaggle](https://www.kaggle.com/datasets/crawford/emnist/data) verfügbar - hier einfach emnist-letters-train.csv herunterladen und wie in der Anleitung oben den Pfad verändern. 
Hierfür einfach den Pfad in der zweiten Code-Zeile ändern. Außerdem müssen die Größeen der letzten Gewichtsmatrix und Biasmatrix von 10 auf 26 vergrößert werden und in der Code-Zelle, in der der Gradientenabstieg definiert wird nach der folgenden Zeile:  
    w1,b1,w2,b2,w3,b3=matrizen_erstellen()  
    folgender Code hinzugefügt werden, damit das Programm noch laufen kann:  
    label=label-1  
Dann kann der Code eigentlich schon laufen. Jedoch wäre es gut, wenn noch mindestens eine Schicht hinzugefügt wird und zu jeder Schicht ein paar mehr Neuronen, damit das Netz besser funktioniert.
