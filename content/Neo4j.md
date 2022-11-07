# Neo4j
<br></br>
## Was sind Graphdatenbanken (Graph databases)?
- Sammlung aus Kanten und Knoten, welche in Beziehung zueinander stehen
- NoSQL-Datenbanken
- komplizierte Datenaufrufe bestehend aus mehreren JOINS werden mit einfacheren Graph-Traversals ersetzt
- Graph-Speicherstruktur
- flexibles Datenmodell
- Leistung, unabhängig von der Anzahl und Tiefe der Verbindungen
<br></br>

## Was ist Neo4j?
- weltweit führende, in Java implementiere Open-Source-Graphdatenbank
- wird von Tausenden von Startups, Bildungseinrichtungen und großen Unternehmen genutzt, wie bsp. Microsoft oder Ebay
- umfangreiche, produktionsreife Algorithmenbibliothek und fortschrittliche, bahnbrechende Workflows für maschinelles Lernen
- "eine eingebettete, plattenbasierte, transaktionale Datenbank-Engine, die Daten in Graphen statt in Tabellen speichert."
<br></br>

## Eigenschaften von Neo4j
- Native Graphdatenbank
- Optimiert auf das Speichern und Abrufen von Graphdaten
- NoSQL
- Schema-optional
- Daten werden als Schlüssel-Wert-Paare gespeichert
- Neo4j-Datenbanken skalieren horizontal
- Schema und Struktur sind Flexibel
- Beziehungen zwischen Daten sind verwaltbar
<br></br>

## Aufbau
- Labeled-Property-Graph-Modell
- Bestehend aus vier Komponenten
<ol>- Nodes (Knoten): Hauptdatenelemente, die durch Beziehungen verbunden sind</ol>
<ol>- Relationships (Kanten): Beschreibt die Verbindungen zwischen den Knoten und verbindet sie miteinander</ol>
<ol>- Properties (Attribute): Attribute von Knoten und Beziehungen</ol>
<ol>- Labels: Gruppieren Knoten und beschleunigen sie</ol>
<br></br>

## Abfragesprache
- Cypher als deklarative Abfragesprache
- Syntax bestehend aus „ASCII-Art“
- Daten und Beziehung werden in Form von Knoten und Kanten gespeichert
- Jeder Knoten hat eine beliebige Anzahl von Attributen 
- Knoten und Kanten können eine Bezeichnung haben
- Labels können verwendet werden, um die Treffermenge bei der Suche einzuschränken
- Knoten können beliebig viele Labels und Properties haben, Kanten nur ein Label und beliebig viele Properties
<br></br>

## Neo4j vs RBDM
| Neo4j         | RDBM (MySQL, PostgreSQL) |
|---------------|--------------------------|
| Graph-Speicherstruktur | feste, vordefinierte Tabellen  |
| flexibles Datenmodell | logisches Modell  |
| Leistung, unabhängig von der Anzahl und Tiefe der Verbindungen | Verarbeitungsgeschwindigkeit nimmt mit zunehmenden Dateneingaben ab|
| Cypher-Sprache |SQL-Sprache  |
<br></br>

## Vor- und Nachteile
|Vorteile|Nachteile|
|--------|---------|
|keine Join-Probleme existieren|nicht für große binäre Datenobjekte gebaut|
|gute Datenintegrierung von neuen Strukturen||
|Echtzeitausführung||
|komplizierte Datenaufrufe in Graph-Traversals ersetzt||
|whiteboard-friendly||

