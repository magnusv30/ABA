# Anleitung für Implementierung von Code in Google Colab
Für dieses Projekt kann Google Colab sehr gut verwendet werden, es muss nichts auf dem PC installiert werden. Es wird lediglich ein Browser und ein Google-Konto benötigt. Außerdem ist Google Colab gratis. 
## 1 Anmeldung auf Google Colab und Herunterladen des Projkets von Github
[https://colab.research.google.com/](https://colab.research.google.com/) öffnen und mit dem Google Konto anmelden.
Außerdem erst auf [mnist-1](https://github.com/magnusv30/ABA/blob/d338cde66c7138177eeb85f9b5b7caa984ce8e08/MNIST-1.ipynb) klicken und rechts oben auf herunterladen klicken, um das Projekt später auf Colab auszuführen.
## 2 Hochladen des Projekts
Wenn man sich dann in Google Colab angemeldet hat, erscheint folgendes Fenster:
<img width="451" height="350" alt="Screenshot Colab Notebook öffnen" src="https://github.com/user-attachments/assets/22bc97dd-0860-4b3e-8dd6-bfa1219e1ec8" />
Hier dann auf "Hochladen" klicken und auf "Durchsuchen". Dann die Datei, die im vorherigen Schritt heruntergeladen wurde, auswählen. 
## 3 Hochladen des MNIST-Trainingsdatensatzes
Um den MNIST-Trainingsdatensatz in Google Colab hochzuladen, muss dieser zuerst über [mnist_train.csv](https://python-course.eu/data/mnist/mnist_train.csv) heruntergeladen werden. Um den Datensatz für den Code erreichbar zu machen, muss dieser in Google Colab in Dateien hochgeladen werden. Dazu links auf das Ordner-Symbol klicken <img width="43" height="115" alt="Ordner Symbol Colab" src="https://github.com/user-attachments/assets/1d0b92d0-c3d4-415d-a1d8-23352939f731" /> und bei den drei Punkten rechts von sample_data auf Öffnen klicken. Hier dann links oben auf "Hochladen" <img width="137" height="38" alt="image" src="https://github.com/user-attachments/assets/88182c23-7ea9-449a-8f55-e99c34873523" /> und die Datei mnist_train.csv auswählen. Dieser Prozess kann etwas dauern.
## 4 Verorten der Trainingsdatensatzes im Code
Um den Speicherort des Trainingsdatensatzes dem Programm bekannt zu geben, muss der bestehende Pfad verändert werden. Hierzu neben mnist_train.csv auf die drei Punkte klicken und auf "Pfad kopieren" klicken und im Code den Ausdruck "data/mnist_train.csv" durch den kopierten Pfad ersetzen.

