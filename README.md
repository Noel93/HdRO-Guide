# HdRO-Guide

## Einleitung

Hier möchte ich meinen persönlichen Versuch dokumentieren, sämtliche Quests und Taten in Herr der Ringe Online (HdRO) / Lord of the Rings Online (LotRO) aufzulisten. Dies ist vor allem aus dem Wunsch entstanden, solche Quests nicht mehr zu verpassen, welche unter Umständen nicht mehr verfügbar sind, bspw. wenn man andere Quests erfüllt. Auch soll sich ein "natürlicher Flow" ergeben, durch den man möglichst effizient durch die Gebiete spielen kann, während man parallel sämtliche Aufgaben dort erfüllt, um den inneren Completionist zufriedenzustellen.

## Aufbau

### Dateien

Die Dateien repräsentieren jeweils ein Gebiet und sind entsprechend aufsteigend durchnummeriert. Die Reihenfolge entspricht dabei grob der Reihenfolge, in der Gebiete im Zuge der epischen Questreihe besucht werden - also im Normalfall der Reihenfolge, in der Gebiete releast wurden, mit Ausnahme von später eingeführten Low Level Gebieten wie z.B. die Fernen Auen, welche anhand der geografischen Nähe einsortiert wurden. 

Ab Moria gibt es Gebiete, die zusätzlich in Unter-Gebiete unterteilt sind. Dies wird in der Reihenfolge durch ```X.1```, ```X.2``` usw. repräsentiert. So ergibt sich eine Zuordnung von Questlog-Kategorien zu Dateien: ```Moria```-Quests kommen in ```15) Moria.txt```, Quests der Kategorie ```Die Großbinge``` in ```15.1) Moria - Die Großbinge.txt```.

Ausnahmen sind ```00) Ortsunabhängig.txt```, wo Quests aufgeführt sind, die bspw. durch Levelup oder per Postnachrichten verfügbar sind, und ```01) Einleitung.txt```, welches die Intro-Quests der verschiedenen Völker auflistet, die nur in der anfänglichen Intro-Instanz angenommen werden können.

### Dateiinhalt

Die einzelnen Dateien beginnen mit dem Namen der Questlog-Kategorie und der Level-Range des Gebiets, bspw. ```Trum Dreng (65-66)```. 

Anschließend beginnt die Auflistung der Quests des Gebiets. Diese können zur Übersichtlichkeit in Abschnitte aufgeteilt sein, bspw. nach Quest-Hub. Einzelne Abschnitte können optional eine Überschrift besitzen (z.B. Name des Quest-Hubs bzw. des Quest-Gebiets). Beziehen sich alle Quests des Abschnitts auf eine Quest-Kategorie, die nicht der Bezeichnung in der ersten Zeile der Datei entspricht, muss dies ebenfalls in der Abschnitt-Überschrift dargestellt werden, z.B. ```("Scharmützel") Die Belagerung von Gondamon```.

Einzelne Quests haben das Format ```Level Name Repeatable-Flag```, wobei die möglichen Flags ```(R)``` für wiederholbare Quests und ```(R3)``` bzw. ```(R5)``` für die limitiert wiederholbaren Quests sind. Gehört die Quest zu einer anderen Quest-Kategorie als in der ersten Zeile der Datei steht und besitzt der Abschnitt keine entsprechende Quest-Kategorie in der Überschrift, muss die Kategorie vor der Quest dargestellt werden, bspw. ```("Zentrum von Gondor: Nieder-Lebennin") 100 Das Dunkel im Osten```. Hinter der Quest wird der Questgeber genannt, mit ```(Name, Koordinaten)```. Bei Quests mit nicht eindeutigem Questgeber, z.B. mehrere Objekte oder Gegner in einem Bereich oder Landschaftsquests, wird dies mit ```um XY``` und beispielhaften oder mittig gelegenen Koordinaten dargestellt. Gibt ein Questgeber mehrere Quests (mit keinen oder den exakt gleichen Voraussetzungen), werden diese kommasepariert aufgelistet, mit den Daten des Questgebers hinter der letzten Quest, bspw. ```20 Jagdauftrag: Groß genug für einen Läufer (R), 20 Jagdauftrag: Perfekt gekringelt (R) (Sonja Landei, 22.3S,44.0W)```.

Folgen auf eine oder mehrere Quests eine oder mehrere andere Quests, wird dies mit ```X -> Y``` gezeigt. Dies bedeutet immer, dass ```Y``` exakt ```X``` als Voraussetzung(en) hat, nicht mehr und nicht weniger. Hat ```Y``` hierbei den selben Questgeber / Quelle wie ```X```, wird dieser nicht erneut nach der Quest aufgeführt. Hat ```Y``` andere Voraussetzungen (bspw. neben ```X``` noch ```Z```), muss dies gesondert in einer neuen Zeile aufgeführt werden.
Mögliche Voraussetzungen sind hierbei:
- ```Nach X: Y``` für Quests, die aufeinander folgen, ohne dass dies durch ```->``` dargestellt werden kann (z.B. weil sie räumlich getrennt sind oder ```X``` zu einer längeren Questreihe gehört, während ```Y``` nur eine optionale Nebenquest darstellt).
- ```Nach A, B und C: Y``` für Quests, die den Abschluss mehrerer anderer Quests erfordern, ohne dass dies durch ```->``` dargestellt werden kann.
- ```Nach Annahme von X: Y``` für Quests, die nach der Annahme einer anderen verfügbar werden.
- ```Nach X Objective #Z: Y``` für Quests, die nicht sofort nach Annahme, aber im Verlauf einer anderen verfügbar werden.
- ```Während X: Y``` für Quests, die nur während einer anderen Quest verfügbar sind. Wichtig: nur, wenn ```X``` nicht ohne ```Y``` abgeschlossen werden kann, also z.B. eine Wrapper-Quest!
- ```Nur während X: Y``` für Quests, die nur während einer anderen Quest verfügbar sind, aber für deren Abschluss nicht relevant sind und somit verpasst werden können!
- ```Nur bis Abschluss von X: Y``` für Quests, die nicht mehr verfügbar sind, wenn eine andere abgeschlossen wurde.

Taten sind nach Art kategorisiert, hauptsächlich ```Erkundungstaten``` und ```Bezwingertaten```, welche ggf. am Anfang eines Abschnitts über den Quests platziert werden und als durch ```-``` getrennte Auflistungen von erkundbaren Orten, Gegnertypen o.ä. in Kombination mit den Koordinaten dargestellt sind.
Bspw.
```
Aerthir
Erkundungstat (Hata Kebir, 84.2S,37.6W - Lager der Schatten, 82.5S,37.6W - Pelagir, 83.0S,34.8W)
Bezwingertat (Haradrim und Halbtrolle, um 84.6S,36.7W)
... Quests ...
```

## Anmerkungen

Es wird lange Zeit ein Work in Progress verbleiben, da ich den Guide parallel zu meinem aktuellen Playthrough erstelle und nach diesem vermutlich länger keinen neuen starten werde. An hdro-guide@outlook.de können gerne Korrekturen, Verbesserungsvorschläge etc. gesendet werden!

Aktuell befindet sich alles in Textformat. Falls jemand eine übersichtlichere Alternative (z.B. Flowcharts für die Questreihen?) kennt, welche alle Use Cases abbilden kann, dann den Vorschlag ebenfalls gerne an obige Mail senden.

Shoutout geht raus an die Entwickler des LotRO Companion Tools (https://sourceforge.net/projects/lotrocompanion/), welches enorm bei der Erfassung der Voraussetzungen einzelner Quests hilft.