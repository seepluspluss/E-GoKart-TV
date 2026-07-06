# 🛠️ Mechanische Spezifikationen & Fahrzeug-Geometrie

Diese Dokumentation enthält alle relevanten Maße, Geometriedaten und technischen Anforderungen für den Umbau des Rimo-Leihkarts auf einen Torque-Vectoring-Doppelantrieb.

---

## 📐 1. Fahrzeug-Abmessungen & Spurweiten
* **Gesamtbreite des Karts:** `1125 mm`
* **Gesamtlänge (Bumper zu Bumper):** `1680 mm`
* **Radstand (Achse zu Achse):** `1310 mm`
* **Spurweite Vorne (Reifenaußenkante):** `965 mm`
* **Spurweite Hinten (Reifenaußenkante):** `1140 mm`
  * *Konstruktions-Notiz:* Die breite Spur hinten (`1140 mm`) bietet zusammen mit den breiten Hinterreifen (`230 mm`) massiven mechanischen Grip. Das Torque Vectoring wird hier extrem effektiv arbeiten können, um das Kart agil in die Kurve zu zwingen.

---

## ⚙️ 2. Hinterachse & Wellenmaße
* **Außendurchmesser der Achse:** `30,11 mm`
  * *Bedeutung:* Kartsport-Präzisionswelle mit leichtem Übermaß.
  * *Konsequenz:* **Keine Standard-Industriekugellager bestellen!** Ausschließlich Kartsport-Lager (z. B. Typ GSH 30 RRB) verwenden. Aluminium-Naben (für Riemen und Bremse) müssen ggf. minimal ausgeschliffen werden.
* **Sicherung:** 4x **zweiteilige (geteilte) Wellenklemmringe** aus brüniertem Stahl verwenden.

---

## 🛑 3. Bremssystem (Spiegelung für geteilte Achse)
* **Bremsscheibendicke:** `7,07 mm` (Sollmaß: `7,00 mm`)
  * *Konsequenz:* Der zusätzliche Bremssattel und die neue Scheibe müssen zwingend für die Rimo-typischen **7 mm Dicke** ausgelegt sein.
* **Hydraulik:** Ansteuerung beider Sättel via 3-Wege-T-Stück über das originale Bremspedal.

---

## ⚡ 4. Antrieb & Riemen-Geometrie (Aktueller Ist-Zustand)
Aus den Messungen lässt sich das aktuelle Übersetzungsverhältnis und der Bauraum für den Doppelantrieb ableiten:

* **Hinterreifen-Breite:** `230 mm` pro Seite.
* **Heck-Bumper-Breite (Halterung/Schutz):** `108 mm`.
* **Bereits vorhandener Zahnriemen:**
  * *Breite:* `38,47 mm` (Sehr massiver, breiter Riemen für hohe Drehmomente).
  * *Durchmesser (Großes Rad):* `170 mm`.
* **Motor-Riemenscheibe (Zahnrad klein):**
  * *Zähnezahl:* 28 Zähne.
  * *Außendurchmesser:* `69,37 mm`.
  * *Breite:* `38 mm`.
  * *Mindestdurchmesser Welle:* `21,9 mm`.

---

## 🪑 5. Sitz & Bauraum für Elektronik/Akkus
* **Sitzbreite Oben:** `535 mm`
* **Sitzbreite Unten:** `555 mm`
* **Abstand Haltestangen (Sitzstreben):** `380 mm`
  * *Bedeutung:* Der Raum zwischen den hinteren Sitzstreben (`380 mm`) und unter der Sitzschale ist der primäre Montageort für das neue mittlere Achslager sowie die geschützte Unterbringung eurer NXP-ECU-Box.

---

## 📋 Letzte offene Messung vor der Bestellung
* [ ] **Bremsscheiben-Lochkreis:** Anzahl der Schrauben und Lochabstand (wird für die Bestellung der spiegelverkehrten Bremsscheibenaufnahme benötigt).
