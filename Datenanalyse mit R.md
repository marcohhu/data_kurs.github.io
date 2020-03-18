--- 
title: "Datenanalyse mit R"
author: "Marco"
date: "2020-03-18"
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

[Work in Process]

<!--chapter:end:index.Rmd-->

# Einleitung {-}

tbc...

## Who will find this book useful? {-}

Das Buch ist als Ergänzung zur Data-Übung gedacht...


<!--chapter:end:intro.Rmd-->

# Getting started
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

## Pakate

<!--chapter:end:getting-started.Rmd-->

# Styleguide

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

