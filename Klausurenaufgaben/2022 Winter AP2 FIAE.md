
## In- / Homogene IT infrastruktur
Dies bedeutet das alle Teile innerhalb der Infrastruktur von einem Hersteller kommen.

Vorteil:
Meistens erfolgt dann eine bessere Kommunikation zwischen den jeweiligen geräten

Nachteil:
Kann höhere kosten verlangen.

## Funktionale Anforderungen
Was das IT-Gerät konkret kann (Funktionen und Dienste). Also zum Beispiel: Ein Server welcher es ermöglicht den Mitarbeiter auf dessen Datenbank zuzugreifen.

Andere Beispiele:
Eine Firewall bietet Schutz von Internet traffic von aussen.
Eine Tastatur ermöglicht das interagieren mit dem Computer.
Ein Switch ermöglicht es die Anzahl der ports innerhalb eines Netzwerks zu erweitern.

## Nicht-Funktionale Anforderungen
Werte die von den Leistungen eines IT-Gerät ertragen werden. Zum Beispiel: Der neu errichtete Server erleichtert die Arbeit der Mitarbeiter um 49.6%!

Andere Beispiele:
Die Firewall verweigert 99.99% von meisten unübersehten Internet-traffic
Die Tastatur verschnellert das tippen meister Mitarbeiter bis zu 25%
Der Switch erlaubt die einbindung von 10 mehr Nutzern

## Automatisierte Kompilierung und Bereitstellung
Automatisierte Kompilierung, wie der Name sagt, automatisiert den Kompilierungsprozess von Programmen. Dies erfolgt meist über in einem CI/CD system dessen repo. Das CI/CD system baut, sobald ein commit gepusht wurde, eine Version und stellt sie in einem Server bereit.

Vorteile:
Ersparrte Zeit, die durch das nicht interagieren des Kompilierungsprozesss kommt.
Vereinfachtes Testing, jeder Push wird zu einem build was QA tester es ermöglicht einfach die neuste version zu holen.

## TLS-Protokoll
Das Transport Layer Security Protocol ermöglicht Sichere Verbindungen über ein sonst unsicheres Netzwerk. Das TLS Protokoll verwendet hierfür ein symmetrisches Verschlüsselungsverfahren.

#### Verschlüsselungsverfahren
Das Verschlüsselungsverfahren ist ein symmetrischen Verschlüsselungsverfahren wo der Client den Server einen Schlüssel mitteilt um die Ankommenden Nachrichten zu dechiffrieren. der Server und der Client nutzen den selben Schlüssel.

Dieser Prozess wird mit eine Handshake initiiert um eine sIchere Verbindung zwischen Host- und Client zu etablieren. Der Handshake passiert jedes mal wenn eine Verbindung über HTTPS usw. ausgeführt wird. und Klärt zwischen dem Server die Verwendete Version von TLS, die Authentifizierung des Server über dessen Public Key und die Generierung des Session Keys. Anschließend sendet der Client beim Initialen schritt die verwendete Cipher Suite.
#### Cypher Suite
Ein satz an Algorithmen die verwendet werden um eine Sichere Verbindung zu etablieren.

## Single Sign On
Beschreibt den Prozess nur einen Account zu erstellen um an mehreren Diensten teilzunehmen.
Grundsätzliches Beispeil

Vorteile:
Einfach für den Nutzer

Nachteil:
Wird dein Account gebreached, verlierst du recht viel an mist.