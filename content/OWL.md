# WEB ONTOLOGY LANGUAGE (OWL)

## Ontologien
Ein Datenmodell, dass Wissen in Form von Konzepten darstellt und die Beziehungen dieser Konzepte.
![Screenshot (68)](https://user-images.githubusercontent.com/92676445/198880512-e3d4ba4b-77d1-4ede-bb96-79432297f14d.png)

OWL soll verwendet werden, wenn die in Dokumenten enthaltenen Informationen von Anwendungen verarbeitet werden müssen, im Gegensatz zu Situationen, in denen der Inhalt nur Menschen präsentiert werden muss. OWL kann verwendet werden, um die Bedeutung von Begriffen in Vokabularen und die Beziehungen zwischen diesen Begriffen explizit darzustellen. Diese Darstellung von Begriffen und deren Zusammenhängen wird als Ontologie bezeichnet. OWL hat mehr Möglichkeiten zum Ausdrücken von Bedeutung und Semantik als XML, RDF und RDF-S, und daher geht OWL in seiner Fähigkeit, maschineninterpretierbare Inhalte im Web darzustellen, über diese Sprachen hinaus. OWL ist eine Überarbeitung der Webontologiesprache DAML+OILEinbeziehen von Lehren aus dem Design und der Anwendung von DAML+OIL.

## DIe OWL-Sprache bietet 3 Untersprachen, um unterschiedliche Nutzergruppen gerecht zu werden

**OWL FULL**
- umfasst alle OWL Sprachkonstrukte
- Obermenge von RDF
- RDF Aussagen können mit OWL FULL Konstrukten beliebig gemischt werden

**OWL DL**
- DL steht 
- Subsprache von OWL FULL
- Kompromiss zwischen Ausdruckskraft und Entscheidbarkeit

**OWL LITE**
- Subsprache von OWL DL
- zur Erstellung einer einfachen Klassenhirachie
- Auswertung der Ausdrücke leichter
