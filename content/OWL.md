# WEB ONTOLOGY LANGUAGE (OWL)

## Ontologien
Ein Datenmodell, dass Wissen in Form von Konzepten darstellt und die Beziehungen dieser Konzepte.
![Screenshot (68)](https://user-images.githubusercontent.com/92676445/198880512-e3d4ba4b-77d1-4ede-bb96-79432297f14d.png)

**OWL ist die Abkürzung für "Web Ontology Language" und dient ähnlich dem RDF der maschinenlesbaren Darstellung von Inhalten, ist aber gegenüber XML, RDF, RDF-S oder ähnlichen Sprachen ein größeres Vokabular und eine formale Semantik.**

- Standartsprache um im Semnatic Web Informationen zu repräsentieren
- zur Beschreibung von Ontologien (Klassen und Eigenschaften (Properties), sowie die Beziehungen zwischen diesen werden beschreiben)


## Die OWL-Sprache bietet 3 Untersprachen, um unterschiedliche Nutzergruppen gerecht zu werden

**OWL FULL**
- umfasst alle OWL Sprachkonstrukte
- Obermenge von RDF
- RDF Aussagen können mit OWL FULL Konstrukten beliebig gemischt werden
- bietet weitreichende Ausdrucksfähigkeit
- keine Garantie, dass Ergebnisse berechenbar sind 

**OWL DL**

- DL steht für Description Language
- Subsprache von OWL FULL
- Kompromiss zwischen Ausdruckskraft und Entscheidbarkeit

**OWL LITE**
- Subsprache von OWL DL
- zur Erstellung einfacher Klassenhirachie und Einschränkungen
- Auswertung der Ausdrücke leichter

![The-three-OWL-sublanguages](https://user-images.githubusercontent.com/92676445/198892509-a4b0dbde-0915-4e64-8f7a-0733ef3bf135.png)

## Aufbau OWL Dokument
![+Aufbau+OWL-Ontologie-Dokument](https://user-images.githubusercontent.com/92676445/198982071-ee7fa352-bb6d-4980-8f15-738eb046404a.jpg)

- Aussagen mit Klassen und Eigenschaften
- Klassen: Menge von Individuen, die bestimmte Eigenschaften teilen
- Eigenschaften: Beziehung zwischen Idividuen und Individuen oder Klassen
- Es gibt keine festgelegte Reihenfolge der Aussagen

**Klassen**

...werden definiert durch Namensgebung und Spezifizierung

<em>owl:class</em>  (Subklasse von rdf:class)             -------->         <em><owl:class rdf:ID=,,dishes´´/></em>

Es gibt zwei vordefinierte Klassen
- <em>owl:Thing</em> <strong>Oberklasse aller Klassen</strong>
- <em>owl:Nothing</em> <strong>Unterklasse aller Klassen</strong>
