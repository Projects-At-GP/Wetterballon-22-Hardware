# Wetterballon-22-Hardware

Datenlogger STRATO3 Specs

Parameter | Wert | Einheit
---|---|---
Eingangsspannung | 4,5 - 9 | Volt
Temperaturbereich (Bildschirm) | 0 to +85 | °C
Maximale Höhe (Sensor) | 50.000 | Meter
Druckbereich | 10 to 1200 | mbar
Luftfeuchtigkeit | 0 to 100 | %
Aufnahmerate | 0,5 | Hz
Temperatur-Messbereich ext. | -55 to +85 | °C
Temperatur-Messbereich int. | -40 to +85 | °C
Abmessungen | 85x54x10 | mm
Gewicht (ohne Batterie) | 50 | g
Gewicht (mit Batterie) | 94 | g
Laufzeit (bei 9V Li Batterie) | 24 | Stunden

Output string (also die Daten die er misst)
$;*Up-Time[hh:mm:ss]*;UTC[hh:mm:ss / NA];*Date[DD.MM.YYYY]*;RMC(GPS) Valid[bool];*Sats in Use[int]*;Latitude;*Longitude*;Speed over Ground[knots];*Speed over Ground[km/h]*;Course over Ground[°];*Altitude NN[m]*; Board: Temp[°C];*Extern: Temp[°C]*;Extern: Hum[%];*Extern: Press[hPa]*;Batt Voltage[V];*Logger Status*\r\n

Erklärung:  
Messwert | Bedeutung
---|---
Up-Time | Aktuelle Laufzeit
UTC | Koordinierte Weltzeit
Date | Datum
RMC Valid | Gültigkeit der GPS-Daten
Sats in Use | Anzahl der benutzten Sateliten
Latitude | Breitengrad
Longitude | Längengrad
Speed over Ground [knots] | Geschwindigkeit über Grund in Knoten
Speed over Ground [km/h] | Geschwindigkeit über Grund in km/h
Course over Ground | Kurs über Grund in Grad
Altitude NN | Höhe über NN
Board: Temp [°C] | Temperatur des Board-Sensors
Extern: Temp [°C] | Temperatur des externen Sensors
Extern: Hum [%] | Luftfeuchtigkeit des externen Sensors
Extern: Press [hPa] | Luftdruck des externen Sensors
Batt Voltage [V] | Batteriespannung
Logger Status | Logger Status für Fehlermeldungen
\r\n | newline escape string (windows)
