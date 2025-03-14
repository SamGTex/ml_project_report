# Segmentierung von Gewässern auf Satellitenbildern

**Projektarbeit** im Rahmen des Kurses: Maschinelles Lernen für Physiker*innen

**Partner:** Nico Guth [@NicoJG](https://github.com/NicoJG)

**Code:** Das Projekt wurde mithilfe der Deep-Learning Python-Bibliothek Tensorflow durchgeführt und das neuronale Netz auf Google Colab trainiert.

# Methode
Convolutional Neural Network (**CNN**) mit U-Struktur

<img src="https://github.com/SamGTex/ml_project_report/blob/main/content/img/u-net-architecture.png" alt="drawing" width="600"/>

Quelle: [O. Ronneberger, P.Fischer und T. Brox. „U-Net: Convolutional Networks for Bio-medical Image Segmentation“](http://lmb.informatik.uni-freiburg.de/Publications/2015/RFB15a.)

# Ergebnisse
<pre>
        Input                      Maske                Ergebnis CNN            Ergebnis RF
</pre>

<img src="https://github.com/SamGTex/ml_project_report/blob/main/content/img/ergebnisse_gut.png" alt="drawing" width="800"/>

©Mapbox ©OpenStreetMap

# Alternativ-Methode
Random Forest (**RF**) und Informationen über den Gradienten.

# Datensatz
**Input:** Satellitenbild

**Output:** Maske mit Gewässern

Der mithilfe der Mapbox- und OpenStreetMap-API generierte Datensatz beinhaltet ca. 58.000 Satellitenbilder.
Zu jedem Satellitenbild gehört ein Maskenbild, welches vorhandene Gewässer anzeigt.
Jeder in der Karte eingezeichnete Punkt stellt ein Satellitenbild dar.
Der Datensatz repräsentiert also den europäischen Kontinent.

![map][map]

[map]: https://github.com/SamGTex/ml_project_report/blob/main/content/img/map.png "Map"



