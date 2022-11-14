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

<p align="center">
<img src="https://user-images.githubusercontent.com/92687630/201656067-372f7e32-67d9-49b7-8926-c665003febca.png" alt="Aufbau" width="800"/>
</p>

## Abfragesprache
- Cypher als deklarative Abfragesprache
- Syntax bestehend aus „ASCII-Art“
- Daten und Beziehung werden in Form von Knoten und Kanten gespeichert
- Jeder Knoten hat eine beliebige Anzahl von Attributen 
- Knoten und Kanten können eine Bezeichnung haben
- Labels können verwendet werden, um die Treffermenge bei der Suche einzuschränken
- Knoten können beliebig viele Labels und Properties haben, Kanten nur ein Label und beliebig viele Properties

<p align="center">
<img src="https://user-images.githubusercontent.com/92687630/200586921-2a0b16d4-f871-4866-a684-09c7a249c70f.png" alt="CQL" width="800"/>
</p>
  
<br></br>

## Neo4j vs RBDM
| Neo4j         | RDBM (MySQL, PostgreSQL) |
|---------------|--------------------------|
| Graph-Speicherstruktur | feste, vordefinierte Tabellen  |
| flexibles Datenmodell | logisches Modell  |
| Leistung, unabhängig von der Anzahl und Tiefe der Verbindungen | Verarbeitungsgeschwindigkeit nimmt mit zunehmenden Dateneingaben ab|
| Cypher-Sprache |SQL-Sprache  |
<br></br>

## Beispiel
<img src="https://user-images.githubusercontent.com/92687630/200589729-cedd9864-8501-4444-a5f0-126897012a01.png" alt="" width="300"/>
<br></br>


|Neo4j|RBDM|
|:-----------:|:----------:|
|<img src="https://user-images.githubusercontent.com/92687630/200590756-1b030130-6c6f-45fc-a462-46a6bb2e9b32.png" alt="" width="300"/>|<img src="https://user-images.githubusercontent.com/92687630/200591004-79ff55cc-71c2-4b2c-857c-d65537afcb34.png" alt="" width="300"/>|






## Vor- und Nachteile
|Vorteile|Nachteile|
|--------|---------|
|keine Join-Probleme existieren|nicht für große binäre Datenobjekte gebaut|
|gute Datenintegrierung von neuen Strukturen||
|Echtzeitausführung||
|komplizierte Datenaufrufe in Graph-Traversals ersetzt||
|whiteboard-friendly||
-------------------------------
<br></br>
## Quiz
**Neo4j ist eine...**
<ol>
  <li>Relationale Datenbanken</li>
  <li>Graphdatenbank</li>
  <li>Objektorientierte Datenbank</li>
  <li>Hierarchische Datenbank</li>
  <li>Abfragesprache</li>
</ol>
<br></br>

**Inwiefern ist Neo4j eine noSQL-Datenbank?**
<ol>
  <li>Es wird ein relationaler Ansatz verfolgt</li>
  <li>Daten können ohne vorausdefiniertes Schema gespeichert werden</li>
  <li>Es wird kein SQL genutzt um auf Daten zuzugreifen</li>
  <li>Sie ermöglicht die Speicherung und den Zugriff auf miteinander verbundene Datenpunkte</li>
  <li>Daten müssen in eine  normalisierte Form gebracht werden um komplexe Datenobjekte zu zerlegen</li>
</ol>
<br></br>

**Welches davon ist kein CQL-Befehl?**
<ol>
  <li>Match</li>
  <li>Create</li>
  <li>Delete</li>
  <li>Exit</li>
  <li>Set</li>
</ol>
