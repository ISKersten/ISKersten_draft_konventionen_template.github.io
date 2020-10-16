---
layout: default
---

# Architektur der

# Geodateninfrastruktur

# Deutschland

## Konventionen zu Metadaten

```
Arbeitskreis Metadaten
05. 02 .20 20
Version: 2.0. 3
```
Dieses Dokument beschreibt die Konventionen zu Metadaten in der GDI-DE mit Erläuterungen und
Beispielen.


_(Leerseite)_


## Dokumentinformation

```
Bezeichnung Architektur der Geodateninfrastruktur Deutschland – Konventionen
zu Metadaten
Autor AK Metadaten
Erstellt am 02. 04 .201 9
Bearbeitungszustand in Bearbeitung
x Vorgelegt
Abgestimmt
Dokumentablage Kollaborationsplattform GDI-DE
Arbeitskreis
Metadaten
```
```
Peter Kochmann (GDI-NW | Bezirksregierung Köln – Abteilung
Geobasis NRW)
Steffen Bach (GDI-BW | Landesamt für Geoinformation und
Landentwicklung Baden-Württemberg – Kompetenzzentrum
Geodateninfrastruktur)
Andreas Berg (GDI-SN | Staatsbetrieb Geobasisinformation und
Vermessung Sachsen (GeoSN) – Administration
Geodateninfrastruktur)
Valentina Gorsic (GDI-HE | Hessisches Landesamt für
Bodenmanagement und Geoinformation –
Geoinformationsmanagement)
Anja Jacobi (GDI-SN | Staatsbetrieb Geobasisinformation und
Vermessung Sachsen (GeoSN) – Koordinierung
Geodateninfrastruktur)
Anja Loddenkemper (Kst. GDI-NI | Landesamt für Geoinformation und
Landesvermessung Niedersachsen – Landesbetrieb -)
Stefanie Nadler (BLE | Bundesanstalt für Landwirtschaft und
Ernährung – Fachzentrum für Geoinformation und Fernerkundung für
den Geschäftsbereich des BMEL)
Andrea Pörsch (GDI-BB | LGB – Landesvermessung und
Geobasisinformation Brandenburg – Kontaktstelle GDI-DE +
Metadatenmanagement)
Michael Räder (MDI-DE | Nationalpark-Verwaltung Niedersächsisches
Wattenmeer / Niedersächsischer Landesbetrieb für Wasserwirtschaft,
Küsten- und Naturschutz)
Sabine Schütze (BKG | Bundesamt für Kartographie und Geodäsie –
Geodateninfrastrukturleistungen)
Martin Thal (GDI-HH | Landesbetrieb Geoinformation und
Vermessung – Urban Platform | Betrieb Serversysteme)
Renate Zweer (GDI-BE | Senatsverwaltung für Stadtentwicklung und
Wohnen – Geoinformation)
Anja Litka (Kst. GDI-DE | Bundesamt für Kartographie und Geodäsie)
```
Die Autoren danken den vielen Personen und Institutionen, die am Entwicklungsprozess des
Konventionendokumentes aktiv beteiligt waren.


## Änderungsverzeichnis

```
Version Datum Änderung Ersteller
```
```
0.
beta
```
```
27 .03.2013 Aufbereitung als Vorlage zur Beschlussfassung im
LG GDI-DE
```
```
AK Metadaten
```
```
0.9 13 .05.2014 Beschluss Nr. 69 im LG GDI-DE Vorsitz LG
1.
beta
```
```
17.11.2014 Aufbereitung als Vorlage zur Beschlussfassung im
LG GDI-DE
```
```
AK Metadaten
```
```
1.0 14.01.2015 Beschluss Nr. 79 im LG GDI-DE Vorsitz LG
1.
beta
```
```
21.04.2015 Fehlerkorrektur Codelisten, Ergänzung Anhang 2 AK Metadaten
```
```
1.1.0 27.07.2015 Beschluss Nr. 88 im LG GDI-DE Vorsitz LG
1.1.
beta
```
```
01.04.2016 ATS-Referenzen und Abschnitt 1.4 eingefügt; ed.
Korrekturen
```
```
AK Metadaten
```
```
1.1.1 14.04.2016 Aufbereitung zur Veröffentlichung Kst. GDI-DE
1.2.
beta
```
```
04. 04. 2017 Kategorisierung der Konventionen bzgl. INSPIRE
und/oder GDI-DE plus entsprechende
Kennzeichnung in jedem Kapitel
```
```
AK Metadaten
```
##### 1.2.

```
beta
```
```
18.04.2017 Aufbereitung als Vorlage zur Beschlussfassung im
LG GDI-DE
```
```
Kst. GDI-DE
```
```
1.2.
beta
```
```
01.08.2017 Korrekturen sowie Aktualisierung als Vorlage zur
Beschlussfassung im LG GDI-DE
```
```
AK Metadaten
```
```
1.2.0 30.08.2017 Beschluss Nr. 103 im LG GDI-DE Vorsitz LG
1.3.
beta
```
```
nicht
veröffentlicht
```
```
interne Version; Arbeitsdokument bzgl. Anpassung
der Konventionen an TG MD 2.0.
```
```
AK Metadaten
```
```
2.0.
beta
```
```
0 7.03.2019 Anpassung der Konventionen an TG MD 2.0.1 AK Metadaten
```
```
2.0.
beta
```
```
02.04.2019 Aufbereitung als Vorlage zur Beschlussfassung im
LG GDI-DE
```
```
Kst. GDI-DE
```
```
2.0.0 06.06.2019 Beschluss Nr. 121 im LG GDI-DE Vorsitz LG
2.0.1 12 .0 6 .2019 Anpassung der Beispiele aufgrund Beschluss im LG
GDI-DE
```
```
AK Metadaten
```
```
2.0.2 22.11.2019 Redaktionelle Anpassungen (Anhang 2) AK Metadaten
2.0.3 05.02.2 020 Redaktionelle Anpassungen (Anhang 3) AK Metadaten
```

## Inhalt


- 1 Einführung
   - 1.1 Die Architektur der Geodateninfrastruktur Deutschland
   - 1.2 Konventionen zu Metadaten
   - 1.3 Die Topologie der Metadatenkataloge
   - 1.4 Hinweise zum Dokument
- 2 Grundsätzliche Konventionen für alle Metadaten
   - 2.1 Multiplizität des identificationInfo-Elementes
   - 2.2 Eindeutiger Metadatensatzidentifikator
   - 2.3 Art der Ressource
   - 2.4 Sprache der Metadaten
   - 2.5 Kontakt (Verantwortliche Stelle Metadaten)
   - 2.6 Kontakt (Verantwortliche Stelle für die Ressource)
   - 2.7 Schlüsselwörter
      - 2.7.1 Schlüsselwort „inspireidentifiziert“
   - 2.8 Beschränkungen des öffentlichen Zugangs ([INS VO MD], B 8.2)
   - 2.9 Nutzungs- und Zugriffsbedingungen
      - 2.9.1 Nutzungs- und Zugriffsbedingungen in der GDI-DE (ohne INSPIRE)
      - 2.9.2 Bedingungen für den Zugang und die Nutzung bei INSPIRE ([INS VO MD], B 8.1)
   - 2.10 Regionalschlüssel
   - bereitgestellten Daten 2.11 Kennzeichnung der Verbindlichkeit von per Darstellungs- und/oder Downloaddienst
   - 2.12 Konformität (Übereinstimmung mit Spezifikationen, [INS VO MD], B 7)
- 3 Konventionen für Metadaten zu Datenbeständen und Anwendungen
   - 3.1 Eindeutiger Ressourcenidentifikator ([INS VO MD], B 1.5)
   - 3.2 Schlüsselwörter
      - 3.2.1 Quellenangabe für Schlüsselwörter zu INSPIRE-Themen.......................................................
      - 3.2.2 Schlüsselwort „opendata“
   - 3.3 Themenkategorie nach ISO (Zuordnung zum INSPIRE-Thema: [INS VO MD], B 2.1)
   - 3.4 Ressourcenverweis für Datensätze und –serien (transferOptions, [INS VO MD], B 1.4)
   - 3.5 Konformität (Übereinstimmung mit Spezifikationen, [INS VO MD], B 7)
   - 3.6 Nutzungsbedingungen und Lizenzinformationen für Open Data
   - 3.7 Formatangaben
- 4 Konventionen für Metadaten zu Diensten
   - 4.1 Schlüsselwörter
      - 4.1.1 Schlüsselwörter zu Dienstkategorien bei INSPIRE
   - 4.2 Verlinkung zum verwendeten Datenbestand (Daten-Dienste-Kopplung)
      - 4.2.1 Gekoppelte Daten-Ressource ([INS VO MD], B 1.6)
      - 4.2.2 Art der Kopplung zwischen Dienst und zugehörigen Daten
   - 4.3 Ressourcenverweise für Dienste
      - 4.3.1 Ressourcenverweis unter transferOptions ([INS VO MD], B 1.4)
      - 4.3.2 Ressourcenverweis unter connectPoint
   - 4.4 Art des Geodatendienstes bei INSPIRE ([INS VO MD], B 2.2)
   - 4.5 Version des Geodatendienstes bei INSPIRE
   - 4.6 Konformität (Übereinstimmung mit Spezifikationen, [INS VO MD], B 7)
- 5 Daten-Dienste-Kopplung
- 6 Open Data-Informationen zu Datensätzen und -serien
- 7 Werkzeuge zur Überprüfung der Konventionen
- Referenzen
- Anhang 1: INSPIRE-Spezifikationen (Durchführungsbestimmungen)
- Anhang 2: Zuordnung der INSPIRE-Annex-Themen zu ISO-Themenkategorien
- Anhang 3: Beschränkungen des öffentlichen Zugangs bei INSPIRE
- Version 1.2.0 vom 01.08.2017 Anhang 4: Nachweis der Änderungen der Konventionen zu Metadaten Version 2.0.0 gegenüber


## 1 Einführung

### 1.1 Die Architektur der Geodateninfrastruktur Deutschland

Um ein reibungsloses Zusammenwirken der nationalen technischen Komponenten der GDI-DE zu
ermöglichen, sind organisatorische und technische Rahmenvorgaben erforderlich, die zusammen-
fassend als Architekturkonzept der GDI-DE bezeichnet werden.

Zur leichteren Handhabung ist das Architekturkonzept der GDI-DE aus einzelnen Dokumenten in
drei verschiedenen Kategorien (grundsätzliche Festlegungen, spezielle technische Festlegungen und
Empfehlungen) aufgebaut:

**Abbildung 1 : Architekturkonzept der GDI-DE – Übersicht über die Architekturdokumente**

Grundsätzliche Festlegungen werden durch Beschluss des LG GDI-DE in folgenden Dokumenten
getroffen:

```
 Das Dokument „Architektur der GDI-DE - Ziele und Grundlagen“ erläutert die strategischen
Ziele, fachliche und technische Grundsätze sowie die rechtlichen und organisatorischen
Rahmenbedingungen der GDI-DE [GDI-DE Architektur - Ziele].
 Das Dokument „Architektur der GDI-DE - Technik“ beschreibt die verschiedenen Architektur-
komponenten und referenziert hierfür relevante Normen, Standards und Spezifikationen
[GDI-DE Architektur - Technik].
 Das Dokument „Architektur der GDI-DE - Maßnahmenplan“ zeigt die für die künftige
Entwicklung der GDI-DE erforderlichen Schritte auf [GDI-DE Architektur - Maßnahmen].
```
Spezielle technische Festlegungen, vor allem in Bezug auf Technik und Betrieb von Komponenten der
GDI-DE, werden durch Beschluss des LG GDI-DE in folgenden Dokumenten getroffen:

```
 Profile der GDI-DE zu internationalen oder nationalen Normen und
 Konventionen, die über eine Norm oder Spezifikation hinausgehen.
```

Darüber hinausgehende Informationen werden als Handlungsempfehlungen von Arbeitskreisen
weiter konkretisiert.

### 1.2 Konventionen zu Metadaten

Im vorliegenden Dokument werden Konventionen zu Metadaten sowie deren Bereitstellung
erläutert und zusammengefasst. Diese Konventionen werden im Arbeitskreis (AK) Metadaten
erarbeitet. Ältere Vorgängerversionen gehen auch auf Arbeiten der Projektgruppe
Geodatenkatalog.de und einen Metadaten-Workshop mit Ansprechpartnern der GDI-DE aus Bund
und Ländern zurück. Weitere Hinweise, welche sich auf die Inhalte von Metadaten beziehen, finden
sich in eigenen Handlungsempfehlungen, z. B. der Länder-GDIs^1 , wieder.

In Geodateninfrastrukturen gibt es grundsätzlich zwei unterschiedliche Typen von
Metadatendokumenten:

```
 Typ1: Capabilities-Dokumente, mit welchen Dienste-Schnittstellen ihre Eigenschaften
beschreiben.
 Typ2: Metadaten nach ISO 19115/19119, welche in Katalogen erfasst und bereitgestellt
werden.
```
Das vorliegende Dokument befasst sich überwiegend mit Konventionen zu Typ 2. Typ 1 wird in den
Konventionsdokumenten bzw. Handlungsempfehlungen des AK Geodienste behandelt^2.

Grundsätzlich sollen in der GDI-DE sowohl die Anforderungen aus der INSPIRE-Richtlinie [INS VO
MD, INS TG MD] (sofern relevant) als auch die ISO-Festlegungen [ISO 19115, ISO 19119, ISO 19139]
erfüllt werden. Alle Vorgaben der ISO (Belegungspflichten bzw. -bedingungen, Werteumfänge etc.)
gelten somit auch für die GDI-DE. Das bedeutet, dass es weitere, zwingend zu belegende
Metadatenelemente geben kann, die benötigt werden, um einen ISO- und/oder INSPIRE-konformen
Metadatensatz zu bilden, auch wenn das vorliegende Dokument keine Konvention dazu aufführt.

Ergänzend bzw. vertiefend werden in diesem Dokument konkrete Konventionen für einzelne
Metadatenelemente in der GDI-DE beschrieben. Die Festlegungen im vorliegenden Dokument
betreffen Metadatenelemente, für die Regelungsbedarf in der GDI-DE gesehen wird, der über die
grundsätzlichen Regelungen der ISO hinausgehen kann oder aus verpflichtenden oder bedingten
Angaben für INSPIRE resultiert.

Außerdem trifft dieses Dokument keine Festlegungen zur inhaltlichen Strukturierung von Freitext-
Elementen wie z. B. Titel und Kurzbeschreibung. Etwaige Regelungen für eine einheitliche Vergabe
von Titeln, Kurzbeschreibungen etc. und die Festlegung von Benennungsmustern liegen im
Ermessen der einzelnen Fachnetzwerke und sind durch diese in eigenen Leitfäden zu treffen.

Bzgl. der Vorgaben seitens INSPIRE wird an dieser Stelle explizit darauf hingewiesen, dass zzt. für
die GDI-DE keine Betrachtung der sog. „aufrufbaren Geodatendienste“, die keine INSPIRE-
Netzdienste sind, erfolgt. Aus der INSPIRE Technical Guidance zu Metadaten V2.0.1 wurden daher
nur die Belange für Metadaten zu Datensätzen und -serien sowie zu Netzdiensten berücksichtigt. Die
Vorgaben für aufrufbare Geodatendienste gelten seitens INSPIRE davon unbenommen; eine
Präzisierung durch die GDI-DE bleibt jedoch zzt. aus, weil momentan keine Anwendungsfälle

