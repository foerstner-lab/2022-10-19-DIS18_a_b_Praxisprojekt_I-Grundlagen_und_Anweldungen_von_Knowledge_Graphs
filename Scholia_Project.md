# SCHOLIA DISEASES VISUALIZATION

Wir visualisieren die verschiedenen Krankheiten, welche auf https://scholia.toolforge.org/  vorhanden sind. Wir möchten dabei auf die veröffentlichten Paper und zusammenhängenden Krankheiten eingehen. Wir nutzen dafür Python und verschiedene Python Libraries. Wir konzentrieren uns dabei auf die Circos Plots, um die Verbindungen der Krankheiten und deren Paper zu visualisieren. 

Das ideale Ergebnis ist eine vollständige Visualisierung aller Krankheiten, die auf Scholia zu finden sind. Die Visualisierung soll dabei sehr aufschlussreich sein und sehr viele Informationen beinhalten, ohne die Übersichtlichkeit zu verringern. Im Idealfall ist die Visualisierung so gut, dass sie bei Scholia integriert werden kann.

### Beispiel: 
![Example](https://github.com/kaiserog/2022-10-19-DIS18_a_b_Praxisprojekt_I-Grundlagen_und_Anweldungen_von_Knowledge_Graphs/blob/main/content/images/circos-naming-names-nyt.png)
(Quelle: http://circos.ca/intro/general_data/)
Z.b. Politiker durch Krankheiten ersetzen, Verbindungen sind die “related diseases”, Blöcke sind die Anzahl an Paper, die Dicke der Blöcke ist wie oft die Paper zitiert wurden.

Das minimale Projektziel ist die Visualisierung einzelner Krankheiten. Die Informationsdichte schränkt dabei die Übersichtlichkeit ein. Daher kann sie auch nicht bei Scholia integriert werden. 

Die grobe Zeitplanung liegt bei 12 Stunden in periodischem Wechsel von biwöchentlichen Zyklen.
![Timetable](https://github.com/kaiserog/2022-10-19-DIS18_a_b_Praxisprojekt_I-Grundlagen_und_Anweldungen_von_Knowledge_Graphs/blob/main/content/images/image2.png)

## Research:
- Welche Visualisierungstools nutzen wir?
- Welche Libraries?
- Wie kommen wir an die Daten von Scholia?
- Wie erhalten wir die vollständigen Daten?
- Müssen wir noch andere Quellen hinzufügen?

## Implementation:
- Pycircos
- Matplot
- Plotly
- Feedback:
- Interne Feedbackrunden
- Q&As
- Ideen und Anregungen
- Verbesserungsvorschläge 

## Geplante Arbeitsweise:
- Wir nehmen an, dass die Daten von Scholia inhaltlich korrekt sind.
- Python
3-Phasen-Modell: Research, Implementation, Feedback
- Iteratives Arbeiten

## Ressourcen:
- Github
- Scholia
- Python
- Wikidata
 
## grobe Gliederung des GitHub-Repositorium:
- Lizenz
- MIT
- GPL
- Creative Commons
- BSD
- -> für Code: MIT, GPL, BSD
- -> für Texte, Bilder, Sound: Creative Commons (CC)
- -> Empfehlung: CC by oder CC0
- -> für die Lizenzsierung fügen Sie einfach eine Lizenzdatei mit dem entsprechenden Text unter Hinzufügung Ihrer Namen dem Repo hinzu
- ggf. requirements.txt/setup.py -Datei: beinhaltet das Setup der benötigten anderen Tools und deren Versionen, die für den Code gebraucht werden; Packaging über pip - oder conda
- ggf. Dockerfile: behinhaltet Dockercontainer mit benötigten Software-Versionen
- ggf. Projektmanagement über Asana oder GitHub-Tickets
- ggf. automatisches Testing, zum Beispiel mit GitHub Actions
- Standardisierter Code-Style
- Python-Style Guide: PEP8
- automatischer Code-Formatter: Black
- Zen of Python
- ggf. run-Skripte

