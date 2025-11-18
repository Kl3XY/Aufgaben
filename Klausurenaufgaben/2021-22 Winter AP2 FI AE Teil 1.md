## Compilersprachen
Compiler gehen durch den gesamten code durch und kompilieren den anschließend in Maschinencode um eine separate Executeable zu erstellen. Schnellere Executable, fehler werden im vorraus angezeigt aber dafür ist der compileprozess länger.

Beispiele:
C,
C++,
Rust,
C#

## Interpreter
Interpreter übersetzen und führen den Code aus während es aktiv läuft. Initiale compile zeit ist schneller dafür ist das programm langsamer.

Beispiele:
Python,
Javascript,
PHP

## Bibliotheken
Bibliotheken sind eigene Projekte die von Drittpersonen angeboten werden welche kernaspekte eines Projektes bereits erledigt haben. Diese ersparen Unmengen an viel zeit jedoch können auch schadsoftware enthalten oder sogar komprimiert sein. Oder sogar auf veralteter, nicht mit neusten standard kompatible, software basieren.

## Dokumentation
Bei der Ansprache von "Dokumentation" wird hiermit das Kommentieren der Klassen gemeint.
Konstruktor Kommentieren, Methoden Kommentieren und bla bla
![[Pasted image 20251118113316.png]]

## Versionsverwaltung
Versionsverwaltungssoftware (wie z.B. Git) dokumentiert und behält den Verlauf der Versionen von der Software woran die Versionsverwaltungssoftware angeklebt wurde.
Versionsverwaltungssoftware basiert auf Repositories, in den meisten fällen gibt es ein Lokales und ein Remote Repository. Das Lokale befindet sich immer in deinem PC während das Remote sich auf einem Server meistens befindet. Ein Repository beeinhält den Quellcode der jetzigen version sowie auch die Historie der vergangen Versionen.

Es ist meist ne gute idee ein VVS zu haben einfach nur um Fuck ups zu vermeiden.

## Anwendungsfalldiagramm
![[Pasted image 20251118125947.png]]
Ich habe das schon ein paar dutzend male erklärt in diesem Obsidian doc. Hier ist ein bild.

## ER Modell / Relationale Datenbankmodell

#### ER-Modell
![[Pasted image 20251118130039.png]]

Relationales-Datenbankmodell (ER-Diagramm auch genannt)
![[Pasted image 20251118130134.png]]

## Barrierefrei
Ein Programm, oder andere art von Medie, so gestalten das selbst Menschen mit beeinträchtigungen das Programm verwenden können.

Beispiele:
Farbfilter
Text-to-Speech ausgaben
Audioerklärung
Einfache Sprache

## UML-Klassendiagramm
ist unter [[02-02]] erklärt worden
## HTTP Errors
#### 404
Der Angegebene URL oder Pfad innnerhalb eine Domain wurde nicht gefunden
#### 403
Der Nutzer hat nicht ausreichend rechte um diesen Inhalt anzugucken
#### 500
Generischer fehler
#### 501
Nicht Implementierte funktion.
## Symmetrische Verschlüsselungen
Eine Verschlüsselungsart wo beide seiten, Client und Server den selben Key benutzen um zu Enkodieren und Dekodieren

## Asymmetrische Verschlüsselungen
nutzen ein Public und Private key. Der Public Key verschlüsselt die Daten und kann Digitale Signuren die vom Privaten Schlüssel kommen überprüfen. Der Private entschlüsselt daten und kann Digitale Signaturen erstellen und validieren.

## Programm Signaturen
Programme müssen signiert werden um offiziell von Windows als Sicher anerkannt zu werden.
Um das Programm zu evaluieren kann der Programmierer das Programm zu Microsoft schicken um ein Viren und Malware test durchzuführen um das Programm zu evaluieren oder eine Valuating License kaufen um es zu umgehen.

Es ist auch möglich eine Code-Signatur in den Einstellungen des Compilers einzustellen.

## Effizienz und Änderbarkeit

Änderbarkeit beschreibt wie leicht es ist ein Programm zu erweitern ohne viele Fehler aufzurufen

Effizienz beschreibt das Zeitliche Verhalten des Programmes und wie Optimal es läuft. (Etwas was spiele heutzutage gekonnt ignorieren.)

## Automatische Code Reviews und Unit Tests
Wie der Name sagt das sind Automatisierte versionen der einzelnen Test-Verfahren. Jedoch ist hierbei etwas sehr dumm da sie oftmals immernoch menschlichen input benötigen und daher die ersparrte zeit recht gering ist.
Bei Unit Tests muss trotzdem einem entwickler erzählt werden was genau er machen soll.


## Black Box Tests
Tests ohne zu wissen wie das Programm intern aussieht

## White Box tests
Tests mit dem Wissen wie das Programm intern aussieht.