(^1) [http://www.geoportal.de/DE/GDI-DE/Media-Center/Dokumente/dokumente.html?lang=de](http://www.geoportal.de/DE/GDI-DE/Media-Center/Dokumente/dokumente.html?lang=de)
(^2) [http://www.geoportal.de/DE/GDI-DE/Arbeitskreise/Geodienste/geodienste.html?lang=de](http://www.geoportal.de/DE/GDI-DE/Arbeitskreise/Geodienste/geodienste.html?lang=de)


existieren. Bei Bedarf wird dies zu einem späteren Zeitpunkt im Rahmen der Fortschreibung dieses
Dokumentes ergänzt.

### 1.3 Die Topologie der Metadatenkataloge

In der GDI-DE existieren eine Vielzahl verteilter, eigenständiger Metadatenkataloge, deren Inhalte im
zentralen Geodatenkatalog.de zusammengeführt werden. Eine ähnliche Aggregation geschieht auch
in anderen Knoten. Beispielsweise laufen in den Katalogen der Bundesländer die Metadaten aus
verschiedenen Bereichen und Ebenen der Verwaltung zusammen. Abbildung 2 (Seite 9 ) verdeutlicht
diesen Zusammenhang.

Eine Beschreibung der zentralen Komponente „Geodatenkatalog.de“ der GDI-DE erfolgt in diesem
Dokument nicht, sondern ist im Dokument „Architektur der GDI-DE – Technik“ zu finden [GDI-DE
Architektur - Technik]. Dort werden auch die Voraussetzungen für die Einbindung einer dezentralen
Katalogschnittstelle in die GDI-DE beschrieben.

**Abbildung 2 : Topologie der Metadatenkataloge**

Durch die Topologie der Metadatenkataloge ist es notwendig, dass Änderungen eines Katalogs
überall dort nachvollzogen werden, wo dessen Bestand übernommen wird. Wird also ein
Metadatensatz in einem Katalog gelöscht, so wird er auch in allen anderen Katalogen entfernt, welche
diesen Katalog harvesten, da der _fileIdentifier_ des Metadatensatzes und damit der Metadatensatz
selbst nicht mehr auffindbar ist. Übernommen werden zugleich alle „neuen“ Metadaten mit einem
bisher nicht vorhandenen _fileIdentifier_ und alle geänderten Metadaten, deren _fileIdentifier_ bereits
bekannt sind, die jedoch einen aktualisierten Zeitstempel tragen.


### 1.4 Hinweise zum Dokument

Die Festlegungen in diesem Dokument sind für die Metadaten-Sprache „Deutsch“ getroffen, sofern
durch ISO oder INSPIRE keine anderen Forderungen bestehen.

Den einzelnen Festlegungen in diesem Dokument ist jeweils ein XPath-Ausdruck vorangestellt:

Dieser adressiert bzw. beschreibt die Position des betreffenden Metadatenelementes im XML-
Dokument. Die Kodierung des Elementes in XML wird jeweils wie folgt exemplarisch dargestellt:

Die einzelnen Festlegungen des Dokumentes enthalten am Anfang jeweils folgende Tabelle:

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ (^) ☐ ☐
zusätzlich für INSPIRE (^) ☐ (^) ☐ ☐
Diese Tabelle gibt einen Überblick über die jeweilige Forderung der GDI-DE bzw. zusätzlich für
INSPIRE. Dabei gelten folgende Festlegungen:
 „GDI-DE“ – generelle Konventionen für alle Metadaten, um eine Einheitlichkeit in den
Metadaten der GDI-DE zu fördern und deren Interoperabilität zu gewährleisten. Diese
Anforderungen können begründet sein
 über [ISO 19115] und [ISO 19119] hinausgehende Festlegungen zwecks
Einheitlichkeit;
 durch die Verwendung der Metadaten für Open Data (siehe Kapitel 6 );
 durch Vorgaben seitens INSPIRE, für die eine Verallgemeinerung und Übertragung
auf die gesamte GDI-DE als sinnvoll erachtet wurde.
 „zusätzlich für INSPIRE“ - Konventionen, die sich aus der RICHTLINIE 2007/2/EG DES
EUROPÄISCHEN PARLAMENTS UND DES RATES vom 14. März 2007 zur Schaffung einer
Geodateninfrastruktur in der Europäischen Gemeinschaft (INSPIRE), den INSPIRE
Implementing Rules oder den zugehörigen Technical Guidance-Dokumenten ergeben.
Hierbei handelt es sich um Klarstellungen oder Präzisierungen der GDI-DE, um die
Metadaten, die Ressourcen für INSPIRE beschreiben, einheitlich zu gestalten (z. B. in Fällen,
in denen INSPIRE Freiräume zulässt). Grundsätzlich betrifft dies nur Metadaten, die
Datensätze, -serien oder Netzdienste für INSPIRE beschreiben. Die Konventionen unter „GDI-
DE“ (s.o.) sind dabei ebenfalls zu beachten und einzuhalten.
 _verpflichtend_ – generelle Verpflichtungen zur Erfüllung der Anforderungen seitens der GDI-
DE bzw. für INSPIRE.
 _konditional_ - Verpflichtungen unter bestimmten Bedingungen, um die Anforderungen seitens
der GDI-DE bzw. für INSPIRE zu erfüllen. Die jeweilige Konvention ist dann verpflichtend,
wenn die benötigten Informationen vorliegen bzw. eine beschriebene Situation zutrifft.
**XPath:**
MD_Metadata/
**Beispiel:**
<gmd:MD_Metadata>
...
</gmd:MD_Metadata>


```
 optional - keine Verpflichtung zur Führung der jeweiligen Information. Für den Fall, dass
diese Information aber erfasst werden soll, gelten die jeweils genannten Konventionen.
```
Im Fließtext sind die Bezeichnungen von Metadatenelementen kursiv gesetzt, z. B.: _MD_Metadata_.
Die Attributwerte sind in Anführungszeichen angegeben, z. B.: „Es gelten keine Bedingungen“.

Die dabei verwendeten Bezeichnungen von Metadatenelementen beziehen sich auf die Nomenklatur
der Spezifikationen der [ISO 19115] und [ISO 19119] sowie der INSPIRE-Verordnung für Metadaten
[INS VO MD].

Jede Festlegung in diesem Dokument endet mit einem Verweis auf die dazugehörige
Testbeschreibung in Form einer _Abstract Testsuite_ (ATS). Dort sind die jeweiligen Testschritte,
welche in der GDI-DE Testsuite implementiert wurden, im Detail beschrieben:

Als Referenz werden unter
_https://ims.geoportal.de/git/tree/AK-Metadaten.git/version2.0.0/konventionen!beispiel_xml_
Beispieldokumente bereitgestellt:
 _dataset.xml_ (Daten-Metadatensatz)
 _service.xml_ (Dienst-Metadatensatz)
 _wms.xml_ (WMS-Capabilities-Dokument)
 _opendata_dataset.xml_ (Daten-Metadatensatz)

In diesen Muster-Metadatensätzen sind die Konventionen, wie in diesem Dokument dargelegt,
umgesetzt.

Dieses Dokument wird in einem stetigen Prozess fortgeschrieben und veröffentlicht. Je nach
Veränderungen im Dokument werden die Versionsnummern wie folgt angepasst:

```
Änderungen in der
Versionsnummer
```
```
Anlass bzw. Umfang der Änderung
```
1. (^) Änderungen in den gesetzlichen Bestimmungen und damit
grundsätzliche Änderungen im Dokument
1.1 (^) Geringfügige Änderungen oder Ergänzungen in den Kapiteln, Ergänzung
von neuen Kapiteln
1.1.1 Berichtigung von Schreibfehlern, Fehlerbehebung, redaktionelle
Änderungen in den Kapiteln ohne fachliche Auswirkungen
**ATS:**
https://ims.geoportal.de/git/tree/AK-Metadaten.git/version2.0.0/konventionen!ats


## 2 Grundsätzliche Konventionen für alle Metadaten

Die Konventionen in diesem Kapitel betreffen die Metadaten zu allen Ressourcen in der GDI-DE,
unabhängig von der Art der Ressource im _hierarchyLevel_ - Element (siehe 2.3).

### 2.1 Multiplizität des identificationInfo-Elementes

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☒ (^) ☐ ☐
zusätzlich für INSPIRE (^) ☐ ☐ ☐
Um die Einheitlichkeit und eindeutige Interpretierbarkeit der Metadaten in der GDI-DE zu fördern,
gilt als Konvention für alle Metadaten in der GDI-DE:
Alle relevanten Informationen sind im ersten _identificationInfo_ - Element anzugeben.
Gemäß [ISO 19115] kann das _identificationInfo_ - Element innerhalb eines Metadatensatzes mehrfach
verwendet werden. Im Rahmen von INSPIRE wird jedoch nur das erste _identificationInfo_ - Element
ausgewertet (siehe [INS TG MD], 2.3). Auch im Geoportal.de finden nur Informationen
Berücksichtigung, die im ersten _identificationInfo_ - Element angegeben sind.

### 2.2 Eindeutiger Metadatensatzidentifikator

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☒ ☐ ☐
zusätzlich für INSPIRE (^) ☐ ☐ ☐
Ein Metadatensatz besitzt immer einen eindeutigen Identifikator. Die Verwendung einer UUID
gemäß RFC 4122^3 wird empfohlen. Sollte der bisher verwendete Metadatensatzidentifikator
historisch bedingt nicht den Regeln einer UUID entsprechen, so ist dieser im Sinne des
Bestandsschutzes weiterhin zulässig. Der Identifikator soll, unabhängig von Überarbeitung am
Metadatensatz selbst, nicht verändert werden. Beim Replizieren muss dieser beibehalten und darf
nicht überschrieben werden. Nur so sind eine eindeutige Identifizierung von Metadaten, die
(^3) RFC 4122: https://www.ietf.org/rfc/rfc4122.txt
**XPath:**
MD_Metadata/identificationInfo[1]
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_2.1_identificationInfo.pdf?inline=false
**XPath:**
MD_Metadata/fileIdentifier


zuverlässige Filterung von Dubletten sowie die Aktualisierung vorhandener Metadatensätze anhand
von _fileIdentifier_ ([ISO 19115], B.2.1, No. 2) und _dateStamp_ ([ISO 19115], B.2.1, No. 9) innerhalb der
GDI-DE möglich.

### 2.3 Art der Ressource

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☒ (^) ☐ ☐
zusätzlich für INSPIRE (^) ☐ (^) ☐ ☐
Ein Metadatensatz muss immer eine Information über die Art der Ressource, die er beschreibt,
beinhalten. Dies geht über die Regelungen aus [ISO 19115] für das _hierarchyLevel_ - Element ([ISO
19115], B.2.1, No. 6 ) hinaus und soll eine eindeutige Interpretierbarkeit des Metadatensatzes
innerhalb der GDI-DE ermöglichen.

### 2.4 Sprache der Metadaten

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☒ (^) ☐ ☐
zusätzlich für INSPIRE (^) ☐ ☐ ☐
**Beispiel:**
<gmd:fileIdentifier>
<gco:CharacterString>
**f7e4808f-642c-404b-ae57-067e0d7d**
</gco:CharacterString>
</gmd:fileIdentifier>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_2.2_metadatensatzidentifikator.pdf?inline=false
**XPath:**
MD_Metadata/hierarchyLevel
**Beispiel:**
<gmd:hierarchyLevel>
<MD_ScopeCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_ScopeCode"
codeListValue=" **dataset** "/>
</gmd:hierarchyLevel>
**ATS:**
https://git.gdi-de.org/ak-metadaten/konventionen/raw/master/ats/gdide_2.3_artRessource.pdf
?inline=false


Ein Metadatensatz muss immer eine Information über die in den Metadaten verwendete Sprache
beinhalten.

Diese Konvention beruht auf den Vorgaben aus [INS TG MD], 2.2.2 (Requirement C.5) und geht über
die Regelungen aus [ISO 19115] für das _language_ - Element in [ISO 19115], B.2.1, No. 3, hinaus.

Um die Einheitlichkeit und die eindeutige Interpretierbarkeit der Metadaten in der GDI-DE zu
fördern, wird diese Konvention für alle Metadaten in der GDI-DE übernommen.

### 2.5 Kontakt (Verantwortliche Stelle Metadaten)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☒ (^) ☐ ☐
zusätzlich für INSPIRE (^) ☐ (^) ☐ ☐
Ein Metadatensatz muss immer eine Information über die für die Erstellung und Pflege der
Metadaten zuständige Stelle beinhalten. Diese Information muss mindestens Folgendes beinhalten:
 einen Namen im _organisationName_ - Element _;_
 eine E-Mail-Adresse im _electronicMailAddress_ - Element;
 die Rolle „pointOfContact“ im _role_ - Element.
Diese Konvention beruht auf den Vorgaben aus [INS TG MD], 2.2.3 (Requirement C.6) und geht über
die Regelungen aus [ISO 19115] für das _CI_ResponsibleParty_ - Element in [ISO 19115], B.3.2.1, No. 374,
hinaus.
Um die Einheitlichkeit der Metadaten in der GDI-DE zu fördern, wird diese Konvention für alle
Metadaten in der GDI-DE übernommen.
**XPath:**
MD_Metadata/language
**Beispiel:**
<gmd:language>
<LanguageCode codeList="http://www.loc.gov/standards/iso639-2/"
codeListValue=" **ger** "/>
</gmd:language>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_2.4_spracheMetadaten.pdf?inline=false
**XPath:**
MD_Metadata/contact/CI_ResponsibleParty/organisationName
MD_Metadata/contact/CI_ResponsibleParty/contactInfo/CI_Contact/address/CI_Address/e
lectronicMailAddress
MD_Metadata/contact/CI_ResponsibleParty/role


### 2.6 Kontakt (Verantwortliche Stelle für die Ressource)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☒ ☐ ☐
zusätzlich für INSPIRE (^) ☐ ☐ ☐
Ein Metadatensatz muss immer eine Information über die für die Ressource zuständige Stelle
beinhalten. Diese Information muss mindestens Folgendes beinhalten:
 einen Namen im _organisationName_ - Element _;_
 eine E-Mail-Adresse im _electronicMailAddress_ - Element.
**Beispiel:**
<gmd:contact>
<gmd:CI_ResponsibleParty>
<gmd:organisationName>
<gco:CharacterString> **Verwaltung XY** </gco:CharacterString>
</gmd:organisationName>
...
<gmd:contactInfo>
<gmd:CI_Contact>
...
<gmd:address>
<gmd:CI_Address>
...
<gmd:electronicMailAddress>
<gco:CharacterString> **verwaltungXY@deutschland.de** </gco:CharacterString>
</gmd:electronicMailAddress>
</gmd:CI_Address>
</gmd:address>
...
</gmd:CI_Contact>
</gmd:contactInfo>
<gmd:role>
<gmd:CI_RoleCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#CI_RoleCode"
codeListValue=" **pointOfContact** "/>
</gmd:role>
</gmd:CI_ResponsibleParty>
</gmd:contact>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_2.5_kontaktMetadaten.pdf?inline=false
**XPath:**
MD_Metadata/identificationInfo[1]//pointOfContact/CI_ResponsibleParty/organisationN
ame
MD_Metadata/identificationInfo[1]//pointOfContact/CI_ResponsibleParty/contactInfo/C
I_Contact/address/CI_Address/electronicMailAddress
MD_Metadata/identificationInfo[1]//pointOfContact/CI_ResponsibleParty/role


Diese Konvention beruht auf den Vorgaben aus [INS TG MD], 2.3.3 (Requirement C.10) und geht über
die Regelungen aus [ISO 19115] für das _CI_ResponsibleParty_ - Element in [ISO 19115], B.3.2.1, No. 374,
hinaus.

Um die Einheitlichkeit der Metadaten in der GDI-DE zu fördern, wird diese Konvention für alle
Metadaten in der GDI-DE übernommen.

Als **zusätzliche Empfehlung** gilt: Im _role_ - Element wird die Rolle „pointOfContact“ verwendet.

Hintergrund: Sowohl die Auswertung in der GDI-DE zum INSPIRE-Monitoring sowie die Ableitung
der Metadaten für GovData berücksichtigen diese Rolle in besonderer Art, d. h. derart
gekennzeichnete Kontakte sind diejenigen, die übernommen bzw. bevorzugt werden.

Weitere Kontakte mit anderen Rollen bleiben davon unberührt.

### 2.7 Schlüsselwörter

Schlüsselwörter dienen der schnellen Auffindbarkeit von Daten und Diensten. Häufig werden
Schlüsselwörter verwendet, um Geodatenressourcen zu bestimmten Fachthemen such- bzw.
auffindbar zu machen oder um die Geodatenressourcen in einem lokalen Zusammenhang, z. B. in

```
Beispiel:
<gmd:pointOfContact>
<gmd:CI_ResponsibleParty>
<gmd:organisationName>
<gco:CharacterString> Verwaltung XY </gco:CharacterString>
</gmd:organisationName>
...
<gmd:contactInfo>
<gmd:CI_Contact>
...
<gmd:address>
<gmd:CI_Address>
...
<gmd:electronicMailAddress>
<gco:CharacterString> verwaltungXY@deutschland.de </gco:CharacterString>
</gmd:electronicMailAddress>
</gmd:CI_Address>
</gmd:address>
...
</gmd:CI_Contact>
</gmd:contactInfo>
<gmd:role>
<gmd:CI_RoleCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#CI_RoleCode"
codeListValue=" pointOfContact "/>
</gmd:role>
</gmd:CI_ResponsibleParty>
</gmd:pointOfContact>
```
```
ATS:
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_2.6_kontaktRessource.pdf?inline=false
```

einem Portal gesammelt darstellen zu können. In diesem Dokument wird jedoch nur Bezug auf
Schlüsselwörter genommen, die für die GDI-DE in ihrer Gesamtheit gültig sind.

#### 2.7.1 Schlüsselwort „inspireidentifiziert“

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ (^) ☐
zusätzlich für INSPIRE (^) ☒ ☐ (^) ☐
Metadatensätze, die von INSPIRE betroffene Geodatensätze oder –dienste beschreiben, werden mit
dem Eintrag des Schlüsselworts „ **inspireidentifiziert** “ im _keyword_ - Element ([ISO 19115], B.2.2.3,
No. 53) gekennzeichnet und werden dadurch beim INSPIRE-Monitoring berücksichtigt.
Das Schlüsselwort „inspireidentifiziert“ ist keinem Thesaurus entnommen und wird ohne
Quellenangabe in den Metadaten geführt.

### 2.8 Beschränkungen des öffentlichen Zugangs ([INS VO MD], B 8.2)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☐
zusätzlich für INSPIRE (^) ☒ (^) ☐ ☐
Dieser Abschnitt beschreibt, wie Zugriffseinschränkungen im Sinne des INSPIRE-Elements
"Beschränkungen des öffentlichen Zugangs" entsprechend der [INS TG MD] zu erfassen sind. Dabei
sind Beschränkungen des öffentlichen Zugangs nur in den in Artikel 13(1) a) - h) der INSPIRE-
Richtlinie genannten Fällen zulässig.
**XPath:**
MD_Metadata/identificationInfo[1]//descriptiveKeywords/*/keyword
**Beispiel:**
<gmd:descriptiveKeywords>
<gmd:MD_Keywords>
<gmd:keyword>
<gco:CharacterString> **inspireidentifiziert** </gco:CharacterString>
</gmd:keyword>
</gmd:MD_Keywords>
</gmd:descriptiveKeywords>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_2.7.1_schluesselwortInspireidentifiziert.pdf?inline=fals
e
**XPath:**
MD_Metadata/identificationInfo[1]//resourceConstraints/MD_LegalConstraints/accessCo
nstraints


