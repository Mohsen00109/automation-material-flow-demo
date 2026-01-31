Project 2 – Industrial Automation & IIoT Architecture Demo

Dieses Projekt stellt eine simulationsbasierte Referenzarchitektur für moderne Industrieautomatisierung und IIoT-Systeme dar.
Der Schwerpunkt liegt nicht auf der reinen SPS-Programmierung, sondern auf der ganzheitlichen Betrachtung eines Automatisierungssystems bestehend aus Steuerung, Kommunikation, Datenverarbeitung und Visualisierung.

---

Projektidee

Ziel dieses Projekts ist es, eine realitätsnahe industrielle Systemarchitektur aufzubauen, wie sie in modernen Produktionsanlagen eingesetzt wird. Dabei werden klassische Automatisierungskonzepte mit modernen IT- und IIoT-Technologien kombiniert. Das Projekt dient als technische Demonstration und persönliches Engineering-Portfolio.

---

Grundszenario

Das zugrunde liegende Szenario bildet eine automatisierte Produktions- und Lagerlinie ab.
Rohteile werden zufällig in unterschiedlichen Farbvarianten in dasSystem eingespeist, bearbeitet, sortiert, palettiert und anschließend in einem Hochregallager zwischengespeichert.


---

Systemarchitektur – Überblick

Die Architektur ist bewusst mehrschichtig aufgebaut und folgt dem Prinzip der funktionalen Entkopplung.

Steuerungsebene
- TwinCAT als zentrale Steuerungsplattform
- Simulation der Hauptprozesse und Bewegungsabläufe

Ergänzende Logikebene
- CodeSys zur nicht sicherheitskritischen Datenverarbeitung
- Vorbereitung von Alarm- und Zustandsinformationen

Kommunikationsebene
- OPC UA für strukturierte Prozessdaten
- TCP/IP für systemübergreifende Kommunikation
- MQTT als leichtgewichtige IIoT-Schnittstelle

Daten- und Serviceebene
- Node-RED zur Datenaufbereitung und -verteilung
- SQL-Datenbank zur Speicherung historischer Daten

Visualisierungsebene
- Web-Dashboard
- perspektivisch Ignition

---

Datenfluss

1. Prozessdaten entstehen in der Steuerungsebene
2. Über OPC UA werden relevante Variablen bereitgestellt
3. Node-RED übernimmt Filterung, Strukturierung und Logik
4. Daten werden über MQTT verteilt
5. Speicherung erfolgt in einer SQL-Datenbank
6. Visualisierung und Alarmierung greifen auf diese Daten zu

---

Alarm- und Überwachungskonzept

Ein zentrales Ziel ist der Aufbau eines flexiblen Alarmsystems:
- Ereignisbasierte Alarme
- Priorisierung
- Zeitstempelung
- Quittierung
- Historische Auswertung

Ein Teil der Alarmverarbeitung wird bewusst (passiv) umgesetzt,um reale Industriearchitekturen mit entkoppelten Services abzubilden.

---

Bewegungs- und Achssimulation

Zur Erhöhung des Realitätsgrades werden virtuelle Achsen implementiert. Die Bewegungssteuerung erfolgt über speziell entwickelte

Funktionsbausteine mit:
- klar definierten Zuständen
- separaten Bewegungsmodi
- strukturierter Fehlerbehandlung

Ziel ist eine möglichst realitätsnahe Abbildung industrieller Achssysteme.

---

Projektstatus

Dieses Projekt befindet sich(in aktiver Entwicklung).
Der aktuelle Stand bildet eine stabile technische Basis, die schrittweise um weitere Funktionen erweitert wird, darunter:
- erweiterte Alarmkonzepte
- zusätzliche Visualisierungen
- Performance-Optimierung
- erweiterte Datenauswertung

Regelmäßige Updates sind geplant.

---

Hinweis

Dieses Projekt basiert vollständig auf einer Simulation.
Es enthält keine realen Kunden-, Anlagen- oder Firmendaten und dient ausschließlich Demonstrations-, Lern- und Entwicklungszwecken.

