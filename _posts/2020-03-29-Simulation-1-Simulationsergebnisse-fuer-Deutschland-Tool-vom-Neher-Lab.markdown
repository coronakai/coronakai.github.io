---
layout: post
title:  "Simulation 1: Simulationsergebnisse für Deutschland (Tool vom Neher Lab)"
date:   2020-03-29 10:00:00 +0200
categories: Simulationen
---
Heute zeige ich einige Simulationsergebnisse für Deutschland, die ich mit Hilfe des Modells der Arbeitsgruppe des Physikers Prof. Dr. Richard Neher der Uni Basel (Biozentrum) erstellt habe (https://neherlab.org/covid19/). Zwei Anmerkungen möchte ich vorher machen:

1. `Modelle idealisieren immer ein System.` Inwieweit ein Modell etwas vorhersagen kann, muss immer sehr kritisch hinterfragt werden. (Man denke an Wettermodelle und die Genauigkeit der Vorhersagen des Wetters in einer Woche.) Daher: Alle Ergebnisse, die ich zeige, sind grundsätzlich fehlerbehaftet. Sie können höchstens eine Ahnung davon geben, was uns noch bevorsteht. Zudem habe ich das Modell nicht selber kalibriert, sondern mich weitestgehend auf die vorgegebenen Parameterwerte bzw. auf Werte des RKI verlassen. In nächster Zeit wird unsere Arbeitsgruppe ein eigenes Modell kalibrieren und verschiedene Szenarien berechnen.

2. `Das Modell beruht auf Daten aus China, wenn es darum geht, wie viele erkrankte Menschen ins Krankenhaus eingewiesen, ggf. beatmet werden und wie viele davon prozentual sterben.` Es kann sein, dass der Virus mit der Zeit mutiert oder dass sich aufgrund der kommenden, wärmeren Jahreszeit der Verlauf der Erkrankung verändert.

Wer mehr über das zugrundeliegende Basismodell erfahren möchte, sollte sich unbedingt das Video auf [YouTube („Simulating an epidemic“ von 3Blue1Brown)](https://youtu.be/gxAaO2rsdIs) angucken.

**Parametrisierung des Modells**

Im Bild unten sind die Parameterwerte für meine Simulationen zu sehen. `Der wichtigste Wert, um eine ansteckende Krankheit zu beschreiben, ist die Basisreproduktionszahl R0. Diese gibt an, wie viele Menschen eine infizierte Person am Anfang einer Epidemie im Durchschnitt ansteckt. Bei CoViD-19 wird dieser Wert auf ca. 3 geschätzt (ohne Maßnahmen und ohne Herdenimmunität).` Anzumerken sei, dass sich die Anzahl der Intensivbetten mittlerweile auf ca. 28.000 erhöht hat. Die Zahl wird auch noch weiter steigen. Bei den Verläufen, die ich euch zeigen werde, hat jedoch selbst eine Verdopplung der Intensivbetten kaum Einfluss auf die Gesamtzahl der Verstorbenen. Zudem ist noch nicht klar, wie hoch die Dunkelziffer der Infizierten ist. Es lässt sich jedoch sagen, dass alles, was ich jetzt schreibe, laut Modellrechnung ca. einen Monat früher einsetzen würde, wenn die Dunkelziffer um den Faktor 10 höher läge als die festgestellte Zahl der Infizierten.

![Parameterwerte der Simulation](/assets/sim1/parameters.png)

**Keine Maßnahmen**

Wenn wir vor gut zwei Wochen nichts verändert hätten, würden wir das Maximum der Infiziertenzahl Ende Mai erreichen. Die Kapazitäten der Krankenhäuser wären von Anfang Mai bis Anfang August 2020 sehr stark überschritten. Außerdem würden mehr als 1.000.000 Menschen an CoViD-19 sterben.
Die Punkte geben den bisherigen Verlauf an: Grau: Gesamtzahl der Infizierten, Gelb: Zahl der in den vergangen drei Tagen Infizierten, Violett: Verstorbene.

![Transmissionsfaktor ohne Maßnahmen](/assets/sim1/nomitigation_transmission.png)
![Simulationsverlauf bei keinen Maßnahmen](/assets/sim1/nomitigation.png)

**Mittlere Maßnahmen**

Wenn wir die Ansteckungsrate bis mindestens zum Jahresende halbieren, wären die Krankenhäuser zwar immer noch überlastet—und das von Mai bis September, aber es würden nur ca. 500.000 Menschen sterben. Das Maximum der Ansteckungsrate wäre Ende Mai erreicht.

![Transmissionsfaktor bei mittelstarken Maßnahmen](/assets/sim1/mediummitigation_transmission.png)
![Simulationsverlauf bei mittelstarken Maßnahmen](/assets/sim1/mediummitigation.png)

**Starke Maßnahmen**

Wenn wir die Ansteckungsrate bis mindestens zum Jahresende um 90% reduzieren würden, wären die Krankenhäuser von Anfang Mai bis Ende Juni leicht überlastet. Am Ende könnten 120.000 Menschen an CoViD-19 gestorben sein. Das Maximum der Ansteckungsrate wäre Mitte Mai erreicht.

![Transmissionsfaktor bei starken Maßnahmen](/assets/sim1/strongmitigation_transmission.png)
![Simulationsverlauf bei starken Maßnahmen](/assets/sim1/strongmitigation.png)

**Starke Maßnahmen mit früher Lockerung**

Wenn wir die starken Maßnahmen lockern würden, so bald wir „über den Berg“ wären, könnte es passieren, dass am Ende wieder 500.000 Menschen stürben.

![Transmissionsfaktor bei starken Maßnahmen und früher Lockerung](/assets/sim1/strongmitigationendedearly_transmission.png)
![Simulationsverlauf bei starken Maßnahmen und früher Lockerung](/assets/sim1/strongmitigationendedearly.png)

**Diskussion**

`Welchen Effekt die Maßnahmen, die nun gelten, haben, können wir noch nicht aus den Daten ablesen. Die Latenz beträgt, so wie es im Moment aussieht, min. einen Monat.` Das wäre so, als würden wir das Wetter für morgen vorhersagen, aber erst übermorgen die Messwerte für Temperatur, Feuchtigkeit und Luftdruck erhalten, die wir für unsere Modelle benötigen. Daher noch einmal: Die Simulationsergebnisse sind sehr, sehr unsicher. Aber komplett falsch ist das Modell nicht, wie der bisherige Verlauf der Ausbreitung es beweist. Daher ist es umso wichtiger, dass wir uns längerfristig auf eine Kontaktvermeidung einstellen und diese bestmöglich umsetzen und hoffen, dass sehr bald ein wirksames Medikament oder eine Impfung gefunden wird.

Ich freue mich über Fragen und Anmerkungen dazu.