Die Beschränkungen des öffentlichen Zugangs sind nach [INS TG MD], 2.3.6 (Requirement C.17),
innerhalb eines gemeinsamen _MD_LegalConstraints_ - Objekts in folgenden Elementen anzugeben:

```
 genau ein accessConstraints - Element, Codelisten-Wert " otherRestrictions " aus
MD_RestrictionCode ([ISO 19115], B.5.24)
```
und

```
 ein oder mehrere otherConstraints - Elemente; jedes enthält einen Grund für die
Beschränkung des öffentlichen Zugangs nach Artikel 13(1) a) - h) der INSPIRE-Richtlinie als
gmx:Anchor - Element (Verweis auf einen Eintrag in der seitens INSPIRE bereitgestellten
Codeliste zu LimitationsOnPublicAccess). Da die Metadaten-Sprache Deutsch ist, soll die
zusätzliche Text-Ausprägung die deutsche Übersetzung des angegebenen Codelisten-Wertes
beinhalten. Die Tabelle im Anhang 3: Beschränkungen des öffentlichen Zugangs bei INSPIRE
enthält die o. g. Gründe nach Artikel 13 der INSPIRE-Richtlinie und listet den jeweils
benötigten Eintrag für das gmx:Anchor - Element sowie für den deutschsprachigen Begleittext
auf.
```
Liegen keine Beschränkungen vor, so ist im _otherConstraints_ - Element statt eines Grundes für die
Beschränkung der Verweis zum Codelisten-Wert " **noLimitations** " der INSPIRE-Codeliste zu
LimitationsOnPublicAccess^4 ebenfalls als _gmx:Anchor_ - Element einzutragen. Zur semantischen
Abgrenzung gegenüber den Nutzungsbedingungen (siehe 2.9) wird als deutschsprachige
Entsprechung der Freitext „Es gelten keine Zugriffsbeschränkungen“ empfohlen. Alternativ kann der
für diesen Zweck bisher dokumentierte Freitext „Es gelten keine Bedingungen“ beibehalten werden.

(^4) [http://inspire.ec.europa.eu/metadata-codelist/LimitationsOnPublicAccess](http://inspire.ec.europa.eu/metadata-codelist/LimitationsOnPublicAccess)
**Beispiel mit Begründung nach Artikel 13:**
<gmd:resourceConstraints>
<gmd:MD_LegalConstraints>
<gmd:accessConstraints>
<gmd:MD_RestrictionCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_RestrictionCode"
codeListValue=" **otherRestrictions** "/>
</gmd:accessConstraints>
<gmd:otherConstraints>
<gmx:Anchor xlink:href="http://inspire.ec.europa.eu/metadata-
codelist/LimitationsOnPublicAccess/INSPIRE_Directive_Article13_1e"> **Öffentlicher
Zugriff beschränkt entsprechend Artikel 13(1)(e) der INSPIRE-Richtlinie: e)
aufgrund nachteiliger Auswirkungen auf die Rechte des geistigen Eigentums**
</gmx:Anchor>
</gmd:otherConstraints>
</gmd:MD_LegalConstraints>
</gmd:resourceConstraints>


### 2.9 Nutzungs- und Zugriffsbedingungen

#### 2.9.1 Nutzungs- und Zugriffsbedingungen in der GDI-DE (ohne INSPIRE)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☒ ☐ (^) ☐
zusätzlich für INSPIRE (^) ☐ ☐ (^) ☐
Dieser Abschnitt beschreibt, wie Nutzungs- und Zugriffsbedingungen in den Metadaten der GDI-DE
dokumentiert werden, sofern es sich um eine Ressource handelt, die nicht unter die INSPIRE-
Richtlinie fällt. Sonst gelten stattdessen die Regelungen für das INSPIRE-Element "Bedingungen für
den Zugang und die Nutzung" unter 2.9.2.
Die Bedingungen für den Zugang und die Nutzung sind innerhalb eines gemeinsamen
_MD_LegalConstraints_ - Objekts anzugeben. Dadurch wird sichergestellt, dass textliche Erläuterungen
zweifelsfrei der ggf. dokumentierten Beschränkungsart zugeordnet werden können.
In den Metadaten der GDI-DE besteht das _MD_LegalConstraints_ - Objekt für Nutzungs- und
Zugriffsbedingungen aus folgenden Elementen:
 verpflichtend mindestens ein _useConstraints_ - Element; Inhalt ist Codelisten-Wert aus
_MD_RestrictionCode_ ([ISO 19115], B.5.24); empfohlener Inhalt: „ **otherRestrictions** “;
und
**Beispiel mit Aussage, dass keine Beschränkungen vorliegen:**
<gmd:resourceConstraints>
<gmd:MD_LegalConstraints>
<gmd:accessConstraints>
<gmd:MD_RestrictionCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_RestrictionCode"
codeListValue=" **otherRestrictions** "/>
</gmd:accessConstraints>
<gmd:otherConstraints>
<gmx:Anchor xlink:href="http://inspire.ec.europa.eu/metadata-
codelist/LimitationsOnPublicAccess/noLimitations"> **Es gelten keine
Zugriffsbeschränkungen** </gmx:Anchor>
</gmd:otherConstraints>
</gmd:MD_LegalConstraints>
</gmd:resourceConstraints>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_ 2 .8_beschraenkungOeffZugang.pdf?inline=false
**XPath:**
MD_Metadata/identificationInfo[1]//resourceConstraints/MD_LegalConstraints/useConst
raints


```
 bedingt verpflichtend (falls useConstraints mit „ otherRestrictions “ belegt wurde)
mindestens ein otherConstraints - Element; in welchem die Nutzungs- und
Zugriffsbedingungen sowie Informationen über etwaige Gebühren in Textform oder als
Verweis (URL) zu dokumentieren sind.
```
_Anmerkung: In Anlehnung an die INSPIRE-Anforderung, immer eine Aussage zu Nutzungs- und
Zugriffsbedingungen in den Metadaten zu führen und diese in der GDI-DE ausschließlich und einheitlich
in den ISO-Elementen useConstraints/otherConstraints abzulegen (siehe 2.9.2), wird an dieser Stelle
zwecks Einheitlichkeit auch für diejenigen Ressourcen, die nicht unter die INSPIRE-Richtlinie fallen, als
GDI-DE-Konvention festgelegt, die gleiche Struktur (d. h. die ISO-Elemente
useConstraints/otherConstraints) zu verwenden. Die inhaltliche Belegung ist für Ressourcen, die unter
die INSPIRE-Richtlinie fallen, jedoch restriktiver._

Für den Fall, dass keine Bedingungen gelten oder die Bedingungen unbekannt sind, ist dies ebenfalls
zu dokumentieren. Der Eintrag erfolgt als deutschsprachiger Freitext „Es gelten keine
Bedingungen“ (siehe folgendes Beispiel) oder „Bedingungen unbekannt“.

_Anmerkung: Eine „unbekannte“ Bedingung ist für den Nutzer nicht hilfreich und sollte möglichst
konkretisiert werden._

```
Beispiel mit Nutzungsbedingungen:
<gmd:resourceConstraints>
<gmd:MD_LegalConstraints>
<gmd:useConstraints>
<gmd:MD_RestrictionCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_RestrictionCode"
codeListValue=" otherRestrictions "/>
</gmd:useConstraints>
<gmd:otherConstraints>
< gco:CharacterString> Es gelten die Lizenzbedingungen „Datenlizenz
Deutschland - Namensnennung - Version 2.0“ bzw. „dl-de/by- 2 - 0”
(https://www.govdata.de/dl-de/by- 2 - 0) mit den dort geforderten Angaben zum
Quellenvermerk. Als Rechteinhaber und Bereitsteller ist „Land NRW“, sowie das Jahr
des Datenbezugs in Klammern anzugeben. Beispiel für Quellenvermerk: Land NRW (2017)
Datenlizenz Deutschland - Namensnennung - Version 2.0 (www.govdata.de/dl-de/by- 2 -
0). </gco:CharacterString>
</gmd:otherConstraints>
</gmd:MD_LegalConstraints>
</gmd:resourceConstraints>
```
```
Beispiel für nicht vorliegende Bedingungen:
<gmd:resourceConstraints>
<gmd:MD_LegalConstraints>
<gmd:useConstraints>
<gmd:MD_RestrictionCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_RestrictionCode"
codeListValue=" otherRestrictions "/>
</gmd:useConstraints>
<gmd:otherConstraints>
< gco:CharacterString> Es gelten keine Bedingungen </gco:CharacterString>
</gmd:otherConstraints>
</gmd:MD_LegalConstraints>
</gmd:resourceConstraints>
```

#### 2.9.2 Bedingungen für den Zugang und die Nutzung bei INSPIRE ([INS VO MD], B 8.1)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ (^) ☐
zusätzlich für INSPIRE (^) ☒ ☐ (^) ☐
Dieser Abschnitt beschreibt, wie Nutzungs- und Zugriffsbedingungen im Sinne des INSPIRE-
Elements "Bedingungen für den Zugang und die Nutzung" entsprechend der [INS TG MD] zu erfassen
sind.
Die Bedingungen für den Zugang und die Nutzung sind nach [INS TG MD], 2.3.7 (Requirement C.18),
innerhalb eines gemeinsamen _MD_LegalConstraints_ - Objekts nach einer vorgegebenen Bildungsregel
anzugeben. Für die GDI-DE wird diese zwecks Einheitlichkeit weiter spezifiziert, so dass folgende
Elemente erforderlich sind:
 genau ein _useConstraints_ - Element, Codelisten-Wert " **otherRestrictions** " aus
_MD_RestrictionCode_ ([ISO 19115], B.5.24)
und
 mindestens ein _otherConstraints_ - Element; in welchem die Nutzungs- und
Zugriffsbedingungen sowie Informationen über etwaige Gebühren in Textform oder als
Verweis (URL) zu dokumentieren sind.
_Anmerkung: Seitens INSPIRE besteht die Anforderung, immer eine Aussage zu den Bedingungen für den
Zugang und die Nutzung in den Metadaten zu führen und diese entweder in den ISO-Elementen
useConstraints/otherConstraints oder accessConstraints/otherConstraints abzulegen. Zwecks
Einheitlichkeit in der GDI-DE und zur Abgrenzung von den Beschränkungen des öffentlichen Zugangs
(siehe 2.8) wurde festgelegt, hier ausschließlich die ISO-Elemente useConstraints/otherConstraints zu
verwenden._
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_2.9.1_bedingungenGDIde.pdf?inline=false
**XPath:**
MD_Metadata/identificationInfo[1]//resourceConstraints/MD_LegalConstraints/useConst
raints


Für den Fall, dass keine Bedingungen gelten oder die Bedingungen unbekannt sind, ist dies
entsprechend [INS VO MD], Teil B 8.1, zu dokumentieren. Die Einträge erfolgen gem. [INS TG MD],
2.3.7 (Requirement C.18), als _gmx:Anchor_ - Element mit Verweis auf einen Eintrag in der seitens
INSPIRE bereitgestellten Codeliste ConditionsApplyingToAccessAndUse^5 über die Werte
" **noConditionsApply“** bzw. „ **conditionsUnknown** “ sowie den zugehörigen deutschsprachigen
Texten (siehe folgende Beispiele).

_Anmerkung: Eine „unbekannte“ Bedingung ist für den Nutzer nicht hilfreich und sollte möglichst
konkretisiert werden._

