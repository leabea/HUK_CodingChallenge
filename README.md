# HUK_CodingChallenge

### Aufgabe im Rahmen der Coding Challenge:
Die Aufgabe besteht in der Modellierung der zu erwartenden Schadenhöhe pro Versicherungsnehmer und Jahr anhand der Risikomerkmale der Kunden.
Dieser Wert ist Basis für die Berechnung eines fairen Versicherungsbeitrags.

Dabei soll die folgende Struktur eingehalten werden:

* Explorative Datenanalyse: Sich mit dem Datensatz vertraut machen und Identifizierung möglicher Probleme sowie Erkennen grundlegender statistischer Zusammenhänge, welche für die anschließende Modellierung wichtig sein könnten.
  
* Feature Engineering: Aufbereitung der Variablen.
  
* Modellvergleich: Entscheidung für geeignetes Modell anhand einer dafür geeigneten Metrik. 
  
* Modellbuilding: Trainieren des gewählten Modell zur Vorhersage der erwarteten Schadenhöhe pro Kunde und Jahr. Ziel ist es, einen möglichst fairen Versicherungsbeitrag pro Jahr für einzelne Kunden anhand der Ihnen zu Verfügung stehenden Merkmale zu bestimmen. Dazu soll eine geeignete Metrik genutzt werden, um die Güte des finalen Modells zu beurteilen. Es soll gezeigt werden, welche Variablen und Zusammenhänge für das finale Modell relevant sind. Überlegung, wie das gewählte Modell weiter optimiert werden könnte.

### Datensatzbeschreibung:

1. freMTPL2freq:
* IDpol: ID des Vertrags
* ClaimNb: Anzahl Schäden im Versicherungszeitraum
* Exposure: Länge des Versicherungszeitraums (in Jahren) [Komponente der Zielvariable]
* Area: Area-Code des Versicherungsnehmers [unabhängige Variable]
* VehPower: Leistung des versicherten Kfz [unabhängige Variable]
* VehAge: Alter des versicherten Kfz [unabhängige Variable]
* DrivAge: Alter des Versicherungsnehmers [unabhängige Variable]
* BonusMalus: Schadenfreiheitsrabatt (französische Entsprechung der Schadenfreiheitsklasse)
[unabhängige Variable]
* VehBrand: Marke des versicherten Kfz [unabhängige Variable]
* VehGas: Antrieb des versicherten Kfz [unabhängige Variable]
* Density: Anzahl der Einwohner pro km2 im Wohnort des Versicherungsnehmers [unabhängige Variable]
* Region: Region des Versicherungsnehmers [unabhängige Variable]
  
2. freMTPL2sev:
* IDpol: ID des Vertrags
* ClaimAmount: Höhe der einzelnen Schadenaufwände (mehrere Einträge pro Vertrag, falls im Zeitraum mehrere Schäden vorhanden waren.) [Komponente der abhängigen Variable]
