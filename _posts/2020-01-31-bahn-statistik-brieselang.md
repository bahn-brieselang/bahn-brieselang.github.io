---
layout: post
title: "Bahn Statistik Brieselang"
date: 2020-01-31
---

Die Deutsche Bahn stellt über die Portale https://data.deutschebahn.com/ und https://developer.deutschebahn.com/ einige Schnittstellen zu Zug- und Fahrplandaten zur Verfügung. Für die Echtzeitauskunft gibt es die Portale https://mobile.bahn.de und https://reiseauskunft.bahn.de.
Diese Portale führen aber die Echtzeitinformationen nur in einem kurzen Zeitfenster an, etwa eine Stunde vor Abfahrt bis zur Ankunft des Zuges am Zielbahnhof. Dabei ist bei den Echtzeitinformationen zu unterscheiden zwischen Verspätung uns besondere Hinweise für den Zug.
Verspätungen werden bei der Deutschen Bahn unterteilt in Ankunftsverspätung, Abfahrtsverspätung und Verspätung für die gesamte Reise des Zuges. Da immer mehr Statistiken darüber geführt werden, und nicht bloss von der Bahn selber, ist das eher ein "weicher" Wert, bis 5 Minuten oder gar bis 15 Minuten gibt es gar keine Verspätung.
Besondere Hinweise bei einem Zug können sehr vielfältig sein. Zum einen sind das Verkehrstage, Informationen zur Wagenreihung oder fehlende Wagen. Auch nicht vorhandene behindertengerechte Einstiegshilfen finden Erwähnung. Es gibt aber keine einheitlichen Werte dafür.
Diese Informationen verarbeitet [schiene2.py](https://github.com/eumel8/trainqa/blob/master/apps/schiene2.py) aus dem [Trainqa](https://github.com/eumel8/trainqa) Projekt. Es werden stündlich Fahrplaninformation in Echtzeit abgerufen und abgespeichert.

[Tableau Public](https://public.tableau.com) ist ein Datenvisualisierungsdienst, der sehr grosse Verbreitung findet. Er spezialisiert sich auf die Verarbeitung von "Big Data". Auch unseres Trainqa-Daten werden dort verarbeitet und visualisiert. Auf dem [Trainqa Dashboard](https://public.tableau.com/profile/eumel#!/vizhome/trainqa/Dashboard1) findet man die zwei Tabellen:

* Verspätungen pro Tag: Hier wird die **Anzahl** der verspäteten Züge pro Tag gezählt, sofern dies von der Bahn gemeldet wurde
* Störungen pro Tag: Hier wird ebenfalls die **Anzahl** von Zugstörungen pro Tag gemeldet. Im Prinzip sind das die Meldungen "mehrere Wagen fehlen"

Eine automatische Datenbereinigung findet nur hinsichtlich doppelter Datensätze von Zugverbindungen statt. Das Feld für besondere Hinweise könnte noch weiter untersucht werden hinsichtlich genauerer Gründe für Störungen. 