(^5) [http://inspire.ec.europa.eu/metadata-codelist/ConditionsApplyingToAccessAndUse](http://inspire.ec.europa.eu/metadata-codelist/ConditionsApplyingToAccessAndUse)
**Beispiel mit Nutzungsbedingungen:**
<gmd:resourceConstraints>
<gmd:MD_LegalConstraints>
<gmd:useConstraints>
<gmd:MD_RestrictionCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_RestrictionCode"
codeListValue=" **otherRestrictions** "/>
</gmd:useConstraints>
<gmd:otherConstraints>
< gco:CharacterString> **Es gelten die Lizenzbedingungen „Datenlizenz
Deutschland - Namensnennung - Version 2.0“ bzw. „dl-de/by- 2 - 0”
(https://www.govdata.de/dl-de/by- 2 - 0) mit den dort geforderten Angaben zum
Quellenvermerk. Als Rechteinhaber und Bereitsteller ist „Land NRW“, sowie das Jahr
des Datenbezugs in Klammern anzugeben. Beispiel für Quellenvermerk: Land NRW (2017)
Datenlizenz Deutschland - Namensnennung - Version 2.0 (www.govdata.de/dl-de/by- 2 -
0).** </gco:CharacterString>
</gmd:otherConstraints>
</gmd:MD_LegalConstraints>
</gmd:resourceConstraints>
**Beispiel für nicht vorliegende Bedingungen:**
<gmd:resourceConstraints>
<gmd:MD_LegalConstraints>
<gmd:useConstraints>
<gmd:MD_RestrictionCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_RestrictionCode"
codeListValue=" **otherRestrictions** "/>
</gmd:useConstraints>
<gmd:otherConstraints>
<gmx:Anchor xlink:href="http://inspire.ec.europa.eu/metadata-
codelist/ConditionsApplyingToAccessAndUse/noConditionsApply"> **Es gelten keine
Bedingungen** </gmx:Anchor>
</gmd:otherConstraints>
</gmd:MD_LegalConstraints>
</gmd:resourceConstraints>


### 2.10 Regionalschlüssel

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☒
zusätzlich für INSPIRE (^) ☐ (^) ☐ ☐
**Empfehlung:** Geodaten und Geodatendienste, die einen räumlichen Bereich in Form einer
bestimmten Verwaltungseinheit abdecken, können über deren 12 - stelligen Regionalschlüssel (RS)
oder alternativ über die Angabe von NUTS^6 /LAU^7 - Regionen gezielt auffindbar gemacht werden,
wenn der entsprechende Schlüssel in den Metadaten hinterlegt wird. Die Angabe in den Metadaten
ist optional, wird aber empfohlen, um Auswertungen zu ermöglichen.
(^6) _Nomenclature des unités territoriales statistiques_ ist die Klassifikation von räumlichen Bezugseinheiten der amtlichen Statistik in der EU
(^7) _Local Administrative Units_ sind NUTS-Ergänzungen zur Klassifikation von kommunalen Verwaltungsverbänden bzw. Gemeinden
**Beispiel für unbekannte Bedingungen:**
<gmd:resourceConstraints>
<gmd:MD_LegalConstraints>
<gmd:useConstraints>
<gmd:MD_RestrictionCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_RestrictionCode"
codeListValue=" **otherRestrictions** "/>
</gmd:useConstraints>
<gmd:otherConstraints>
<gmx:Anchor xlink:href="http://inspire.ec.europa.eu/metadata-
codelist/ConditionsApplyingToAccessAndUse/conditionsUnknown"> **Bedingungen unbekannt**
</gmx:Anchor>
</gmd:otherConstraints>
</gmd:MD_LegalConstraints>
</gmd:resourceConstraints>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_2.9. 2 _bedingungenINSPIRE.pdf?inline=false
**XPath:**
MD_Metadata/identificationInfo[1]//extent/EX_Extent/geographicElement/EX_Geographic
Description/geographicIdentifier/MD_Identifier/code


Alternativ kann die Kodierung auch in einem _CharacterString_ - Element erfolgen:

```
Beispiel mit Regionalschlüssel-Kodierung:
<gmd:geographicElement>
<gmd:EX_GeographicDescription>
<gmd:geographicIdentifier>
<gmd:MD_Identifier>
<gmd:code>
<gmx:Anchor xlink:href=”https://registry.gdi-
de.org/id/<namespaceRS>/033595407004”> 033595407004 </gmx:Anchor>
</gmd:code>
</gmd:MD_Identifier>
</gmd:geographicIdentifier>
</gmd:EX_GeographicDescription>
</gmd:geographicElement>
```
```
Beispiel mit NUTS/LAU-Kodierung:
<gmd:geographicElement>
<gmd:EX_GeographicDescription>
<gmd:geographicIdentifier>
<gmd:MD_Identifier>
<gmd:code>
<gmx:Anchor xlink:href=”https://registry.gdi-
de.org/id/<namespaceNUTS>/03359004”> 03359004 </gmx:Anchor>
</gmd:code>
</gmd:MD_Identifier>
</gmd:geographicIdentifier>
</gmd:EX_GeographicDescription>
</gmd:geographicElement>
```
```
Beispiel mit Regionalschlüssel-Kodierung:
<gmd:geographicElement>
<gmd:EX_GeographicDescription>
<gmd:geographicIdentifier>
<gmd:MD_Identifier>
<gmd:code>
<gco:CharacterString> 033595407004 </gco:CharacterString>
</gmd:code>
</gmd:MD_Identifier>
</gmd:geographicIdentifier>
</gmd:EX_GeographicDescription>
</gmd:geographicElement>
```
```
Beispiel mit NUTS/LAU-Kodierung:
<gmd:geographicElement>
<gmd:EX_GeographicDescription>
<gmd:geographicIdentifier>
<gmd:MD_Identifier>
<gmd:code>
<gco:CharacterString> 03359004 </gco:CharacterString>
</gmd:code>
</gmd:MD_Identifier>
</gmd:geographicIdentifier>
</gmd:EX_GeographicDescription>
</gmd:geographicElement>
```

Der Regionalschlüssel wird vom Statistischen Bundesamt veröffentlicht [DESTATIS], die NUTS/LAU-
Regionen durch das Statistische Amt der Europäischen Union (kurz Eurostat oder ESTAT).

Die in den Beispielen genannten URL (z. B. https://registry.gdi-
de.org/id/<namespaceRS>/033595407004) enthalten persistente Identifikatoren für den
jeweiligen Schlüssel. Diese verweisen auf einen WFS, der u. a. die Geometrie der Verwaltungseinheit
ausgibt.

### bereitgestellten Daten 2.11 Kennzeichnung der Verbindlichkeit von per Darstellungs- und/oder Downloaddienst

### Downloaddienst bereitgestellten Daten

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☒
zusätzlich für INSPIRE (^) ☐ (^) ☐ ☐
Um in Zukunft rechtsgültige Auskunftssysteme auf Basis von Geodatendiensten zu ermöglichen, soll
die Verbindlichkeit von Daten, die mittels Diensten bereitgestellt werden, automatisiert ausgewertet
werden können. Eine mögliche Ausprägung dieser Verbindlichkeit kann der Status „amtliche
Daten“ sein. Damit Planer und Entscheider unmittelbar erkennen können, inwieweit die
vorliegenden Informationen für die Beantwortung ihrer jeweiligen Fragestellung ausreichend
verbindlich sind, wird eine Information darüber in der Qualitätsaussage in den Metadaten hinterlegt.
Die Angabe der Verbindlichkeit in den Daten- und den Dienst-Metadaten ist optional, wird aber wie
folgt empfohlen:
Unter _dataQualityInfo_ wird im entsprechenden _DQ_ConformanceResult_ - Element in
 _specification_ die rechtliche Grundlage (z. B. Verordnung, gesetzlicher Rahmen) zitiert;
 _explanation_ ein Freitext wie z. B.
 „amtlicher Dateninhalt“,
 „Bei diesen Daten handelt es sich um einen amtlichen Dateninhalt.“ oder
 „Dieser Dienst präsentiert amtliche Daten.“ angegeben;
 _pass_ der Wert „true“ gesetzt, um zu kennzeichnen, dass die benannte Rechtsgrundlage
tatsächlich zu Grunde liegt.
Das folgende Beispiel zeigt, wie die Verbindlichkeit in Bezug auf eine konkrete gesetzliche Regelung
im Metadatensatz abgebildet werden kann:
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_2. 10 _regionalschluessel.pdf?inline=false
**XPath:**
MD_Metadata/dataQualityInfo/DQ_DataQuality/report/DQ_DomainConsistency/result/DQ_Co
nformanceResult


### 2.12 Konformität (Übereinstimmung mit Spezifikationen, [INS VO MD], B 7)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☐
zusätzlich für INSPIRE (^) ☒ ☐ ☐
Gemäß [INS VO MD], B 7 und [INS TG MD], 2.4.1 (Requirements C.20 bis C.2 2 ) ist in den Metadaten
zu dokumentieren, ob die beschriebene Ressource gegenüber einer Spezifikation geprüft wurde und
ob diese Überprüfung erfolgreich war. Grundsätzlich ist die Konformität mindestens bzgl. der jeweils
**Beispiel:**
<gmd:report>
<gmd:DQ_DomainConsistency>
<gmd:result>
<gmd:DQ_ConformanceResult>
<gmd:specification>
<gmd:CI_Citation>
<gmd:title>
<gco:CharacterString> **Verfahrensart: Regelflurbereinigung nach §§ 1,37**
</gco:CharacterString>
</gmd:title>
<gmd:date>
<gmd:CI_Date>
<gmd:date>
<gco:Date"> **2011 - 03 - 03** </gco:Date>
</gmd:date>
<gmd:dateType>
<gmd:CI_DateTypeCode codeList=
"http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#CI_DateTypeCode"
codeListValue=" **revision** "/>
</gmd:dateType>
</gmd:CI_Date>
</gmd:date>
</gmd:CI_Citation>
</gmd:specification>
<gmd:explanation>
<gco:CharacterString> **amtlicher Dateninhalt** </gco:CharacterString>
</gmd:explanation>
<gmd:pass>
<gco:Boolean> **true** </gco:Boolean>
</gmd:pass>
</gmd:DQ_ConformanceResult>
</gmd:result>
</gmd:DQ_DomainConsistency>
</gmd:report>
**ATS:**

_- derzeit kein spezifischer Test vorgesehen -_

```
XPath:
MD_Metadata/dataQualityInfo/DQ_DataQuality/report/DQ_DomainConsistency/result/DQ_Co
nformanceResult
```

relevanten Durchführungsbestimmung anzugeben. Mit der Aussage zur Konformität wird
ausgedrückt, ob

```
 die Daten bereits im INSPIRE-Datenmodell vorliegen und bereitgestellt werden (Daten-
Metadaten: Übereinstimmung mit der Durchführungsbestimmung zur Interoperabilität, IR
1089/2010);
 der Dienst die Vorgaben (Funktionen, Performanz, Capabilities etc.) für Netzdienste einhält
(Dienst-Metadaten: Übereinstimmung mit der Durchführungsbestimmung zu Netzdiensten,
IR 976/2009);
```
In zusätzlichen Elementen können weitere Spezifikationen wie z. B. Änderungsverordnungen, die die
Durchführungsbestimmungen betreffen, sowie Technical Guidance-Dokumente, z. B.
Datenspezifikationen oder zu Darstellungs- bzw. Downloaddiensten, referenziert werden.

Die Informationen werden je zitierter Spezifikation in einem eigenen _DQ_ConformanceResult_ -
Element mit _specification_ , _explanation_ und _pass_ ([ISO 19115], B.2.4.4, No. 129 bis No. 132) angegeben:

```
 specification - Element: Für den Titel der Spezifikation wird das title - Element ([ISO 19115],
B.3.2.1, No. 360) aus CI_Citation verwendet. Das Element kann als Freitext
(gco:CharacterString) oder Verweis (gmx:Anchor mit xlink:href auf einen seitens der EU
festgelegten Link plus Freitext) codiert werden. Die Abschnitte 3.5 (für Datensätze und -
serien) bzw. 4.6 (für Netzdienste) regeln Benennung und Schreibweise der jeweiligen
Durchführungsbestimmung, die zusammen mit dem angegebenen Veröffentlichungsdatum
zu verwenden ist. Dort ist auch der jeweilige Link für den Verweis mittels gmx:Anchor
dokumentiert und Beispiele abgebildet. Im Anhang 1: INSPIRE-Spezifikationen
(Durchführungsbestimmungen) sind die in Frage kommenden INSPIRE
Durchführungsbestimmungen abermals aufgelistet.
 explanation - Element: Hier kann grundsätzlich Freitext eingetragen werden. Beispielsweise
können Angaben zu den verwendeten Anwendungen bei der Überprüfung der Konformität
gemacht werden (siehe Kapitel 7 ).
 pass- Element: Gemäß [ISO 19115] ist der Wertebereich von pass auf 0 (= nein) und 1 (= ja)
festgelegt. INSPIRE definiert abweichend davon, aber in Übereinstimmung mit [ISO 19139],
die zulässigen Werte als true und false. Wurde die Übereinstimmung mit der Spezifikation
noch nicht überprüft, kann das Element leer bleiben, sofern im pass- Element das Attribut
nilReason=“unknown“ angegeben wird.
```

## 3 Konventionen für Metadaten zu Datenbeständen und Anwendungen

Die Konventionen in diesem Kapitel betreffen die Metadaten zu allen Ressourcen in der GDI-DE, die
keine Dienste sind, d. h. deren Inhalt im _hierarchyLevel_ - Element ungleich „service“ ist (siehe 2.3).
Somit fallen auch Metadaten zu Anwendungen (z. B. Portale) darunter, deren Metadatenstruktur in
ISO 19115 analog zu Metadaten zu Datenbeständen geregelt ist.

### 3.1 Eindeutiger Ressourcenidentifikator ([INS VO MD], B 1.5)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☒ (^) ☐ ☐
zusätzlich für INSPIRE (^) ☐ (^) ☐ ☐
Die Angabe des eindeutigen Ressourcenidentifikators erfolgt im _identificationInfo_ - Element (ISO
19115, B.2.1, No. 15). Gemäß den INSPIRE-Vorgaben in [INS TG MD], 3.1.2.1, Requirement 1.3, ist
dieser aus einem **Namensraum** ( **namespace** ) und einem lokalen **Identifikator** ( **localID** ) zu bilden.
Der lokale Identifikator ist eine Zeichenkette und wird i. d. R. vom Eigentümer der Daten vergeben.
Der Namensraum, z. B. der Organisation, definiert den Kontext, in dem der lokale Identifikator
vergeben wird. Innerhalb eines Namensraumes identifiziert ein lokaler Identifikator eindeutig eine
Ressource ([INS VO MD], B.1.5; [INS Generic Conceptual Model], 14.2).
Für die Bildung des eindeutigen Ressourcenidentifikators gelten folgende Regeln:

1. Der Ressourcenidentifikator ist ein gültiger „Unique Resource Identifier“ (URI) [RFC 3986].
2. Die Abbildung des Ressourcenidentifikators erfolgt über das _MD_Identifier/code_ - Element
    (ISO 19115, B.2.7.3, No. 205/207)^8.
3. Der _code_ wird aus Namensraum und lokalem Identifikator zusammengesetzt. Hierfür wird
    die localID an den namespace angehängt, getrennt durch „/“ (namespace/localId).
_4._ Nach Möglichkeit soll der verwendete Namensraum über die GDI-DE Registry^9 verwaltet
    werden. Weitere Informationen dazu sind im GDI-DE Wiki^10 zu finden.

_Hinweis: Der im Beispiel genannte Namensraum „_ **_https://registry.gdi-de.org/id/de.nw_** _“ ist ein Platzhalter.
Dieser setzt sich aus einem für alle Namensräume festgelegten Prefix (z. B. https://registry.gdi-
de.org/id/ ) und einem domänenspezifischen Teil (z. B. „de.nw“) zusammen. Der domänenspezifische
Teil entsteht erst durch Registrierung des Namensraums in der GDI-DE Registry._

(^8) Das queryable ‚ResourceIdentifier‘ wird lt. [OGC CSW ISO AP] auf MD_Identifier/code abgebildet.
(^9) https://registry.gdi-de.org/
(^10) _https://wiki.gdi-de.org/display/REGISTRYDE/Namensraum-Register_
**XPath:**
MD_Metadata/identificationInfo[1]/MD_DataIdentification/citation/CI_Citation/identi
fier/MD_Identifier


### 3.2 Schlüsselwörter

#### 3.2.1 Quellenangabe für Schlüsselwörter zu INSPIRE-Themen.......................................................

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ (^) ☐
zusätzlich für INSPIRE (^) ☒ ☐ ☐
In Metadaten zu INSPIRE-Datensätzen oder -serien ist nach [INS TG MD], 3.1.2.2 (Requirement 1.4)
die Angabe mindestens eines Schlüsselworts notwendig, das dem Thesaurus „GEMET - INSPIRE
themes“ entstammt. Dieser Thesaurus ist zudem nach [INS TG MD], 2.3.5 (Requirement C.15) als
Quellenangabe anzugeben bzw. zu bennen.
Für die Metadaten in der GDI-DE werden die Anforderungen an die Quellenangabe wie folgt
präzisiert, um die Einheitlichkeit der Metadaten zu fördern und Weiterverwendungen im EU-Kontext
zu unterstützen:
 _title_ - Element: „GEMET - INSPIRE themes, version 1.0“
 _date_ - Element: „2008- 06 - 01“ mit _dateType_ =“publication“
**Beispiel:**
<gmd:identificationInfo>
<gmd:MD_DataIdentification>
<gmd:citation>
<gmd:CI_Citation>
...
<gmd:identifier>
<gmd:MD_Identifier>
<gmd:code>
<gco:CharacterString> **https://registry.gdi-de.org/id/de.nw/DENWAT01**
</gco:CharacterString>
</gmd:code>
</gmd:MD_Identifier>
</gmd:identifier>
...
</gmd:CI_Citation>
</gmd:citation>
...
</gmd:MD_DataIdentification>
</gmd:identificationInfo>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_ 3. 1 _ressourcenidentifikator.pdf?inline=false
**XPath:**
MD_Metadata/identificationInfo[1]/MD_DataIdentification/descriptiveKeywords/*/thesa
urusName


#### 3.2.2 Schlüsselwort „opendata“

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☒ (^) ☐
zusätzlich für INSPIRE (^) ☐ ☐ (^) ☐
**Bedingung für das Gelten dieser Konvention:** Die zu beschreibende Ressource fällt unter Open
Data.
**Beispiel:**
<gmd:descriptiveKeywords>
<gmd:MD_Keywords>
<gmd:keyword>
<gco:CharacterString> **Gewässernetz** </gco:CharacterString>
</gmd:keyword>
...
<gmd:thesaurusName>
<gmd:CI_Citation>
<gmd:title>
<gco:CharacterString> **GEMET - INSPIRE themes, version 1.0**
</gco:CharacterString>
</gmd:title>
<gmd:date>
<gmd:CI_Date>
<gmd:date>
<gco:Date> **2008 - 06 - 01** </gco:Date>
</gmd:date>
<gmd:dateType>
<gmd:CI_DateTypeCode codeList=
"http://standards.iso.org/iso/19139/resources/codelist/gmxCodelists.xml#CI_DateType
Code" codeListValue=" **publication** "/>
</gmd:dateType>
</gmd:CI_Date>
</gmd:date>
...
</gmd:CI_Citation>
</gmd:thesaurusName>
</gmd:MD_Keywords>
</gmd:descriptiveKeywords>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_ 3. 2. 1 _quellenangabeINSPIRE.pdf?inline=false
**XPath:**
MD_Metadata/identificationInfo[1]/MD_DataIdentification/descriptiveKeywords/*/keywo
rd


Metadaten zu Datensätzen und -serien, die über den Geodatenkatalog.de für GovData bereitgestellt
werden sollen, müssen im _keyword_ - Element ([ISO 19115], B.2.2.3, No. 53) das Schlüsselwort
„ **opendata** “ enthalten.

Das Schlüsselwort „opendata“ ist keinem Thesaurus entnommen und wird ohne Quellenangabe in
den Metadaten geführt.

### 3.3 Themenkategorie nach ISO (Zuordnung zum INSPIRE-Thema: [INS VO MD], B 2.1)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☐
zusätzlich für INSPIRE (^) ☒ ☐ ☐
In Metadaten zu Datensätzen oder -serien ist die Angabe mindestens einer ISO-Themenkategorie
notwendig ([ISO 19115], [INS VO MD], Teil B, 2.1^11 , [INS TG MD], 3.1.2.5, Requirement 1.7). Um für
INSPIRE darüber hinaus eine sachlich und inhaltlich richtige Zuordnung von INSPIRE-Themen zu
ISO-Themenkategorien zu gewährleisten, die durch [INS VO MD], Teil D vorgegeben ist, ist die
Zuordnungstabelle aus
(^11) Nicht anwendbar auf Metadaten, die Dienste beschreiben
**Beispiel für unbekannte Bedingungen:**
<gmd:descriptiveKeywords>
<gmd:MD_Keywords>
<gmd:keyword>
<gco:CharacterString> **opendata** </gco:CharacterString>
</gmd:keyword>
</gmd:MD_Keywords>
</gmd:descriptiveKeywords>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_3. 2. 2 _schluesselwortOpendata.pdf?inline=false
**XPath:**
MD_Metadata/identificationInfo[1]/MD_DataIdentification/topicCategory


anzuwenden. Dabei ist in der XML-Abbildung stets die Schreibweise der Spalte ISO-
Themenkategorie – EN zu verwenden.

Handelt es sich beispielsweise um das INSPIRE-Thema Gewässernetz (entscheidend ist die Angabe
von INSPIRE-Themen und deren Schreibweise gem. GEMET in den Schlüsselwörtern), ist hier die
zugehörige ISO-Themenkategorie „inlandWaters“ (Binnengewässer) anzugeben:

### 3.4 Ressourcenverweis für Datensätze und –serien (transferOptions, [INS VO MD], B 1.4)

### MD], B 1.4)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☐
zusätzlich für INSPIRE (^) ☐ ☒ (^) ☐
**Bedingung für das Gelten dieser Konvention:** Die für INSPIRE zu beschreibende Ressource bzw.
zu beschreibenden Informationen hierzu sind online zugänglich.
Aufgrund der INSPIRE-Vorgaben ([INS VO MD], B.1.4) sind die Ressourcenverweise in den Metadaten
für Datensätze und -serien bedingt verpflichtend. Diese müssen angegeben werden, falls solche
Ressourcen (s. u.) vorhanden bzw. zugänglich sind. Gemäß [INS TG MD], 3.1.3.1 (Requirement 1.8)
ist der Zugriffspunkt unter _transferOptions_ (ISO 19115, B.2.10.1, No. 270 _MD_Distribution_ / No. 274
_MD_DigitalTransferOptions_ ) einzutragen.
Im _CI_OnlineResource_ - Element soll gemäß [INS TG MD], 3.1.3.1 (Recommendation 1.9) eine gültige
URL auf eine der folgenden Ressourcen hinterlegt werden:
 eine Möglichkeit zum direkten Download der beschriebenen Daten
 ein Capabilities-Dokument eines Dienstes
 eine WSDL-Datei (SOAP-Binding)
 eine Client-Anwendung, die einen direkten Zugriff auf den beschriebenen Datensatz gewährt
 eine Webseite, die weitere Anleitungen bzw. Informationen enthält
Die Funktion der hinterlegten URL in _CI_OnlineResource_ kann im _function_ - Element über die Begriffe
der Codeliste B.5.3 _CI_OnLineFunctionCode_ aus [ISO 19115] annotiert werden. Dies wird durch [INS
TG MD], 3.1.3.1 (Recommendation 1.8) empfohlen, ist aber nicht verpflichtend. Eine naheliegende
**Beispiel:**
<gmd:topicCategory>
<gmd:MD_TopicCategoryCode> **inlandWaters** </gmd:MD_TopicCategoryCode>
</gmd:topicCategory>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_ 3. 3 _themenkategorieISO_INSPIRE.pdf?inline=false
**XPath:**
MD_Metadata/distributionInfo/MD_Distribution/transferOptions/MD_DigitalTransferOpti
ons/onLine/CI_OnlineResource/linkage/URL


und sinnvolle Verwendung in Metadaten zu Datensätzen und -serien wird dabei für folgende Begriffe
der Codeliste gesehen:

```
 information - für den Link auf eine Webseite, die weitere Anleitungen bzw. Informationen
enthält
 download - für den Link zum unmittelbaren Herunterladen der beschriebenen Daten.
```
_Hinweis: Die Hinterlegung eines Links zum direkten Download der beschriebenen Daten (s. o.) entbindet
nicht von der Verpflichtung seitens INSPIRE, einen Datenbestand per Downloaddienst (z. B. WFS oder
Atom-Feed) verfügbar zu machen und diesen mittels eines eigenen Dienst-Metadatensatzes zu
dokumentieren._

_Hinweis: Das im Beispiel verwendete Element „name“ ist optional und unterliegt nicht der hier
dokumentierten GDI-DE-Konvention. In diesem Element kann der hinterlegte Link (zusätzlich zur
Kennzeichnung im Element „function“) näher erläutert werden._

### 3.5 Konformität (Übereinstimmung mit Spezifikationen, [INS VO MD], B 7)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☐
zusätzlich für INSPIRE (^) ☒ (^) ☐ ☐
**Beispiel:**
<gmd:transferOptions>
<gmd:MD_DigitalTransferOptions>
<gmd:onLine>
<gmd:CI_OnlineResource>
<gmd:linkage>
<gmd:URL> **[http://www.bezreg-](http://www.bezreg-)
koeln.nrw.de/brk_internet/geobasis/landschaftsmodelle/atkis_basis/index.html**
</gmd:URL>
</gmd:linkage>
<gmd:name>
<gco:CharacterString> **Weitere Informationen zum Inhalt der beschriebenen
Daten** </gco:CharacterString>
</gmd:name>
<gmd:function>
<gmd:CI_OnLineFunctionCode
codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#CI_OnLineFu
nctionCode" codeListValue=" **information** "/>
</gmd:function>
</gmd:CI_OnlineResource>
</gmd:onLine>
</gmd:MD_DigitalTransferOptions>
</gmd:transferOptions>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_ 3. 4 _ressourcenverweisDatensatzSerie.pdf?inline=false


Ergänzend zu den grundsätzlichen Konventionen zur Konformitätsaussage in 2.12 wird an dieser
Stelle das Zitat der anzugebenden Spezifikation geregelt. In Metadaten zu INSPIRE-Datensätzen oder

- serien ist gem. [INS TG MD], 3.1.4.2, Requirement 1.10 die Verordnung 1089/2010
(Interoperabilität von Geodatensätzen und -diensten) zu zitieren, um dokumentieren, ob die Daten
bereits im INSPIRE-Datenmodell vorliegen.

Dazu sind folgende Angaben erforderlich:

```
 Titel: VERORDNUNG (EG) Nr. 1089/2010 DER KOMMISSION vom 23. November 2010
zur Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments und des
Rates hinsichtlich der Interoperabilität von Geodatensätzen und -diensten
 Veröffentlichungsdatum: 2010 - 12 - 08
```
Für die empfohlene Referenzierung mittels gmx:Anchor ([INS TG MD], 3.1.4.2, Recommendation
1 .1 0 ) ist für die genannte Durchführungsbestimmung [http://data.europa.eu/eli/reg/2010/1089](http://data.europa.eu/eli/reg/2010/1089)
zu verwenden (siehe zweites Beispiel).

```
XPath:
MD_Metadata/dataQualityInfo/DQ_DataQuality/report/DQ_DomainConsistency/result/DQ_Co
nformanceResult
```
```
Beispiel mit Angabe der Spezifikation in Textform:
<gmd:DQ_ConformanceResult>
<gmd:specification>
<gmd:CI_Citation>
<gmd:title>
<gco:CharacterString> VERORDNUNG (EG) Nr. 1089/2010 DER KOMMISSION vom 23.
November 2010 zur Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments
und des Rates hinsichtlich der Interoperabilität von Geodatensätzen und -
diensten </gco:CharacterString>
</gdm:title>
<gdm:date>
<gmd:CI_Date>
<gmd:date>
<gco:Date> 2010 - 12 - 08 </gco:Date>
</gmd:date>
<gmd:dateType>
<gmd:CI_DateTypeCode
codeList="http://standards.iso.org/iso/19139/resources/codelist/gmxCodelists.xml#CI
_DateTypeCode" codeListValue=" publication "/>
</gmd:dateType>
</gmd:CI_Date>
</gmd:date>
</gmd:CI_Citation>
</gmd:specification>
<gmd:explanation>
<gco:CharacterString> Die Daten wurden mit dem EU-Validator überprüft.
</gco:CharacterString>
</gmd:explanation>
<gmd:pass>
<gco:Boolean> true </gco:Boolean>
</gmd:pass>
</gmd:DQ_ConformanceResult>
```

### 3.6 Nutzungsbedingungen und Lizenzinformationen für Open Data

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☒ (^) ☐
zusätzlich für INSPIRE (^) ☐ ☐ ☐
**Bedingung für das Gelten dieser Konvention** : Die zu beschreibende Ressource fällt unter Open
Data.
**Beispiel mit Angabe der Spezifikation als Verweis :**
<gmd:DQ_ConformanceResult>
<gmd:specification>
<gmd:CI_Citation>
<gmd:title>
<gmx:Anchor xlink:href="http://data.europa.eu/eli/reg/2010/1089"> **VERORDNUNG
(EG) Nr. 1089/2010 DER KOMMISSION vom 23. November 2010 zur Durchführung der
Richtlinie 2007/2/EG des Europäischen Parlaments und des Rates hinsichtlich der
Interoperabilität von Geodatensätzen und -diensten** </gmx:Anchor>
</gdm:title>
<gdm:date>
<gmd:CI_Date>
<gmd:date>
<gco:Date> **2010 - 12 - 08** </gco:Date>
</gmd:date>
<gmd:dateType>
<gmd:CI_DateTypeCode
codeList="http://standards.iso.org/iso/19139/resources/codelist/gmxCodelists.xml#CI
_DateTypeCode" codeListValue=" **publication** "/>
</gmd:dateType>
</gmd:CI_Date>
</gmd:date>
</gmd:CI_Citation>
</gmd:specification>
<gmd:explanation>
<gco:CharacterString> **Die Daten wurden mit dem EU-Validator überprüft.**
</gco:CharacterString>
</gmd:explanation>
<gmd:pass>
<gco:Boolean> **true** </gco:Boolean>
</gmd:pass>
</gmd:DQ_ConformanceResult>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_ 3. 5 ._konformitaet.pdf?inline=false
**XPath:**
MD_Metadata/identificationInfo[1]/MD_DataIdentification/resourceConstraints/MD_Lega
lConstraints/useConstraints


Dieser Abschnitt beschreibt, wie Nutzungsbedingungen bzw. Lizenzinformationen zu Open Data in
den Metadaten der GDI-DE dokumentiert werden, um zentral bzw. einheitlich dem GovData-Portal
bereitgestellt und dort verarbeitet werden zu können.

Die Angaben zur Lizenz werden zunächst als Nutzungsbedingung erfasst, wie es grundsätzlich in
2.9.1 (Nicht-INSPIRE) bzw. 2.9.2 (bei gleichzeitiger Relevanz für INSPIRE) beschrieben ist.

Darüber hinaus sind die Lizenzinformationen in einem zusätzlichen _otherConstraints_ - Element (im
selben _MD_LegalConstraints_ ) im Datenformat JSON (JavaScript Object Notation) strukturiert
anzugeben: Die einzelnen Paare, gebildet aus Parametername und -wert, werden durch Kommata
getrennt und in geschweiften Klammern eingeschlossen, angegeben. JSON eignet sich an dieser Stelle,
da der relevante Bereich innerhalb des Freitextfeldes recht einfach identifiziert und ausgewertet
werden kann. Mischformen aus JSON und Freitext innerhalb eines _otherConstraints_ - Element müssen
zur Vermeidung von Fehlinterpretationen verhindert werden. Mindestens folgende Parameter sollen
bei der Lizenzbeschreibung gesetzt werden:

```
 id: Identifier der Lizenz^12
 name: Name der Lizenz 13
 url: URL, unter welcher der Lizenztext bezogen werden kann 14
 quelle: Text der Namensnennung, unter welcher die Datenquelle bei einer Weiternutzung
zitiert werden soll
```
(^12) gem. Liste unter https://www.dcat-ap.de/def/licenses/, Spalte „Lizenzcode“
(^13) gem. Liste unter https://www.dcat-ap.de/def/licenses/, Spalte „Name“
(^14) gem. Liste unter https://www.dcat-ap.de/def/licenses/, Spalte „Lizenztext“
**Beispiel mit Nutzungsbedingungen und Lizenzinformationen für Open Data:**
<gmd:resourceConstraints>
<gmd:MD_LegalConstraints>
<gmd:useConstraints>
<gmd:MD_RestrictionCode
codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#MD_Restrict
ionCode" codeListValue=" **otherRestrictions** "/>
</gmd:useConstraints>
<gmd:otherConstraints>
< gco:CharacterString> **Dieser Datensatz kann gemäß der „Nutzungsbestimmungen
für die Bereitstellung von Geodaten des Bundes“
(http://www.geodatenzentrum.de/docpdf/geonutzv.pdf) genutzt werden.**
</gco:CharacterString>
</gmd:otherConstraints>
<gmd:otherConstraints>
< gco:CharacterString>
**{
"id": " geoNutz/20130319",
"name": "Nutzungsbestimmungen für die Bereitstellung von Geodaten des Bundes",
"url": "http://www.geodatenzentrum.de/docpdf/geonutzv.pdf",
"quelle": "Quelle: © GeoBasis-DE / BKG <Jahr des letzten Datenbezugs>"
}**
</gco:CharacterString>
</gmd:otherConstraints>
</gmd:MD_LegalConstraints>
</gmd:resourceConstraints>


### 3.7 Formatangaben

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☐
zusätzlich für INSPIRE (^) ☒ (^) ☐ ☐
Gemäß [INS VO Interop], Art. 13 (3) und [INS TG MD], 3.2.3.1 (Requirement 2.6) ist in den Metadaten
zu dokumentieren, in welchem Format (die [INS VO Interop] beschreibt dies als
„Programmiersprachenkonstrukt“) die Daten vorliegen. Dies fokussiert auf das Dateiformat und
weniger auf die logische Struktur der enthaltenen Daten. In der [INS TG MD] wird dies im Anhang
unter C.3.3 am gewählten Beispiel für eine GML-Datei deutlich. Gegenstand der hier beschriebenen
Konvention ist nicht die verpflichtende Formatangabe selbst (diese Verpflichtung gilt unverändert),
sondern die Betonung der Aussage im Kommentar unter [INS TG MD], Anhang C.3.3:
**Empfehlung:** Die Formatangabe durch die Elemente _name_ und _version_ unter _MD_Format_ ist
ausreichend. Informationen über die zugrundeliegende logische Datenstruktur (z. B. eine INSPIRE-
Datenspezifikation) sollte entgegen dem Beispiel 3.18 der [INS TG MD] nicht begleitend im
_specification-_ Element unter _MD_Format_ , sondern als eigenständige Information im separaten Zweig
_MD_ApplicationSchemaInformation_ der [ISO 19115] geführt werden.
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_ 3. 6 _bedingungen_lizenzOpendata.pdf?inline=false
**XPath:**
MD_Metadata/distributionInfo/MD_Distribution/distributionFormat/MD_Format
MD_Metadata/applicationSchemaInfo/MD_ApplicationSchemaInformation


## 4 Konventionen für Metadaten zu Diensten

Die Konventionen in diesem Kapitel betreffen die Metadaten zu allen Diensten in der GDI-DE, d. h.
die Dienste, deren Inhalt im _hierarchyLevel_ - Element gleich „service“ ist (siehe 2.3).

### 4.1 Schlüsselwörter

#### 4.1.1 Schlüsselwörter zu Dienstkategorien bei INSPIRE

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☐
zusätzlich für INSPIRE (^) ☒ ☐ ☐
In Metadaten zu Diensten für INSPIRE ist die Angabe mindestens eines Schlüsselworts erforderlich,
das aus dem Teil D (Ziffer 4) der [INS VO MD] stammt ([INS VO MD], Teil B, 3, [INS TG MD], 4.1.2.2,
Requirement 3. 4 ). Diese Verpflichtung gilt unverändert.
**Empfehlung** : Zur Förderung der Einheitlichkeit und der eindeutigen Interpretierbarkeit der
Metadaten sollen in der GDI-DE in Abhängigkeit der Art des jeweils zu dokumentierenden Dienstes
folgende Schlüsselwörter verwendet werden:
**Art des Dienstes Schlüsselwort**
WMS, WMTS infoMapAccessService
WFS, predefinedAtom (Vektor) infoFeatureAccessService
WFS-G infoGazetteerService
WCS, predefinedAtom (Raster) infoCoverageAccessService
CSW infoCatalogueService
Sensordienste infoSensorDescriptionService
Anwendung zum Suchen von Geodatenbeschreibungen humanCatalogueViewer
**XPath:**
MD_Metadata/identificationInfo[1]/SV_ServiceIdentification/descriptiveKeywords/*/ke
yword
**Beispiel:**
<gmd:descriptiveKeywords>
<gmd:MD_Keywords>
<gmd:keyword>
<gco:CharacterString> **humanCatalogueViewer** </gco:CharacterString>
</gmd:keyword>
</gmd:MD_Keywords>
</gmd:descriptiveKeywords
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_4.1.1_schluesselwortDienst.pdf?inline=false


### 4.2 Verlinkung zum verwendeten Datenbestand (Daten-Dienste-Kopplung)

#### 4.2.1 Gekoppelte Daten-Ressource ([INS VO MD], B 1.6)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☒ (^) ☐
zusätzlich für INSPIRE (^) ☐ ☐ (^) ☐
**Bedingung für das Gelten dieser Konvention:** Es besteht eine Verbindung zu einer ebenfalls mit
Metadaten beschriebenen Datenquelle.
Das INSPIRE-Element „Gekoppelte Ressource / Coupled resource“ ([INS VO MD], B.1.6; [INS TG MD],
4.1.2.4, Requirement 3.6) wird verwendet, um die Beziehung zwischen Dienst und zugehörigem
Datensatz bzw. zugehörigen Datensätzen auszudrücken. Die Referenzen auf die vom Dienst
bereitgestellten Datensätze werden dabei im _operatesOn_ - Element (ISO 19119, C.1, No. 9) angegeben.
Dies entspricht dem grundsätzlichen Prinzip der Daten-Dienste-Kopplung in der GDI-DE (vgl. Kapitel
5 ) und gilt für alle Metadaten in der GDI-DE.
Laut ([INS VO MD], B.1.6; [ISO 19119]) kennzeichnet dieses Element den bereitgestellten Datensatz
durch den eindeutigen Ressourcenidentifikator (URI) des Datensatzes (siehe 3.1). Gemäß [INS TG
MD] soll die Referenz dabei jedoch auf ein _MD_DataIdentification_ - Objekt eines Daten-
Metadatensatzes verweisen.
Da nach [INS VO MD] die Art der Bezugnahme auf die Daten-Metadaten nicht eindeutig vorgegeben
ist, wird für die Gewährleistung der Interoperabilität innerhalb der GDI-DE die Festlegung getroffen,
auflösbare URLs zu verwenden. Hierfür kann die GDI-DE Registry^15 verwendet werden. Zu den dort
registrierten Namensräumen kann jeweils ein Muster für einen Dienst-Aufruf hinterlegt werden.
Beim Aufruf der Referenz wird von der GDI-DE Registry eine Weiterleitung z. B. auf die hinterlegte
URL mit einem _GetRecords_ - Aufruf eines CSW durchgeführt. Weitere Informationen dazu sind im GDI-
DE Wiki^16 zu finden.
(^15) https://registry.gdi-de.org/
(^16) https://wiki.gdi-de.org/display/REGISTRYDE/Namensraum-Register
**XPath:**
MD_Metadata/identificationInfo[1]/SV_ServiceIdentification/operatesOn/ @xlink:href
**Beispiel:**
<gmd:identificationInfo>
<srv:SV_ServiceIdentification>
...
<srv:operatesOn xlink:href=" **https://registry.gdi-de.org/id/de.nw/DENWAT01** "/>
</srv:SV_ServiceIdentification>
</gmd:identificationInfo>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_4.2.1_verlinkungDatenbestand.pdf?inline=false


#### 4.2.2 Art der Kopplung zwischen Dienst und zugehörigen Daten

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☒ ☐
zusätzlich für INSPIRE (^) ☐ ☐ ☐
**Bedingung für das Gelten dieser Konvention:** Es besteht eine Verbindung zu einer ebenfalls mit
Metadaten beschriebenen Datenquelle.
In den Dienst-Metadaten ist neben den verknüpften Daten-Metadaten auch die Art der Kopplung
anzugeben (ISO 19119, _SV_CouplingType_ ). Dabei sind die Werte „eng“ (tight), „gemischt“ (mixed) und
„lose“ (loose) zulässig.
Es ist davon auszugehen, dass in der Regel ein WMS „eng“ (tight), kaskadierende Dienste
„gemischt“ (mixed) und Downloaddienste ebenfalls „eng“ (tight) gekoppelt sind. Je nach Struktur der
Katalogtopologie können Suchdienste sowohl „lose“, „eng“ oder „gemischt“ gekoppelt sein.

### 4.3 Ressourcenverweise für Dienste

#### 4.3.1 Ressourcenverweis unter transferOptions ([INS VO MD], B 1.4)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☐
zusätzlich für INSPIRE (^) ☐ ☒ (^) ☐
**Bedingung für das Gelten dieser Konvention:** Die für INSPIRE zu beschreibende Ressource bzw.
Informationen dazu sind online zugänglich.
**XPath:**
MD_Metadata/identificationInfo[1]/SV_ServiceIdentification/couplingType/SV_Coupling
Type
**Beispiel:**
<srv:couplingType>
<srv:SV_CouplingType
codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#SV_Coupling
Type" codeListValue=" **tight** "> **tight** </srv:SV_CouplingType>
<srv:couplingType>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_4.2.1_verlinkungDatenbestand.pdf?inline=false
**XPath:**
MD_Metadata/distributionInfo/MD_Distribution/transferOptions/MD_DigitalTransferOpti
ons/onLine/CI_OnlineResource/linkage/URL


Aufgrund der INSPIRE-Vorgaben ([INS VO MD], B.1.4) sind die Ressourcenverweise in den Metadaten
für Dienste bedingt verpflichtend. Diese müssen angegeben werden, falls solche Ressourcen (s. u.)
vorhanden bzw. zugänglich sind. Gemäß [INS TG MD], 4.1.3.1 (Requirement 3.7) ist der Zugriffspunkt
unter _transferOptions_ (ISO 19115, B.2.10.1, No. 270 _MD_Distribution_ / No. 274
_MD_DigitalTransferOptions_ ) einzutragen.

Im _CI_OnlineResource_ - Element soll gemäß [INS TG MD], 4 .1.3.1 (Recommendation 3.5) eine gültige
URL auf eine der folgenden Ressourcen hinterlegt werden:

```
 ein Capabilities-Dokument eines Dienstes
 eine WSDL-Datei (SOAP-Binding)
 eine Webseite, die weitere Anleitungen bzw. Informationen enthält
```
Handelt es sich bei der Ressource um einen Atom-Download-Dienst, so ist hier die URL des Service
Feed einzutragen.

Die Funktion der hinterlegten URL in _CI_OnlineResource_ kann im _function_ - Element über die Begriffe
der Codeliste B.5.3 _CI_OnLineFunctionCode_ aus [ISO 19115] annotiert werden. Dies wird durch [INS
TG MD], 4.1.3.1 (Recommendation 3.4) empfohlen, ist aber nicht verpflichtend. Eine naheliegende
und sinnvolle Verwendung in Metadaten zu Diensten wird dabei für folgenden Begriff der Codeliste
gesehen:

```
 information – für den Link auf das Capabilities-Dokument des Dienstes oder eine Webseite,
die weitere Anleitungen bzw. Informationen enthält
```
```
Beispiel:
<gmd:transferOptions>
<gmd:MD_DigitalTransferOptions>
<gmd:onLine>
<gmd:CI_OnlineResource>
<gmd:linkage>
<gmd:URL>
http://www.wms.nrw.de/geobasis/wms_nw_dtk10?REQUEST=GetCapabilities&SERVICE=wms&VER
SION=1.3.0 </gmd:URL>
</gmd:linkage>
<gmd:function>
<gmd:CI_OnLineFunctionCode
codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#CI_OnLineFu
nctionCode" codeListValue=" information "/>
</gmd:function>
</gmd:CI_OnlineResource>
</gmd:onLine>
</gmd:MD_DigitalTransferOptions>
</gmd:transferOptions>
```
```
ATS:
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_4.3.1_ressourcenverweisTransferOptions.pdf?inline=fa
lse
```

#### 4.3.2 Ressourcenverweis unter connectPoint

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☒ ☐ (^) ☐
zusätzlich für INSPIRE (^) ☐ ☐ (^) ☐
Für jeden Dienst-Metadatensatz gilt, dass die URL zum Dienst unter _connectPoint_ ([ISO 19119], Table
C.2 No. 6) geführt werden muss. Hier ist die URL einzutragen, unter der das Capabilities-Dokument
bzw. der Service Feed des Dienstes (Atom) bezogen werden kann (siehe auch Kapitel 5 ).
Begleitet wird diese Angabe vom _operationName_ - Element, das z. B. aussagt, dass es sich bei dem
angegebenen Link um ein Anfordern des Capabilities-Dokumentes handelt. Unter dem XML-Element
„gmd:URL“ wird in diesem Fall kein kompletter GetCapabilities-Request abgelegt. Bei Atom-Feeds ist
für _operationName_ ein entsprechender Wert, z. B. „Download“, zu setzen.

### 4.4 Art des Geodatendienstes bei INSPIRE ([INS VO MD], B 2.2)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ (^) ☐ ☐
**XPath:**
MD_Metadata/identificationInfo[1]/SV_ServiceIdentification/containsOperations/SV_Op
erationMetadata/connectPoint/CI_OnlineResource/linkage/URL
**Beispiel:**
<srv:containsOperations>
<srv:SV_OperationMetadata>
<srv:operationName>
<gco:CharacterString> **GetCapabilities** </gco:CharacterString>
</srv:operationName>
<srv:DCP>
<srv:DCPList
codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#DCPList"
codeListValue=" **WebServices** "/>
</srv:DCP>
<srv:connectPoint>
<gmd:CI_OnlineResource>
<gmd:linkage>
<gmd:URL>
**[http://www.wms.nrw.de/geobasis/wms_nw_dtk100?](http://www.wms.nrw.de/geobasis/wms_nw_dtk100?)**
</gmd:URL>
</gmd:linkage>
</gmd:CI_OnlineResource>
</srv:connectPoint>
</srv:SV_OperationMetadata>
</srv:containsOperations>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_4.3.2._ressourcenverweisConnectPoint.pdf?inline=false


zusätzlich für INSPIRE (^) ☒ (^) ☐ ☐
Die Festlegung über die Art des Geodatendienstes wird mit dem _serviceType_ - Element ([ISO 19119],
Table C.1) umgesetzt. Die von INSPIRE vorgesehene Werteliste ([INS TG MD], 4.2.1.1 (Requirement
4.1)) ist nicht konform zur OGC CSW-Spezifikation [OGC CSW ISO AP]. Letztere verlangt die OGC-
Bezeichnungen der Dienste. Trotzdem muss die INSPIRE-Vorgabe umgesetzt werden. Danach sind
nur die Werte „view“, „download“, „discovery“ und „transformation“ zulässig. Daher wird empfohlen,
die Art des Geodatendienstes im _serviceTypeVersion_ - Element (4.5) weiter zu spezifizieren.

### 4.5 Version des Geodatendienstes bei INSPIRE

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ (^) ☐
zusätzlich für INSPIRE (^) ☒ (^) ☐ ☐
Ergänzend zum _serviceType_ (4.4) ist im Feld _serviceTypeVersion_ ([ISO 19119], Table C.1 No. 2) die
OGC-Bezeichnung in der Form „OGC:<Diensttyp> <Version>“ einzutragen, also z. B. „OGC:WMS
1.1.1“ oder „OGC:WFS 2.0“. Auf die Verwendung äquivalenter ISO-Bezeichner (z. B. OGC:WMS 1.1.1 =
ISO 19128) ist an dieser Stelle aus Gründen der Einheitlichkeit zu verzichten. In Abhängigkeit vom
jeweiligen _serviceType_ ist das _serviceTypeVersion_ - Element wie folgt zu belegen:
**serviceType serviceTypeVersion**
discovery „OGC:CSW <Version>“
view „OGC:WMS <Version>“ oder „OGC:WMTS <Version>“
download „OGC:WFS <Version>“ oder „OGC:WCS <Version>“ oder „predefined ATOM“
Die Angabe der Versionsnummer ist außer bei „predefined ATOM“ verpflichtend. Die
Versionsnummer richtet sich bezüglich ihrer Schreibweise ( 2 - oder 3-stellig) nach der Version der
zugrundeliegenden OGC-Spezifikation für den Dienst.
**XPath:**
D_Metadata/identificationInfo[1]/SV_ServiceIdentification/serviceType/LocalName
**Beispiel:**
<srv:serviceType>
<gco:LocalName codeSpace="http://inspire.ec.europa.eu/metadata-
codelist/SpatialDataServiceType"> **view** </gco:LocalName>
</srv:serviceType>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_4.4_artGeodatendienst.pdf?inline=false
**XPath:**
MD_Metadata/identificationInfo[1]/SV_ServiceIdentification/serviceTypeVersion


### 4.6 Konformität (Übereinstimmung mit Spezifikationen, [INS VO MD], B 7)

```
verpflichtend^ konditional^ optional^
```
GDI-DE (^) ☐ ☐ ☐
zusätzlich für INSPIRE (^) ☒ ☐ ☐
Ergänzend zu den grundsätzlichen Konventionen zur Konformitätsaussage in 2.12 wird an dieser
Stelle das Zitat der anzugebenden Spezifikation geregelt. In Metadaten zu INSPIRE-Netzdiensten ist
gem. [INS TG MD], 4.2.2.1, Recommendation 4.1 die Verordnung 976/2009 (Netzdienste) zu zitieren,
um zu dokumentieren, ob der Dienst die Vorgaben (Funktionen, Performanz, Capabilities etc. ) für
Netzdienste erfüllt.
Dazu sind folgende Angaben erforderlich:
 Titel: **VERORDNUNG (EG) Nr. 976/2009 DER KOMMISSION vom 19. Oktober 2009 zur
Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments und des Rates
hinsichtlich der Netzdienste**
 Veröffentlichungsdatum: **2009 - 10 - 20**
Für die empfohlene Referenzierung mittels gmx:Anchor ([INS TG MD], 4.2.2.1, Recommendation 4.2)
ist für die genannte Durchführungsbestimmung [http://data.europa.eu/eli/reg/2009/976](http://data.europa.eu/eli/reg/2009/976) zu
verwenden (siehe zweites Beispiel).
**Beispiel:**
<srv:serviceType>
<gco:LocalName codeSpace="http://inspire.ec.europa.eu/metadata-
codelist/SpatialDataServiceType"> **view** </gco:LocalName>
</srv:serviceType>
<srv:serviceTypeVersion>
<gco:CharacterString> **OGC:WMS 1.3.0** </gco:CharacterString>
</srv:serviceTypeVersion>
**ATS:**
https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_4.5_versionGeodatendienst.pdf?inline=false
**XPath:**
MD_Metadata/dataQualityInfo/DQ_DataQuality/report/DQ_DomainConsistency/result/DQ_Co
nformanceResult


**Beispiel mit Angabe der Spezifikation in Textform:**

<gmd:DQ_ConformanceResult>
<gmd:specification>
<gmd:CI_Citation>
<gmd:title>
<gco:CharacterString> **VERORDNUNG (EG) Nr. 976/2009 DER KOMMISSION vom 19.
Oktober 2009 zur Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments
und des Rates hinsichtlich der Netzdienste** </gco:CharacterString>
</gdm:title>
<gdm:date>
<gmd:CI_Date>
<gmd:date>
<gco:Date> **2009 - 10 - 20** </gco:Date>
</gmd:date>
<gmd:dateType>
<gmd:CI_DateTypeCode
codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#gmxCodelist
s.xml#CI_DateTypeCode" codeListValue=" **publication** "/>
</gmd:dateType>
</gmd:CI_Date>
</gmd:date>
</gmd:CI_Citation>
</gmd:specification>
<gmd:explanation>
<gco:CharacterString> **Der Dienst wurde mit dem EU-Validator überprüft.**
</gco:CharacterString>
</gmd:explanation>
<gmd:pass>
<gco:Boolean> **true** </gco:Boolean>
</gmd:pass>
</gmd:DQ_ConformanceResult>


**Beispiel mit Angabe der Spezifikation als Verweis:**

<gmd:DQ_ConformanceResult>
<gmd:specification>
<gmd:CI_Citation>
<gmd:title>
<gmx:Anchor xlink:href="http://data.europa.eu/eli/reg/2009/976"> **VERORDNUNG
(EG) Nr. 976/2009 DER KOMMISSION vom 19. Oktober 2009 zur Durchführung der
Richtlinie 2007/2/EG des Europäischen Parlaments und des Rates hinsichtlich der
Netzdienste** </gmx:Anchor>
</gdm:title>
<gdm:date>
<gmd:CI_Date>
<gmd:date>
<gco:Date> **2009 - 10 - 20** </gco:Date>
</gmd:date>
<gmd:dateType>
<gmd:CI_DateTypeCode
codeList="http://standards.iso.org/iso/19139/resources/gmxCodelists.xml#gmxCodelist
s.xml#CI_DateTypeCode" codeListValue=" **publication** "/>
</gmd:dateType>
</gmd:CI_Date>
</gmd:date>
</gmd:CI_Citation>
</gmd:specification>
<gmd:explanation>
<gco:CharacterString> **Der Dienst wurde mit dem EU-Validator überprüft.**
</gco:CharacterString>
</gmd:explanation>
<gmd:pass>
<gco:Boolean> **true** </gco:Boolean>
</gmd:pass>
</gmd:DQ_ConformanceResult>

**ATS:**

https://git.gdi-de.org/ak-
metadaten/konventionen/raw/master/ats/gdide_4.6_konformitaetDienst.pdf?inline=false


## 5 Daten-Dienste-Kopplung

Das Konzept der dienstorientierten Architektur bildet die technische Grundlage, um die Ziele und
Grundlagen der GDI-DE [GDI-DE Architektur - Ziele] umzusetzen. Um die verteilten Ressourcen über
webbasierte Dienste bereitzustellen und nutzbar zu machen, wird das „Publish-Find-Bind-Muster“
verwendet. Dieses wird im Dokument „Architektur der GDI-DE – Technik“ [GDI-DE Architektur -
Technik] ausführlich beschrieben.

Ein wesentlicher Baustein, um das Publish-Find-Bind-Muster erfolgreich umzusetzen, ist die
Kopplung der Metadaten von Geodaten und Geodatendiensten. Ein Geodatensatz kann dabei über
einen oder mehrere Geodatendienste bereitgestellt werden. Voraussetzung hierfür ist, dass sowohl
der Geodatensatz als auch der Geodatendienst mit Metadaten beschrieben und diese Metadaten
öffentlich zugänglich sind. Ein Geodatendienst besitzt, zusätzlich zum Metadatensatz im Katalog, eine
technische Beschreibung seiner Funktionalitäten in Form eines Capabilities-Dokumentes bzw. eines
Service Feeds (Atom).

Die Metadaten eines Geodatensatzes geben i. d. R. keine Auskunft darüber, über welche
Geodatendienste der Geodatensatz bereitgestellt wird. Daher wird die Suche auf die Dienst-
Metadatensätze erweitert und in diesen nach dem Vorkommen des Identifikators des
Geodatensatzes gesucht. Über die _GetCapabilities_ - URL bzw. die URL zum Service Feed (Atom) im
Dienst-Metadatensatz ergibt sich die Referenz auf den Dienst (vgl. Abbildung 3).

**Abbildung 3: Kopplung der Geodaten und Geodatendienste**

Für die Umsetzung der Daten-Dienste-Kopplung ergeben sich also folgende Anforderungen:


```
 Jeder Geodatensatz erhält durch die Beschreibung mit Metadaten einen eindeutigen
Ressourcenidentifikator, <ID>. Dieser ist nach festgelegten Regeln zu bilden und in dem
zugehörigen Metadatensatz zu dokumentieren (Abschnitt 3.1);
 Jeder Metadatensatz , der Datensätze oder Dienste beschreibt, besitzt einen eindeutigen
Metadatensatzidentifikator, <FID> (Abschnitt 2.2);
 Jeder Metadatensatz , der einen Dienst beschreibt, enthält Referenzen auf die Daten, welche
der Dienst bereitstellt (Abschnitt 4.2.1);
 Jeder Metadatensatz , der einen Dienst beschreibt, enthält Angaben über die Art der
Kopplung (Abschnitt 4.2.2);
 Jeder Metadatensatz , der einen Dienst beschreibt, enthält die URL für den GetCapabilities-
Request des Dienstes bzw. den Service Feed des Dienstes (Atom) (Abschnitt 4.3.2);
 Jedes Capabilities-Dokument bzw. jeder Service Feed (Atom) eines Dienstes enthält einen
Link auf den Metadatensatz, der den Dienst beschreibt oder integriert die INSPIRE-
Metadaten direkt im ExtendedCapabilities - Block des Capabilities-Dokumentes ([GDI-DE HE
ViewServices] und [GDI-DE HE DownloadServices]);
 Jedes Capabilities-Dokument eines Darstellungsdienstes enthält für jedes Layerelement
einen Link auf den Metadatensatz, der die Daten beschreibt sowie eine Referenz auf die
Daten (genauer gesagt auf den in den Metadaten festgelegten Ressourcenidentifikator), die
der Dienst visualisiert ([GDI-DE HE ViewServices]);
 Jedes Capabilities-Dokument eines Downloaddienstes enthält in jedem FeatureType -
Element einen Link auf den Metadatensatz, der die Daten beschreibt sowie im
ExtendedCapabilities - Block eine Referenz auf die Daten (genauer gesagt auf den in den
Metadaten festgelegten Ressourcenidentifikator), die der Dienst bereitstellt. Beim Service
Feed (Atom) wird auf den Service Metadatensatz, sowie für jeden eingebundenen „Dataset-
Entry“ auf den Daten-Metadatensatz verwiesen ([GDI-DE HE DownloadServices]).
```
Aus Sicht einer Anwendung (C _lient_ ) ergibt sich daraus z. B. der in Abbildung 4 dargestellte Ablauf.
Die Anwendung sendet z. B. eine Suchanfrage nach **Datensätzen** an einen Suchdienst. Der Suchdienst
sendet die Antwort in Form von ISO 19139 XML-Dokumenten. Diese enthalten einen eindeutigen
**Ressourcenidentifikator** für die bekannten Geodatensätze (<ID>). Um Dienste zu identifizieren, die
diese Ressourcen anbieten, sendet die Anwendung eine erneute Suchanfrage nach **Diensten** an den
Suchdienst. Dabei wird die **<ID> des Datensatzes als Teil der Suchanfrage** übermittelt. Als
Antwort erhält die Anwendung ein oder mehrere ISO 19139 XML-Dokumente, die die Dienste
beschreiben, welche den gesuchten Datensatz anbieten. Über einen _GetCapabilities-_ Request bzw.
_GetDownloadServiceMetadata-_ Request (Atom) erhält die Anwendung Informationen über
angebotene Layer bzw. FeatureTypes der Dienste, wobei jeweils die <ID> des angebotenen
Geodatensatzes im Capabilities-Dokument enthalten ist. Mit diesen Informationen ist die
Anwendung nunmehr in der Lage, Darstellungen bzw. Downloads des Geodatensatzes anzufordern.


**Abbildung 4: Sequenzdiagramm zur Daten-Dienste-Kopplung am Beispiel von OGC:WMS/WFS**


## 6 Open Data-Informationen zu Datensätzen und -serien

„Open Data“ sind Datensätze, die unter entsprechenden Lizenzen veröffentlicht sind, welche den
Umgang mit diesen Daten regeln. Dabei stehen vor allem die Aspekte Entgeltfreiheit,
Weiterverwertbarkeit und manchmal die Namensnennung bei einer Weiterverwendung der Daten
im Vordergrund. Wenn möglich sollen bereits existierende, offene Lizenzen verwendet werden, die
den Open Data-Kriterien^17 der Open Knowledge Definition (OKD) entsprechen. Diese sind in einer
durch GovData gepflegten Sammlung^18 durch den Wert „true“ beim Attribut _is_okd_compliant_
gekennzeichnet.

Metadaten zu Datensätzen und -serien, die für GovData bereitgestellt werden sollen, müssen in
ausgewählten Elementen bestimmte Inhalte aufweisen:

1. In den Schlüsselwörtern wird der Begriff „ **opendata** “ hinterlegt (Details siehe 3.2.2);
2. Die Angaben zur Lizenz werden als Nutzungsbedingung gem. den Konventionen in den
    Abschnitten 2.9.1 bzw. 2.9.2 erfasst und **zusätzlich** strukturiert im Datenformat JSON
    (JavaScript Object Notation) hinterlegt (Details siehe 3.6);

(^17) [http://opendefinition.org/od/1.1/de](http://opendefinition.org/od/1.1/de)
(^18) https://github.com/fraunhoferfokus/ogd-metadata/blob/master/lizenzen/deutschland.json


## 7 Werkzeuge zur Überprüfung der Konventionen

Für die Überprüfung der Gültigkeit der eigenen Metadaten existieren verschiedene Anwendungen.
Innerhalb der GDI-DE wird die Verwendung der GDI-DE Testsuite^19 empfohlen. Dort stehen Tests zur
Prüfung von Metadaten zur Verfügung. Die Tests sind dabei auf Metadaten in deutscher Sprache
ausgerichtet. So kann einerseits überprüft werden, ob die Anforderung an Metadaten durch ISO und
INSPIRE erfüllt werden, andererseits kann auch die Erfüllung der in diesem Dokument vorliegenden
Konventionen geprüft werden.

Für die Überprüfung von Metadaten stehen verschiedene Testklassen zur Verfügung:

```
 „Metadaten | Konventionen der GDI-DE für INSPIRE-relevante Metadaten“
 „Metadaten | Konventionen der GDI-DE für ISO-konforme Metadaten“
```
Bei den Testklassen mit Bezug auf die Konventionen der GDI-DE ist im Namen der dieser immer die
Version desjenigen Dokumentes "Konventionen zu Metadaten" angegeben, dessen Vorgaben geprüft
werden.

Die GDI-DE-Testklassen prüfen neben der Erfüllung der Anforderungen aus ISO und/oder INSPIRE
insbesondere die weitergehenden Anforderungen der GDI-DE-Konventionen. Die
Konformitätsklasse „Metadaten: GDI-DE INSPIRE“ innerhalb der Testklasse „Metadaten |
Konventionen der GDI-DE für INSPIRE-relevante Metadaten“ prüft hingegen nur die Konformität zu
den Anforderungen aus INSPIRE, welche nicht explizit im Konventionendokument genannt bzw.
aufgeführt sind und unverändert gelten.

Mithilfe der GDI-DE Testsuite können neben Metadaten auch Katalog-/Suchdienste (CSW), Karten-
/Darstellungsdienste (WMS) und Downloaddienste (WFS, Atom) überprüft werden.

Neben der GDI-DE Testsuite gibt es noch weitere Anwendungen zur Überprüfung der Gültigkeit der
Metadaten. Eines dieser Werkzeuge ist der EU INSPIRE Validator^20 , der zur Überprüfung der
Übereinstimmung mit den INSPIRE-Vorgaben entwickelt wurde. Ferner können Dienste und
INSPIRE-Datenmodelle mit dem Tool geprüft werden. Das Ergebnis der Überprüfung im INSPIRE-
Validator ist ein Richtwert, um die Konformität der eigenen Metadaten im Hinblick auf INSPIRE
festzustellen. Der Validator wird beständig weiterentwickelt. Im Gegensatz zur GDI-DE Testsuite
können im INSPIRE-Validator die Konventionen dieses Dokumentes nicht überprüft werden. Daher
ist innerhalb der GDI-DE die GDI-DE Testsuite das maßgebliche Tool, um die Konformität von
Metadaten im Hinblick auf die vereinbarten Konventionen zu überprüfen.

Die Ergebnisse der Konformitätsprüfung gegenüber dem Datenmodell und den Anforderungen an
INSPIRE-Netzdienste werden in den Metadaten des entsprechenden Geodatensatzes bzw.
Geodatendienstes dokumentiert (siehe 2.12, bzw. 3.5 und 4.6). Die Einhaltung des INSPIRE-
Datenmodells wird im Daten-Metadatensatz dokumentiert. Die Einhaltung der Vorgaben zu einem
INSPIRE-Netzdienst wird im Dienst-Metadatensatz dokumentiert.

(^19) https://testsuite.gdi-de.org/gdi/
(^20) Der EU INSPIRE Validator ist zugänglich unter URL: [http://inspire-sandbox.jrc.ec.europa.eu/validator/](http://inspire-sandbox.jrc.ec.europa.eu/validator/)


## Referenzen

[ **DESTATIS** ]: Gemeindeverzeichnis
(https://www.destatis.de/DE/ZahlenFakten/LaenderRegionen/Regionales/Gemeindeverzeichnis/
Administrativ/Archiv/GVAuszugQ/AuszugGV4QAktuell.xlsx?__blob=publicationFile)

[ **GDI-DE Architektur - Technik** ]: Architektur der GDI-DE – Technik, Version 3.4.0

[ **GDI-DE Architektur - Maßnahmen** ]: Architektur der GDI-DE – Maßnahmenplan, Version 3. 3 .0

[ **GDI-DE Architektur - Ziele** ]: Architektur der GDI-DE – Ziele und Grundlagen, Version 3. 1. 1

[ **GDI-DE Architektur - Darstellung** ]: Architektur der GDI-DE – Vorgaben zur Bereitstellung von
Darstellungsdiensten, Version 1.0.1

[ **GDI-DE HE ViewServices** ]: Handlungsempfehlungen für die Bereitstellung von INSPIRE
konformen Darstellungsdiensten, Version 1.0

[ **GDI-DE HE DownloadServices** ]: Handlungsempfehlungen für die Bereitstellung von INSPIRE
konformen Downloaddiensten, Version 1.3.0

[ **INS Generic Conceptual Model** ]: INSPIRE Generic Conceptual Model, Version 3.0, 2008- 06 - 20

[ **INS TG Discovery Services** ]: Technical Guidance for the implementation of INSPIRE Discovery
Services, Version 3.1, 2011- 11 - 07

[ **INS TG Download Services** ]: Technical Guidance for the implementation of INSPIRE Download
Services, Version 3.1, 2013- 08 - 09

[ **INS TG MD** ]: Technical Guidance for the implementation of INSPIRE dataset and service metadata
based on ISO/TS 19139:2007, V. 2.0.1, 2017- 03 - 02

**[INS TG View Services]** : Technical Guidance for the implementation of INSPIRE View Services,
Version 3.11, 2013- 04 - 04

[ **INS VO MD** ]: VERORDNUNG (EG) Nr. 1205/2008 DER KOMMISSION vom 3. Dezember 2008 zur
Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments und des Rates hinsichtlich
Metadaten

[ **INS VO Interop** ]: VERORDNUNG (EG) Nr. 1089/2010 DER KOMMISSION vom 23. November 2010
zur Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments und des Rates
hinsichtlich der Interoperabilität von Geodatensätzen und -diensten, geändert durch Verordnung
(EU) Nr. 102/2011 der Kommission vom 4. Februar 2011, Verordnung (EU) Nr. 1253/2013 der
Kommission vom 21. Oktober 2013 und Verordnung (EU) Nr. 1312/2014 der Kommission vom 10.
Dezember 2014

[ **INS VO Netzdienste** ]: VERORDNUNG (EG) Nr. 976/2009 DER KOMMISSION vom 19. Oktober
2009 zur Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments und des Rates
hinsichtlich der Netzdienste, geändert durch Verordnung (EU) Nr. 1088/2010 der Kommission vom

23. November 2010

[ **INS Generic Conceptual Model** ]: Generic Conceptual Model of the INSPIRE data specifications,
2014 - 04 - 08

[ **ISO 19115** ]: ISO 19115:2003, Geographic information - Metadata (with ISO 19115:2003/Cor.
1:2006, Geographic information - Metadata - Technical Corrigendum 1)

[ **ISO 19119** ]: ISO 19119:2005/PDAM 1, Geographic Information – Services


[ **ISO 19139** ]: ISO/TS 19139 (10/2005), Geographic information - Metadata - Implementation
specification

[ **OGC CSW** ]: OpenGIS® Catalogue Services Specification 2.0.2, 2007- 02 - 23

[ **OGC CSW ISO AP** ]: OpenGIS® Catalogue Services Specification 2.0.2 - ISO Metadata Application
Profile, Version 1.0, 2007- 07 - 19

[ **RFC 3986** ]: Uniform Resource Identifier (URI), Generic Syntax
(http://www.ietf.org/rfc/rfc3986.txt)


## Anhang 1: INSPIRE-Spezifikationen (Durchführungsbestimmungen)

(zu Abschnitt 2.12, Konformität (Übereinstimmung mit Spezifikationen, [INS VO MD], B 7 ))

Die folgende Tabelle enthält die relevanten INSPIRE-Durchführungsbestimmungen, die als Inhalt für
die Aussage zur Konformität ( _specification_ - Element) in Frage kommen:

```
Titel der Spezifikation Datum der
Veröffentlichung
```
```
VERORDNUNG (EG) Nr. 1089/2010 DER KOMMISSION vom 23. November 2010
zur Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments und des
Rates hinsichtlich der Interoperabilität von Geodatensätzen und -diensten
```
```
2010 - 12 - 08
```
```
VERORDNUNG (EG) Nr. 976/2009 DER KOMMISSION vom 19. Oktober 2009 zur
Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments und des
Rates hinsichtlich der Netzdienste
```
```
2009 - 10 - 20
```

## Anhang 2: Zuordnung der INSPIRE-Annex-Themen zu ISO-Themenkategorien

(zu Abschnitt 3.3, Themenkategorie nach ISO (Zuordnung zum INSPIRE-Thema: [INS VO MD], B 2.1))

```
INSPIRE-Annex-Thema ISO-Themenkategorie - DE^21 ISO-Themenkategorie - EN^22
Adressen Ortsangaben location
Atmosphärische Bedingungen Klimatologie/Meteorologie/ Atmosphäre climatologyMeteorologyAtmosphere
Bewirtschaftungsgebiete/Schutzgebiete/ geregelte Gebiete und Berichterstattungseinheiten Planungsunterlagen/ Kataster planningCadastre
Biogeografische Regionen Biologie biota
Boden Geowissenschaften geoscientificInformation
Bodenbedeckung Bilddaten/Basiskarten/ Landbedeckung imageryBaseMapsEarthCover
Bodennutzung Planungsunterlagen/Kataster planningCadastre
Energiequellen Wirtschaft economy
Flurstücke/Grundstücke (Katasterparzellen) Planungsunterlagen/Kataster planningCadastre
Gebäude Bauwerke structure
Gebiete mit naturbedingten Risiken Geowissenschaften geoscientificInformation
Geografische Bezeichnungen Ortsangaben location
Geologie Geowissenschaften geoscientificInformation
Gesundheit und Sicherheit Gesundheitswesen health
Gewässernetz Binnengewässer inlandWaters
Höhe Höhenangaben elevation
Landwirtschaftliche Anlagen und Aquakulturanlagen Landwirtschaft farming
Lebensräume und Biotope Biologie biota
```
(^21) Gemäß deutscher Fassung der [INS VO MD]
(^22) Die Begriffe in der Spalte 'ISO-Themenkategorie-EN' entsprechen der Codeliste B5.27 MD_TopicCategoryCode [ISO 19115] sowie der englischen Fassung der [INS VO MD]


```
INSPIRE-Annex-Thema ISO-Themenkategorie - DE 23 ISO-Themenkategorie - EN 24
Meeresregionen Meere oceans
Meteorologisch-geografische Kennwerte Klimatologie/Meteorologie/ Atmosphäre climatologyMeteorologyAtmosphere
Mineralische Bodenschätze Wirtschaft economy
Orthofotografie Bilddaten/Basiskarten/ Landbedeckung imageryBaseMapsEarthCover
Ozeanografisch-geografische Kennwerte Meere oceans
Produktions- und Industrieanlagen Bauwerke structure
Schutzgebiete Umwelt environment
Statistische Einheiten Grenzen boundaries
Umweltüberwachung Bauwerke structure
Verkehrsnetze Verkehrswesen transportation
Versorgungswirtschaft und staatliche Dienste Ver- und Entsorgung/ Nachrichtenwesen utilitiesCommunication
Verteilung der Arten Biologie biota
Verteilung der Bevölkerung — Demografie Gesellschaft society
Verwaltungseinheiten Grenzen boundaries
```
(^23) Gemäß deutscher Fassung der [INS VO MD]
(^24) Die Begriffe in der Spalte 'ISO-Themenkategorie-EN' entsprechen der Codeliste B5.27 MD_TopicCategoryCode [ISO 19115] sowie der englischen Fassung der [INS VO MD]


## Anhang 3: Beschränkungen des öffentlichen Zugangs bei INSPIRE

(zu Abschnitt 2.8, Beschränkungen des öffentlichen Zugangs ([INS VO MD], B 8.2))

Die folgende Tabelle enthält die o.g. Gründe nach Artikel 13(1) a) - h) der INSPIRE-Richtlinie, aus denen eine Beschränkung des öffentlichen Zugangs
überhaupt nur zulässig ist, und listet den jeweils benötigten Eintrag für das _gmx:Anchor_ - Element sowie für den deutschsprachigen Begleittext auf:

```
Grund nach Artikel 13(1) a) - h) der INSPIRE-
Richtlinie:
Zugang beschränkt, weil dieser nachteilige
Auswirkungen hätte auf...
```
```
Eintrag unter gmx:Anchor deutschsprachiger Begleittext
```
```
... a) die Vertraulichkeit der Verfahren von Behörden, sofern
eine derartige Vertraulichkeit gesetzlich vorgesehen ist;
```
```
xlink:href="http://inspire.ec.europ
a.eu/metadata-
codelist/LimitationsOnPublicAccess/
INSPIRE_Directive_Article13_1a"
```
```
Öffentlicher Zugriff beschränkt entsprechend
Artikel 13(1)(a) der INSPIRE-Richtlinie: a)
aufgrund nachteiliger Auswirkungen auf die
Vertraulichkeit der Verfahren von Behörden
```
```
... b) internationale Beziehungen, die öffentliche Sicherheit
oder die Landesverteidigung;
```
```
xlink:href="http://inspire.ec.europ
a.eu/metadata-
codelist/LimitationsOnPublicAccess/
INSPIRE_Directive_Article13_1b"
```
```
Öffentlicher Zugriff beschränkt entsprechend
Artikel 13(1)(b) der INSPIRE-Richtlinie: b)
aufgrund nachteiliger Auswirkungen auf
internationale Beziehungen, die öffentliche
Sicherheit oder die Landesverteidigung
... c) laufende Gerichtsverfahren, die Möglichkeiten einer
Person, ein faires Verfahren zu erhalten oder die
Möglichkeiten einer Behörde, Untersuchungen
strafrechtlicher oder disziplinarischer Art durchzuführen;
```
```
xlink:href="http://inspire.ec.europ
a.eu/metadata-
codelist/LimitationsOnPublicAccess/
INSPIRE_Directive_Article13_1c"
```
```
Öffentlicher Zugriff beschränkt entsprechend
Artikel 13(1)(c) der INSPIRE-Richtlinie: c)
aufgrund nachteiliger Auswirkungen auf
laufende Gerichtsverfahren
```
```
... d) die Vertraulichkeit von Geschäfts- oder
Betriebsinformationen, sofern das innerstaatliche Recht
oder das Gemeinschaftsrecht diese Vertraulichkeit vorsieht,
um berechtigte wirtschaftliche Interessen, einschließlich des
öffentlichen Interesses an der Wahrung der statistischen
Geheimhaltung und des Steuergeheimnisses, zu schützen;
```
```
xlink:href="http://inspire.ec.europ
a.eu/metadata-
codelist/LimitationsOnPublicAccess/
INSPIRE_Directive_Article13_1d"
```
```
Öffentlicher Zugriff beschränkt entsprechend
Artikel 13(1)(d) der INSPIRE-Richtlinie: d)
aufgrund nachteiliger Auswirkungen auf die
Vertraulichkeit von Geschäfts- oder
Betriebsinformationen
```

```
Grund nach Artikel 13(1) a) - h) der INSPIRE-
Richtlinie:
Zugang beschränkt, weil dieser nachteilige
Auswirkungen hätte auf...
```
```
Eintrag unter gmx:Anchor deutschsprachiger Begleittext
```
... e) Rechte des geistigen Eigentums;

```
xlink:href="http://inspire.ec.europ
a.eu/metadata-
codelist/LimitationsOnPublicAccess/
INSPIRE_Directive_Article13_1e"
```
```
Öffentlicher Zugriff beschränkt entsprechend
Artikel 13(1)(e) der INSPIRE-Richtlinie: e)
aufgrund nachteiliger Auswirkungen auf die
Rechte des geistigen Eigentums
```
... f) die Vertraulichkeit personenbezogener Daten und/oder
Akten über eine natürliche Person, sofern diese der
Bekanntgabe dieser Informationen an die Öffentlichkeit
nicht zugestimmt hat und sofern eine derartige
Vertraulichkeit nach einzelstaatlichem oder
gemeinschaftlichem Recht vorgesehen ist;

```
xlink:href="http://inspire.ec.europ
a.eu/metadata-
codelist/LimitationsOnPublicAccess/
INSPIRE_Directive_Article13_1f"
```
```
Öffentlicher Zugriff beschränkt entsprechend
Artikel 13(1)(f) der INSPIRE-Richtlinie: f)
aufgrund nachteiliger Auswirkungen auf die
Vertraulichkeit personenbezogener Daten
```
... g) die Interessen oder den Schutz einer Person, die die
angeforderte Information freiwillig zur Verfügung gestellt
hat, ohne dazu gesetzlich verpflichtet zu sein oder
verpflichtet werden zu können, es sei denn, dass diese
Person der Herausgabe der betreffenden Informationen
zugestimmt hat;

```
xlink:href="http://inspire.ec.europ
a.eu/metadata-
codelist/LimitationsOnPublicAccess/
INSPIRE_Directive_Article13_1g"
```
```
Öffentlicher Zugriff beschränkt entsprechend
Artikel 13(1)(g) der INSPIRE-Richtlinie: g)
aufgrund nachteiliger Auswirkungen auf den
Schutz einer Person
```
... h) den Schutz der Umweltbereiche, auf die sich die
Informationen beziehen, wie z. B. die Aufenthaltsorte
seltener Tierarten.

```
xlink:href="http://inspire.ec.europ
a.eu/metadata-
codelist/LimitationsOnPublicAccess/
INSPIRE_Directive_Article13_1h"
```
```
Öffentlicher Zugriff beschränkt entsprechend
Artikel 13(1)(h) der INSPIRE-Richtlinie: h)
aufgrund nachteiliger Auswirkungen auf den
Schutz von Umweltbereichen
```

## Version 1.2.0 vom 01.08.2017 Anhang 4: Nachweis der Änderungen der Konventionen zu Metadaten Version 2.0.0 gegenüber

## 01.08.2017

```
NEU ÄNDERUNG (Struktur/Inhalt)
```
```
Kapitel Name des Kapitels Beschreibung der Änderung Referenz auf Version 1.2.0
```
```
1.4 Hinweise zum Dokument
```
```
Änderung der Verpflichtung „INSPIRE“ in „zusätzlich für
INSPIRE“ zur Sicherstellung der Beachtung und Einhaltung
der Konventionen unter „GDI-DE“
```
```
2 GrundMetadatensätzliche Konventionen für alle
```
```
Klarstellung zur Verdeutlichung der neuen
Dokumentenstruktur: Konventionen in diesem Kapitel
betreffen Metadaten zu allen Ressourcen in der GDI-DE,
unabhängig von Art der Ressource im hierarchyLevel - Element
2.2 Eindeutiger Metadatensatzidentifikator Löschung der konditionalen Verpflichtung „INSPIRE“, grundsätzlich geltend für GDI-DE zusätzlich für vormals Kapitel 2.4 „Eindeutiger Metadatensatzidentifikator“
```
```
2.5 Kontakt (Verantwortliche Stelle Metadaten)
```
```
neue Verpflichtung: Metadatensatz muss immer eine
Information über die für die Erstellung und Pflege der
Metadaten zuständige Stelle beinhalten; ausgewählte
Elemente erforderlich
```
```
2.6 Kontakt (Verantwortliche Stelle für die Ressource)
```
```
neue Verpflichtung: Metadatensatz muss immer eine
Information über die für die Ressource zuständige Stelle
beinhalten, ausgewählte Elemente erforderlich
```
```
2.7.1 Schlüsselwort „inspireidentifiziert“ Löschung der konditionalen VerpflichtungErgänzung der Verpflichtung „zusätzlich für INSPIRE“^ „GDI-DE“, vormals Kapitel 2.2 „Schlagwort inspireidentifiziert“
```
```
2.8 Beschränkungen des öffentlichen Zugangs ([INS VO MD], B 8.2)
```
```
Beschränkungen des öffentlichen Zugangs nur in den in
Artikel 13(1) a) - h) der INSPIRE-Richtlinie genannten Fällen
zulässig, bei Existenz solcher Zugriffseinschränkungen:
Vorgaben für Inhalte dieser Angabe (u.a. Referenzierung
mittels gmx:Anchor - Element); zusätzliche Regelung für nicht
vorliegende Beschränkung
```
```
vormals Kapitel 3.3 „Beschränkungen
des öffentlichen Zugangs([INS VO MD], B
8.2)“ sowie Kapitel 3.4 „Codelisten und
freie Einträge“
```
```
GELÖSCHT
```

**Kapitel Name des Kapitels Beschreibung der Änderung Referenz auf Version 1.2.0**

```
2.9.1
und
2.9.2
```
```
Nutzungs- und Zugriffsbedingungen in
der GDI-DE (ohne INSPIRE) bzw.
Bedingungen für den Zugang und die
Nutzung bei INSPIRE ([INS VO MD], B 8.1)
```
```
Differenzierung der Konvention zwischen „Nicht-INSPIRE“
und „INSPIRE“, aufgrund unterschiedlicher struktureller und
inhaltlicher Vorgaben (u.a. Referenzierung mittels
gmx:Anchor - Element); keine Doppelung der
Nutzungsbedingungen im useLimitation - Element (bei
INSPIRE) mehr
```
```
vormals Kapitel 3.2 „Bedingungen für
den Zugang und die Nutzung ([INS VO
MD], B 8.1)“ sowie Kapitel 3.4
„Codelisten und freie Einträge“
```
2.10 Regionalschlüssel

```
Ergänzung um alternative Angabe von NUTS/LAU
```
- Regionen vormals Kapitel 2.8 „Regionalschlüssel“^

2 .11

```
Kennzeichnung der Verbindlichkeit von
per Darstellungs- und/oder
Downloaddienst bereitgestellten Daten
```
```
neue, optionale Konvention: Strukturierung von
Informationen bzgl. der Verbindlichkeit von Daten für die
Bereitstellung mittels Diensten
```
2.12 KonfSpezifikationen)ormität (Übereinstimmung mit Ergänzung zur Führung des Angaben zu Konformität sowie Änderung des Titels _explanation-_ Elementes bei vormals Kapitel 2.7 „Übereinstimmung mit Spezifikationen ([INS VO MD], B 7)“

3 Konventionen für Metadaten zDatenbeständen und Anwendungenu

```
Klarstellung zur Verdeutlichung der neuen
Dokumentenstruktur: Konventionen in diesem Kapitel
betreffen Metadaten zu allen Ressourcen in der GDI-DE, außer
Dienste, d.h. Inhalt im hierarchyLevel - Element ungleich
„service“
```
3.1 Eindeutiger Ressourcenidentifikator ([INS VO MD], B 1.5)

```
Löschung der Kennzeichnung „zusätzlich für INSPIRE“,
grundsätzlich geltend für GDI-DE; keine Unterstützung der
alternativen (i. S. v. GDI-DE-auslaufend) Kodierung mit „#“ als
Trennzeichen mehr
```
```
vormals Kapitel 4.1 „Eindeutiger
Ressourcenidentifikatorin Daten-
Metadaten ([INS VO MD], B.1.5)“
```
3.2.1 Quellenangabe für Schlüsselwörter zu INSPIRE-Themen

Präzisierung der INSPIRE-Anforderungen für Quellenangabe;
verpflichtende Elemente und Inhalte für die Angabe des
Thesaurus
3.2.2 Schlüsselwort „opendata“ separates Element aufgrund von neuer Dokumentenstruktur vormals Kapitel 3.5 „OpenData“

3.3 Themenkategorie nach ISO (Zuordnung zum INSPIRE-Thema: [INS VO MD], B 2.1) Umbenennung der Konvention; keine inhaltliche Änderung

```
vormals Kapitel 2.3 „Zuordnung
INSPIRE-Thema / ISO-
Themenkategorie(INS VO MD, B2.1)“
```

**Kapitel Name des Kapitels Beschreibung der Änderung Referenz auf Version 1.2.0**

3.4

```
Ressourcenverweis für Datensätze und -
serien (transferOptions, [INS VO MD], B
1.4)
```
```
Ergänzung eines Hinweises bzgl. Angabe im function - Element
```
```
vormals Kapitel 2.5.1
„Ressourcenverweis (transferOptions)
([INS VO MD], B 1.4)“
```
3.5 Konformität (Übereinstimmung mit Spezifikationen, [INS VO MD], B 7)

```
Ergänzung für empfohlene Referenzierung der anzugebenden
Durchführungsbestimmung mittels gmx:Anchor - Element;
Löschung der Angaben zu Technical Guidance-Dokumenten
```
```
vormals Kapitel 2.7 „Übereinstimmung
mit Spezifikationen ([INS VO MD], B 7)“
```
3.6 Nutzungsbedingungen und Lizenzinformationen für Open Data

```
separates Element aufgrund der neuen Dokumentenstruktur,
keine Doppelung der Nutzungsbedingungen im useLimitation -
Element (bei INSPIRE) mehr
```
```
vormals Kapitel 3.5 „OpenData“
```
3.7 Formatangaben

```
Klarstellung aufgrund eines missverständlichen Beispiels in
der [TG MD], mit Hinweis auf eine zu bevorzugende
Strukturierung gem. Kommentar unter Anhang C.3.3 der [INS
TG MD]
```
4 Konventionen für Metadaten zu Diensten

```
Klarstellung zur Verdeutlichung der neuen
Dokumentenstruktur: Konventionen in diesem Kapitel
betreffen Metadaten zu allen Diensten in der GDI-DE, d.h.
Inhalt im hierarchyLevel - Element gleich „service“
```
4.1.1 Schlüsselwörter zu Dienstkategorien bei INSPIRE

```
Formulierung einer Empfehlung (Werteauswahl) für Dienste;
in Metadaten für INSPIRE ist die Angabe mindestens eines
Schlüsselworts erforderlich
```
4.2.1 Gekoppelte DatenMD], B 1.6) - Ressource ([INS VO Löschung der konditionalen Verpflichtung bei „INSPIRE“, grundsätzlich geltend für GDI-DE zusätzlich für

```
vormals Kapitel 4.2 „Referenz auf
Geodatensätze in Dienst-Metadaten([INS
VO MD], B.1.6)“
```
4.2.2 Art der Kopplung zwischen Dienst und zugehörigen Daten

```
Löschung der Verpflichtung bei „zusätzlich für INSPIRE“,
keine Vorgaben mehr; grundsätzlich konditional geltend für
GDI-DE
```
```
vormals Kapitel 4.3 „Art der Kopplung
zwischen Dienst und zugehörigen Daten“
```
4.3.1 Ressourcenverweis unter transferOptions ([INS VO MD], B 1.4) Ergänzung eines Hinweises bzgl. Angabe im _function-_ Element

```
vormals Kapitel 2.5.1
„Ressourcenverweis (transferOptions)
([INS VO MD], B 1.4)“
```
4.3.2 Ressourcenverweis unter connectPoint Löschung der Verpflichtung bei „INSPIRE“, grundsätzlich geltend für GDI-DE vormals Kapitel 2.5.2
„Ressourcenverweis (connectPoint)“


**Kapitel Name des Kapitels Beschreibung der Änderung Referenz auf Version 1.2.0**
bzw. Kapitel 4.4 „Verweis im Dienst-
Metadatensatz auf Dienst“

4.4 A([INS VO MD], B 2.2)rt des Geodatendienstes bei INSPIRE Verschiebung der Konvention; keine inhaltliche Änderung

```
vormals Kapitel 2.6.1 „Art des
Geodatendienstes bei INSPIRE-Diensten
(INS VO MD], B 2.2)“
```
4.5 Version des Geodatendienstes bei INSPIRE

```
Änderung der konditionalen Verpflichtung „GDI-DE“ in
„zusätzlich für INSPIRE“ sowie Ergänzung einer Vorgabe
(Muster) zur Strukturierung dieser Information.
```
```
Vormals Kapitel 2.6.2 „Version des
Geodatendienstes“
```
4.6 Konformität (Übereinstimmung mit Spezifikationen, [INS VO MD], B 7)

```
Ergänzung für empfohlene Referenzierung der anzugebenden
Durchführungsbestimmung mittels gmx:Anchor - Element;
Löschung der Angaben zu Technical Guidance-Dokumenten
```
```
vormals Kapitel 2.7 „Übereinstimmung
mit Spezifikationen ([INS VO MD], B 7)“
```
5 Daten-Dienste-Kopplung

```
Reduzierung auf die Darstellung der Grundsätze und
Zusammenhänge; zugehörige Vorgaben für einzelne
Metadatenelemente in separaten Abschnitten
```
```
vormals Kapitel 4 „Daten-Dienste-
Kopplung“
```
6 Open Dataund -serien-Informationen zu Datensät zen

```
Reduzierung auf die Darstellung der Grundsätze und
Zusammenhänge; zugehörige Vorgaben für einzelne
Metadatenelemente in separaten Abschnitten
```
```
vormals Kapitel 3.5 „OpenData“
```
7 Werkzeuge zur Überprüfung der Konventionen Inhaltliche Anpassunverwendeten Testklassen in der GDIgen, u.a. konkrete Nennung der -DE Testsuite. vormals Kapitel 5 „Werkzeuge zur Überprüfung der Konventionen“

Anhang 3 Beschränkungen des öffentlichen Zugangs bei INSPIRE

Anhang mit tabellarischer Auflistung des jeweils benötigten
Eintrages für _gmx:Anchor_ - Element sowie bei Angaben ein
deutschsprachiger Begleittext
Löschung „Glossar“ Kapitel 6
Löschung INSPIRE Datenspezifikationen Anhang 1, 2. Teil
Löschung INSPIRE Technical Guidance zu Diensten Anhang 1, 3. Teil


