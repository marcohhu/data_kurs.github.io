--- 
title: "Datenanalyse mit R"
author: "Marco"
date: "2020-03-20"
site: bookdown::bookdown_site
documentclass: book
bibliography: [book.bib]
biblio-style: apalike
link-citations: yes
github-repo: marcohhu/data_kurs.github.io
url: 'http\://marcohhu/data_kurs.github.io/'
description: "tbc..."
---

# Preface {-}

[Work in Progress]

<!--chapter:end:index.Rmd-->

# Einleitung {-}

tbc...

## Konventionen {-}

Das Buch ist als Ergänzung zur Data-Übung gedacht...

* Packages werden als `package()` gezeigt

## Aufgaben {-}

Aufgaben für die Studierenden können in unterschiedliche Formen in das Dokument eingebettet werden. 

1. Quiz
Mit dem `Webex-Package` können Quiz-Fragen zum Selbststudium bereitgestellt werden. Das Dokument kann allerdings nicht heruntergeladen oder Antworten gespeichert werden. Beispiele für verschiedene Möglichkeiten findest du [hier](https://marcohhu.github.io/data_kurs.github.io/notebooks/sandbox_quiz.html) 

2. Jupyter-Notebooks
Jupyter-Notebooks sind eine IDE-Alternative zu RStudio. Aus meiner Perspektive ist die Installation und Handhabe etwas komplizierter. Allerdings bieten Notebooks eine gute Möglichkeit um Aufgabenblätter zu formulieren, da Notebooks heruntergeladen und bearbeitet werden können (aber auch nur in Jupyter-Notebooks und nicht in RStudio). Auch dazu gibt es ein Beispiel aus einem anderen Tutorium siehe [hier](https://marcohhu.github.io/data_kurs.github.io/notebooks/vis.html)

3. R-Notebooks
Auch RStudio bietet ein Notebook Format an. Großer Vorteil: Das Notebook kann direkt von der Seite heruntergeladen und in Rstudio geöffnet sowie bearbeitet werden. Ein Beispiel findest du [hier](https://marcohhu.github.io/data_kurs.github.io/notebooks/sandbox.nb.html)

<!--chapter:end:intro.Rmd-->

# Getting started {#start}
tbc..





## Kurzinfos zur Entwicklung

A brief history of Time tbc...

## Warum R?

Traditionell wird in den Sozialwissenschaften mit SPSS oder Stata als Statistik- und Analyse-Software gearbeitet. Warum hat sich dann R als defacto Programmiersprache zur Datenanalyse entwickelt? Einige Argumente sprechen für R:

* R ist freie Software und Open Source. 
* R läuft sowohl auf Windows als auch auf Mac Os und Linux.
* R hat eine große und sehr aktive Community. Die Community stellt vielfältige Lern-Ressourcen zur Verfügung und hilft bei Problemen. Wir werden noch kennenlernen, wie wir von der Community profitieren können.
* R wird aktiv weiterentwickelt. Besonders wichtig sind dabei sogenannte Packages, die nicht nur die Arbeit erleichtern, sondern auch die Anwendung neuer Methoden ermöglichen.

Aber R muss auch erlernt werden. Und Software verunsichert uns häufig, wenn sie nicht auf einem Drag-and-Drop Prinzip basiert, sondern durch Programmiercode ausgeführt wird.

## Installation

Bevor wir starten, müssen wir R zunächst installieren. Auf der Website des Cran-Projekts („The Comprehensive R Archive Network“) können wir R downloaden und installieren. Wir beachten einfach die Hinweise (_„install R for the first time“_) auf der Homepage via [Cran](https://cran.r-project.org/). Wenn wir R auf unserem Computer installiert haben, dann können wir mit einem Doppelklick das Programm öffnen und in der R Console starten. 

## Die Console

Die R Console erinnert etwas an Windows 98. Deshalb installieren wir auch später Rstudio, dass uns die Arbeit erleichtert und eher unserem Selbstbild als erfolgreiche Analysten entspricht. Aber erstmal gucken wir uns die Console an.

\includegraphics[width=21.25in]{img/s_r-console} 
In der Console können wir direkt mit unserem Code beginnen. Um einen ersten Eindruck von R zu bekommen, halten wir uns an die alte Tradition ein Programm mit dem Ergebnis  zu schreiben. Dafür nutzen wir die `print()` Funktion, geben in die Console `print(„Hello World!“)` ein und bestätigen mit Enter. 

```r
print("Hello World!")
## [1] "Hello World!"
```

Super, damit haben wir unseren ersten R Code geschrieben. 
Die Console können wir aber auch als Taschenrechner nutzen: So können wir 15 Prozent Trinkgeld von unserem 35,70 Euro Bierdeckel in einer Kneipe berechnen, indem wir einfach 0.15 * 35.70 in die Console eingeben und mit Enter bestätigen. 

```r
0.15 * 35.70
## [1] 5.355
```
Das Ergebnis lautet 5,35 Euro. Falls ein Fehler auftritt, könnte dies an einem Komma `,` anstatt einem Punkt `.` zur Trennung liegen.


## RStudio

## Pakete

<!--chapter:end:getting-started.Rmd-->

# Styleguide {#style}

## Gute Praxis

wie schreibe ich "guten" Code

## R Projekte

Ziel: Ein R Projekt und entsprechende Unterordner anlegen, um nicht die Übersicht zu verlieren. Kurzer Abschnitt, wie Pfade definiert und gesetzt werden.
Organisation eines Projekts

* R Projekt
  + set-up.R
  + R Code
  + Input
  + Grafiken
  + Output

## Trial and Error

## Help
tbc

<!--chapter:end:styleguide.Rmd-->

# Grundlagen

## Objekte

Zu Beginn müssen wir uns die Datenstruktur von R und damit Objekte angucken. Objekte (engl. Objects) speichern verschiedene Datentypen wie Vektoren, Listen, Matrizen oder Funktionen. Als erstes Beispiel erstellen wir einen Vektor mittels `:` Operator. So können wir schnell das Prinzip hinter Objekten verstehen. Dafür erstellen wir ein neues Skript in unserem R-Projekt (siehe Kapitel \@ref(start)). Wir schreiben folgenden Code und führen die Zeile mit `STRG`und `ENTER` aus (alternativ können wir auch den Run-Button in der Toolbar nutzen). Das Ergebnis wird uns in der Console angezeigt.

```r
1:6
## [1] 1 2 3 4 5 6
```

Wir erhalten einen Vektor, das heißt, einen spezifischen Datentyp eines Objekts mit den Ausprägungen 1, 2, 3, 4, 5, 6. In den Sozialwissenschaften ist uns der Objektbegriff eher fremd, weshalb wir uns Objekte auch als eine Variable vorstellen können. In unserem Beispiel hätte die Variable die Ausprägungen eins bis sechs. Allerdings können wir noch nicht mit der Variable weiterarbeiten, sondern müssen diese irgendwo abspeichern. Und nun kommen Objekte ins Spiel: Unsere Variable können wir nämlich in einem Objekt speichern. Alles, was in R gespeichert wird, ist ein Objekt und beinhaltet einen Namen und eine Klasse. Letzteres werden wir später behandeln, zunächst geben wir unserem Objekt einen Namen und weisen mit dem `<-` Operator einen entsprechenden Wert zu. Wir speichern nun den Wert 1 im Objekt a.


```r
a <- 1
```

Wenn wir den Code ausführen und nichts passiert, dann haben wir alles richtig gemacht (ansonsten kommt eine Fehlermeldung). Der Name unseres Objekts lautet nun a, mit dem kleiner-als und dem Minus-Zeichen weisen wir dem Objekt den Wert 1 zu. Anders formuliert: Der Wert 1 ist in der Variable a gespeichert. Wenn wir wissen möchten, was in unserer Variablen gespeichert ist, können wir einfach in der nächsten Zeile a schreiben und den Code ausführen. Wir können nun mit unserem Objekt arbeiten und beispielsweise mit 2 addieren, das Ergebnis bekommen wir direkt angezeigt. 


```r
#wir nehmen den Vektor "a" aus dem vorherigen Beispiel
a <- 1

a + 2
## [1] 3
```

Ist unsere Addition a + 2 nun im Objekt a abgespeichert? Nein, aber wir können das Ergebnis in einem neuen Objekt sichern. Dafür überlegen wir uns einfach einen neuen Namen (zum Beispiel b).


```r
#speichern die Addition im Vektor "b"
b <- a + 2

b
## [1] 3
```

Achtung: R ist case-sensitiv! Das heißt, es macht einen Unterschied, ob wir den Namen unseres Objekts mit Klein- oder Großbuchstaben (zum Beispiel b oder B) schreiben. Ein Name darf nicht mit einer Zahl beginnen und darf bestimmte Sonderzeichen nicht beinhalten (zum Beispiel *, #, !, $, @). Allerdings können Namen mit einem Unterstrich (my_variable), Bindestrich (my-variable) oder einem Punkt (my.variable) geschrieben werden, allerdings nicht beginnen (_myvariable). Wir sollten uns außerdem an bestimmte Konventionen beziehungsweise Routinen halten. Diese Routinen können uns das Leben enorm erleichtern (siehe Kapitel \@ref(style))

<!--chapter:end:grundlagen.Rmd-->

