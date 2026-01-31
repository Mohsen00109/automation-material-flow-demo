Project 1 – TIA Portal Simulation with Factory I/O

Overview
Dieses Projekt ist ein simulationsbasiertes Automatisierungsprojekt, um industrielle Steuerungskonzepte mit dem Siemens TIA Portal zu entwickeln und zu testen.
Das Projekt dient als praxisnahe Demonstration von SPS-Logik, Materialflusssteuerung und HMI-Integration.

---

Technologies
- Siemens TIA Portal (STEP 7)
- HMI Engineering
- Factory I/O
- PLC Simulation

---

Scenario Description
Das Szenario bildet eine automatisierte Produktions- und Lagerlinie ab.
Rohteile werden zufällig in drei Farbvarianten (Grün, Blau, Grau)in das System eingespeist.
Nach der Bearbeitung im Machining Center werden farbabhängige Deckel aufgesetzt und verpresst.

---

Process Flow
Nach dem Fügen der Bauteile übernimmt ein Pick-and-Place-System die Sortierung der Werkstücke.
Ein separates Two-Axis-Pick-and-Place-System verteilt die Teile auf drei Förderlinien:
- Grün → erste Linie
- Blau → mittlere Linie
- Grau → separate Linie
Anschließend erfolgt die farbgetrennte Palettierung.

---

Data Handling (RFID / Data Blocks)
Jede Palette wird mit einer eindeutigen RFID-Box-ID versehen.
Die ID wird vom Steuerungssystem gelesen und in einem Data Block gespeichert, um Palettenstatus und Lagerposition nachvollziehbar zu verwalten.

---

Stacker Logic
Die fertig palettierten Einheiten werden in einem Hochregallager (Stacker-System) eingelagert.
Zusätzlich ist eine Unload-Funktion implementiert, bei der der Stacker zufällig belegte Lagerplätze auswählt und Paletten automatisch entlädt.

---

Project Status
Dieses Projekt befindet sich in kontinuierlicher Weiterentwicklung.
Der aktuelle Stand stellt eine funktionsfähige Basis dar, die schrittweise um weitere Funktionen, Optimierungen und Dokumentation erweitert wird.

---

Notes

Dieses Projekt basiert vollständig auf einer Simulation und enthält keine realen Kunden-, Anlagen- oder Firmendaten.


