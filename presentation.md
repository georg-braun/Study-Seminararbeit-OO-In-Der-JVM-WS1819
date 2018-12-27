### Implementierung Objektorienterter-Konstrukte in der Java Virtual Machine


## Agenda
1. [Aufbau der .Class-Datei](#Aufbau der .Class-Datei)
2. [JVM Grundlagen: Stack & Heap](#JVM Grundlagen: Stack & Heap)
3. [Methodenaufrufe](#Methodenaufrufe)
4. [Konstruktor](#Konstruktor)
5. [Zugriff auf Felder](#Zugriff auf Felder)


## Aufbau der .Class-Datei

![](Grafiken/AufbauClassDatei.png)


## JVM Grundlagen: Stack & Heap


### Stack
- Pro Thread eigener Stack mit Frames
- Frame enthält:
  - Operanden-Stack
  - Array der lokalen Variablen
  - Referenz zum Runtime-Constant-Pool



### Heap

- Geteilter Bereich
- Speicher der Objekt-Daten
  - Über Referenz auffindbar
  - Sichern der Objekt-Daten
  - Referenz zur genutzten Klasse
- Method Area


#### Method Area

- Enthält Infos zu Klassen und Interfaces, Runtime-Constant-Pool, Methodentabellen, ...
- *__Runtime-Constant-Pool:__* Laufzeitrepräsentation der Constant-Pools (class-Dateien)
- *__Methoden-Tabelle:__* Aufrufbare Methoden



#### Beispiele: Zugriff auf die Klassen-Daten
![](Grafiken/ObjektReferenzKlasseVariante1.png)
![](Grafiken/ObjektReferenzKlasseVariante2.png)



#### Beispiel: Von der Objekt-Referenz zur Methode
![](Grafiken/LinkZurMethodenTabelle.png)




### Methodenaufrufe



### Konstruktor



### Zugriff auf Felder

