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

## Klassen

...werden definiert durch Namensgebung und Spezifizierung

<em>owl:class</em>  (Subklasse von rdf:class)             -------->         <em><owl:class rdf:ID=,,dishes´´/></em>

Es gibt zwei vordefinierte Klassen
- <em>owl:Thing</em> <strong>Oberklasse aller Klassen</strong>
- <em>owl:Nothing</em> <strong>Unterklasse aller Klassen</strong>


## OWL kann Klassen logisch kombinieren

<em>Aufzählung</em> (oneOf)
- Klasse wird beschrieben indem ihre Mitglieder aufgezählt werden


<owl:Class rdf:ID="menu"></br>
    <**owl:oneOf** rdf:parseType="Collection"></br>
     <owl:Thing rdf:about="#TacoConPollo"/></br>
     <owl:Thing rdf:about="#TacoConPorcino"/></br>
     <owl:Thing rdf:about="#TacoVerde"/></br>
     <owl:Thing rdf:about="#BurritoConPollo"/></br>
     <owl:Thing rdf:about="#BurritoVerde"/></br>
    <**/owl:oneOf**></br>
</owl:Class>



<em>Vereinigung</em> logisches ODER (unionOf)
- definiert Klasse, die alle Mitglieder aller spezifizierten Klassen enthält


<owl:Class rdf:ID=“MeatDishes"></br>
<**owl:unionOf** rdf:parseType="Collection"></br>
<owl:Class rdf:about="#DishesWithChicken"/></br>
<owl:Class rdf:about="#DishesWithPork"/></br>
<**/owl:unionOf**></br>
</owl:Class>


<em>Durchschnitt</em> logisches UND (intersectionOf)
- definiert Klasse, die alle Mitglieder enthält die zu den spezifizierten Klassen gleichzeitig gehören

<owl:Class rdf:ID=“MeatDishes"></br>
<**owl:intersectionOf** rdf:parseType="Collection"></br>
<owl:Class rdf:about="#Dishes"/></br>
<owl:Restriction></br>
<owl:onProperty rdf:resource="#isMadeOf"/></br>
<owl:hasValue rdf:resource="#Meat"/></br>
</owl:Restriction></br>
<**/owl:intersectionOf**></br>
</owl:Class></br>


<em>Komplement</em> logisches NICHT (complementOf)
- definiert Klasse, indem alle Individuen, die nicht zu der Klasse gehören benannt werden


<owl:Class rdf:ID=“NotADish">
<**owl:complementOf** rdf:resource="#Dish"/>
</owl:Class>

<em>Subklasse</em> (subClassOf)
- Spezialisierung einer anderen Klasse

<owl:Class rdf:ID=“Dish"></br>
<**rdfs:subClassOf** rdf:resource="#DeliciousDish"/></br>
</owl:Class>

<em>Äquivalenzklasse</em> (equivalentClass)
- die KLasse enthält die gleichen Individuen

<owl:Class rdf:about="#Dish"></br>
<**owl:equivalentClass** rdf:resource="#Meal"/></br>
</owl:Class>

<em>Disjunkte Klassen</em> (disjointWith)
- Individuen sind entweder in der einen oder in der anderen Klasse

<owl:Class rdf:about="#Meatdish"></br>
<**owl:disjointWith** rdf:resource="#VegeterianDish"/></br>
</owl:Class>

## Eigenschaften

- Eigenschaften (Properties) erlauben es Aussagen über Klassen und ihre Mitglieder und über Individuen zu machen
- In OWL können Eigenschaften ebenfalls Eigenschaften haben (Eigenschaftcharasteristiken - "property charasteretics")
- Man unterscheidet Objekteigenschaften und Datentypeigenschaften
Objekteigenschaft: ordnen Objekten Objekte zu

<**owl:ObjectProperty** rdf:ID=„isMadeOf"/>

Datentypeigenschaft: ordnen Objekten Objekte zu

<**owl:DatatypeProperty** rdf:ID=„RestaurantClosingTime"/>

## Charakteristiken von Eigenschaften

- owl:equivalentProperty
- owl:inverseOf

BEISPIEL: 
</br>
<owl:ObjectProperty rdf:ID=„menuPrice"></br>
<**owl:equivalentProperty** rdf:resource="#menuCost"/></br>
</owl:ObjectProperty></br>

- Transitivität</br>
<em><owl:TransitiveProperty></em>
- Symmetrie</br>
<owl:SymmetricProperty>
- Rechtseindeutigkeit</br>
<owl:FunctionalProperty>
- Linkseindeutigkeit/Injektivität</br>
<owl:InverseFunctionalProperty>


## Fakten
- Neben den Klassen und Eigenschaftsaxiomen gibt es noch individuelle Axiome

<strong>3 Arten</strong>
- Klassenzugehörigkeit

bsp:</br>
<**Dish** rdf:ID=„TacoConPollo"></br>
<consistsOf rdf:resource="#Taco"/></br>
<prize rdf:resource="#1,50€"/></br>
…</br>
…</br>
<**/Dish**></br>

- Eigenschaftswerte
- Identitätsaussagen

BEISPIEL: </br>
<Dish rdf:ID=„Meatdish"></br>                       
<owl:differentFrom rdf:resource="#TacoConPollo“/></br>
<owl:differentFrom rdf:resource="#TacoConPorcino"/></br>
</Dish>



  
  
  
