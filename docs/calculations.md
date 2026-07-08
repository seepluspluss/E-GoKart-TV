# 🧮 Physikalische Berechnungen & Antriebsauslegung

Diese Übersicht dient zur Berechnung von Übersetzung, Drehmoment und Endgeschwindigkeit für den Torque-Vectoring-Antrieb.

---

## 🏎️ 1. Aktuelle Getriebe-Spezifikationen

| Parameter | Symbol | Gemessener Wert | Formel / Quelle |
| :--- | :---: | :---: | :--- |
| **Zähnezahl Achse (Groß)** | $Z_2$ | **83** | Messung |
| **Zähnezahl Motor (Klein)** | $Z_1$ | **15** | Messung |
| **Übersetzungsverhältnis** | $i$ | **5,5333** | $i = Z_2 / Z_1$ |
| **Reifendurchmesser hinten**| $D$ | *ca. 260 mm* | Noch exakt zu messen |
| **Reifenumfang** | $U$ | **0,817 m** | $U = \pi \cdot D$ |

---

## ⚡ 2. Performance-Simulation (Soll-Werte mit B&R Motor)

Sobald Herr Tutzer uns die exakten Motordaten (Nenndrehzahl und Drehmoment) schickt, tragen wir sie hier ein, um die echte Performance zu berechnen.

| Parameter | Formel für Excel | Wert (Beispiel 4.500 U/min) | Status |
| :--- | :--- | :---: | :--- |
| **Max. Motordrehzahl** | *Herstellerangabe* | **9.000 U/min** | Wartet auf B&R |
| **Max. Achsdrehzahl** | `=Motordrehzahl / i` | **813,25 U/min** | Berechnet |
| **Top-Speed (Theorie)** | `=(Achsdrehzahl * U * 60) / 1000` | **39,58 km/h** | Berechnet |
| **Nenndrehmoment Motor**| *Herstellerangabe* | *tbd Nm* | Wartet auf B&R |
| **Drehmoment an der Achse**| `=Motordrehmoment * i * 2` | *tbd Nm* | (Für beide Motoren) |

---

## ⚙️ Excel-Formel-Spickzettel für das Team

Wenn du die Tabelle in Excel nachbaust, nutze diese Logik für die Zellen (Beispiel):
* **Zelle A1:** `4,500` (Motordrehzahl)
* **Zelle A2:** `5,5333` (Übersetzung)
* **Zelle A3:** `0,817` (Reifenumfang in Metern)
* **Formel für km/h in Zelle A4:** `=(A1 / A2 * A3 * 60) / 1000`

---

## 📌 Erkenntnis für die Konstruktion
Sollte die Endgeschwindigkeit bei der Simulation mit über **90 km/h** zu hoch sein, bedeutet das im Umkehrschluss, dass uns beim Beschleunigen wichtiges Drehmoment fehlt. In dem Fall müssten wir das motorseitige Ritzel ($Z_1$) von 28 Zähnen auf z. B. 15 oder 18 Zähne verkleinern, um eine kürzere, giftigere Übersetzung zu bekommen.



🔗 [Hier geht es zur Live-Excel-Berechnung (Google Sheets)](https://docs.google.com/spreadsheets/d/1rTTlmsxOaWPoelF8dfGwfKrU060xiymMCltuo6tPZT8/edit?usp=sharing)
