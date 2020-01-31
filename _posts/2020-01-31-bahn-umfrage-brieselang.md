---
layout: post
title: "Bahn Umfrage Brieselang"
date: 2020-01-31
---

Was Daten und Computer messen, ist das eine. Aber was empfindet der Mensch, wenn er der Technik ausgeliefert ist? Die Deutsche Bahn lässt dazu etwa einmal im Jahr Umfragen durchführen. Befrager fahren dazu im Zug mit und stellen den Reisenden meist Fragen über ihre Reisegewohnheiten. Sowas wird dann von der [VBB](https://www.vbb.de/unsere-themen/qualitaet/qualitaet-im-regio/meine-linie-rb14) grob zusammengefasst veröffentlicht.
Aber wie sieht die Qualität der Maschine für den Menschen tagtäglich und individuell aus? Also wie empfindet jeder Reise persönlich seine tägliche Fahrt zur Arbeit oder Schule mit der Bahn? Dazu wurde die App [Bahnumfrage Brieselang](https://play.google.com/store/apps/details?id=com.eumelnet.bahn.spreadsheetinput) entwickelt:

![App Foto](https://lh3.googleusercontent.com/sXK6AOztnvVXNWQkr2qxcoNJeQQdduVLjEI8o6Kx82LG63QaRp8jWNmn2RH-rMkkLw=w1440-h620 "App Foto")

Die Bedienung ist sehr einfach gehalten und kann sofort nach Zustieg im Zug ausgefüllt werden:

**Datum/Uhrzeit**

Hier sollte beim Starten der App die aktuelle Uhrzeit angezeigt werden. Bei Bedarf kann man die Angaben ändern, wenn man zun Beispiel erst später die Zugreise bewerten will.

**Fahrtrichtung**

Es gibt bloss zwei Richtungen: Richtung Nauen oder Richtung Berlin

**Pünktlichkeit**

Wie wird die Pünktlichkeit des Zuges bewertet (1=schlecht, 5=sehr gut)

**Platzangebot**

Wie ist das Platzangebot des Zuges? Also ist der Zug vollständig oder fehlen Wagen? (1=schlecht, 5=sehr gutes Platzangebot)

**Auslastung**

Wie ist der Zug durch Reisende ausgelastet? Ist es Modell "Sardinenbüchse" (1=schlecht) oder findet man bequem Platz (5=sehr gut)

Zum Schluss die entscheidene frage, bei der es nur Ja oder Nein gibt:

**Reise akzeptabel**

Also kann man die Fahrt als solche akzeptieren oder findet man die Reise als unausstehlich?


Die gesammelten Daten werden wieder durch [Tableau](https://public.tableau.com/profile/eumel#!/vizhome/bahnumfrage/Dashboard1) verarbeitet und grafisch aufbereitet. Für jeden Tag wird unter allen Bewertungen für jede Kategorie der Mittelwert gebildet. Der bestmögliche Wert ist **5**, entsprechen den 5 Sternen in der App.

Die Akzeptanz kennt nur Ja oder Nein. Hier werden alle Bewertungen in der Totale gezählt und prozentual ausgegeben. Die [App für Android](https://github.com/eumel8/trainqa/tree/master/android) findet man im Trainqa-Verzeichnis. Mitentwickler sind willkommen.
