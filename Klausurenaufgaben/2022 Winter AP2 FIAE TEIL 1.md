
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
Grundsätzliches Beispeil: Mann meldet sich bei Microsoft an um bei Xbox, Minecraft, Office etc. reinzukommen

Vorteile:
Einfach für den Nutzer

Nachteil:
Wird dein Account gebreached, verlierst du recht viel an mist.

## Webanwendungsschichten
#### Darstellungsschicht
Diese schicht ist für die Darstellung des Programmes zuständig
#### Logikschicht
Die Logikschicht beeinhaltet die Geschäftslogik des Programms
#### Datenschicht
Die Datenbank und so.
## MVC

#### View
Das Frontend des Programms. Hierbei wird das Visuelle geklärt

#### Model
Das Model sind die verwendeten Datenstrukturen des Programmes 

#### Controller
Beeinhaltet die Geschäftslogik des Programms

## Agile Vorgehensmodelle

#### Scrum
Eine Iteratives Vorgehensmodell wo fortschritt usw mit Täglichen Meetings festgehalten wird und mit Feedback erweitert werden kann. Elemente dieses Prozessses sind 
Product Owner: Derjenige der das sagen über das Projekt hat, 
Scrum Master: Unterstützung zur einhaltung des Scrum prinzips, 
Developer: Entwickler, 
Product Backlogs: was noch gemacht werden muss, 
Sprints: Die Täglichen Meetings, 
Inkrements etc: 

## Open Source
Der Quellcode der Software ist öffentlcih zugänglich und bearbeitbar. Abhängig von der Lizenz kann der erweiterte Code auch verkauft werden.

Vorteil:
Continuerliche Entwicklung

Nachteil:
Öffentlicher Code kann zu gefundenen schwächen führen.


## HTML Elemente

Boxlists
Dropdowns
knöpfe
etc.

## DTD Datei
DTD Dateien beschreiben die Struktur von einer XML Datei. Das hier hat sein eigenen Syntax 

```
<!ELEMENT Media(Game+)>
<!ELEMENT Game (GameName, GameBeschreibung, SpielTyp, SpielDaten*)>
<!ELEMENT GameName (#PCDATA)>
<!ELEMENT GameBeschreibung (#PCDATA)>
<!ELEMENT SpielTyp (GenreName, KurzBeschreibung)>
<!ELEMENT SpielDaten (DataName, Leben, Welt)>
<!ELEMENT GenreName (#PCDATA)>
<!ELEMENT KurzBeschreibung (#PCDATA)>
<!ELEMENT DataName (#PCDATA)>
<!ELEMENT Leben (#PCDATA)>
<!ELEMENT Welt (#PCDATA)>
```

"#PCDATA" beschreibt die werte angegeben im tag
"stern" = null oder mehr
"plus" = ein oder mehr
"fragezeichen" = null oder ein
"kein symbol" = nur ein

Was ungefähr zu so einer XML wird

```
<?xml version="1.0" encoding="UTF-8">
<!DOCTYPE Media SYSTEM "media.dtd">
<Media>
	<Game>
		<GameName>Limbus Company</GameName>
		<GameBeschreibung>cool ass gatcha game</GameBeschreibung>
		<SpielTyp>
			<GenreName>Gatcha Game</GenreName>
			<KurzBeschreibung>Pull shit</KurzBeschreibung>
		</SpielTyp>
	</Game>
	<Game>
		<GameName>Half-Life 3</GameName>
		<GameBeschreibung>HOPIUM HOPIUM HOPIUM</GameBeschreibung>
		<SpielTyp>
			<GenreName>Action Adventure</GenreName>
			<KurzBeschreibung>kill shit</KurzBeschreibung>
		</SpielTyp>
		<SpielDaten>
			<DataName>Save 1. Jan 01.01.1970</DataName>
			<Leben>99</Leben>
			<Welt>Ruins of City 17</Welt>
		</SpielDaten>
	</Game>
</Media>
```

Es ist auch möglich attribute zu bestimmen.
```
<!ELEMENT auto (Name, Beschreibung)> <!-- Auto hat name und beschreibung --!>
<!ATTLIST auto ps CDATA "10"> <!-- Deklariere Attribute PS im auto. --!>
<!ATTLIST auto typ CDATA "Sport"> <!-- Deklariere Attribute Typ im auto. --!>
<!ELEMENT Name (#PCDATA)>
<!ELEMENT Beschreibung (#PCDATA)>
```

Das auto hat jetzt die Attributen "ps" und "typ". wenn ps nicht gesetzt wird ist es automatisch auf 10 das gleiche beim typ.
die XML würde so aussehen

```
<?xml version="1.0" encoding="UTF-8">
<!DOCTPYE auto SYSTEM "auto.dtd">
<auto ps="349">
	<Name>Lamborghini Gallardo</Name>
	<Beschreibung>Geiler Sportwage</Beschreibung>
<auto/>
```

Auto hat die Beschreibung "Lamborghini Gallardo" und hat die Beschreibung "Geiler Sportwagen". Das Auto hat 349 ps und ist standardmäßig mit den typen "Sport" versehen.