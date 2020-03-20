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
