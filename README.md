# Segmentierung von Gewässern auf Satellitenbildern

**Projektarbeit** im Rahmen des Kurses: Maschinelles Lernen für Physiker*innen

**Partner:** Nico Guth [@NicoJG](https://github.com/NicoJG)

# Methode
Convolutional Neural Network (**CNN**) mit U-Struktur
<img src="https://github.com/SamGTex/ml_project_report/blob/main/content/img/u-net-architecture.png" alt="drawing" width="600"/>

# Alternativ-Methode
Random Forest (**RF**) und Informationen über den Gradienten.

# Datensatz
**Input:** Satellitenbild

**Output:** Maske mit Gewässern

Der selbst generierte Datensatz beinhaltet über 50.000 Satellitenbilder mit Maske und deckt den europäischen Kontinent ab.
Jeder in Karte eingezeichnete Punkt stellt ein Satellitenbild dar.

![map][map]

[map]: https://github.com/SamGTex/ml_project_report/blob/main/content/img/map.png "Map"


# Ergebnisse
**
<pre>
        Input                      Maske                Ergebnis CNN            Ergebnis RF
</pre>
**
<img src="https://github.com/SamGTex/ml_project_report/blob/main/content/img/ergebnisse_gut.png" alt="drawing" width="800"/>
