# Vorlage zur Erstellung einer Abschlussarbeit / Hausarbeit entsprechend der APA 7 Richtlinien

Dieses Repository enthält eine Quarto Vorlage inklusive einer Quarto Extension. Diese Vorlage wurde für den Kurs empirisches wissenschaftliches Arbeiten erstellt, welchen ich für die Charlotte Fresenius Hochschule gehalten habe. Die Kurssprache und die Sprache der Vorlage ist Deutsch. Diese Vorlage erleichtert es, einen Text - inklusive Deckblatt - entsprechend der APA 7 Richtlinien mit Quarto zu erstellen. 

# Vorbereitung des PCs

- Installieren Sie R: [https://www.r-project.org/](https://cran.rstudio.com/)
- Installieren Sie R Studio: [https://posit.co/download/rstudio-desktop/](https://posit.co/download/rstudio-desktop/)
- Installieren Sie Quarto (Version = 1.4 oder höher): [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)
- Installieren Sie das R Paket `quarto` mit
```{r}
install.packages("quarto")
```
Das `quarto` Paket in R ist nicht Quarto selbst, aber es bietet praktische Funktionen zur Interaktion mit Quarto in R.

# Herunterladen des Repos

## Methode 1: Verwendung der Maus

### Methode 1a: Klicken in GitHub

Klicken Sie in GitHub auf die grüne Schaltfläche `<> Code v`, die Sie in diesem Repository finden. In dem sich öffnenden Kontextmenü finden Sie eine Schaltfläche namens `Download ZIP`. Klicken Sie darauf und Sie haben eine gezippte Kopie des Repos, die Sie entzippen und verwenden können.

### Methode 1b: Klicken Sie auf [diesen Link](https://github.com/hubchev/temp_apa_de/zipball/HEAD)

Sie können das Repository mithilfe [dieses Link](https://github.com/hubchev/temp_apa_de/zipball/HEAD) in einer gezippten Datei herunterladen. Jetzt können Sie es in ein Verzeichnis Ihrer Wahl entzippen.

## Methode 2: Verwendung von R

### Methode 2 a): `quarto_use_template()`

Wenn Sie das R Paket `quarto` installiert haben, kann die Vorlage mit der Funktion `quarto_use_template` kopiert werden. Setzen Sie hierzu Ihr Arbeitsverzeichnis auf das Verzeichnis, in dem Sie die Vorlage installieren möchten (z.B. `setwd("pfad/zu/meinem/ordner")`). Stellen Sie sicher, dass das Verzeichnis leer ist und führen Sie diesen Befehl aus:

```{r}
quarto::quarto_use_template("hubchev/temp_apa_de")
```

Eine Eingabeaufforderung fragt, ob Sie dem Autor (mir) vertrauen, keinen schädlichen Code auszuführen. Um fortzufahren, antworten Sie mit `Yes` oder einfach `Y`.

### Methode 2 b): usethis::use_course()

Installieren und laden Sie das usethis-Paket und laden Sie es mit `use_course` herunter:

```{r}
install.packages("usethis")
library("usethis")
usethis::use_course("hubchev/temp_apa_de", destdir = getwd())
```

Standardmäßig wird das Repository in ein Verzeichnis heruntergeladen und in Ihrem Arbeitsverzeichnis gespeichert. Ersetzen Sie `getwd()` gerne durch "pfad/zum/ziel", d.h. den gewünschten Speicherort auf Ihrem System, an dem Sie das Repository herunterladen möchten.

## Methode 3: Verwendung des Terminals

### Methode 3a: Verwendung von Git

Wenn Sie Git auf Ihrem System installiert haben ([hier](https://git-scm.com/downloads) können Sie es ggf. runterladen), können Sie dieses Repository mithilfe der Befehlszeile herunterladen:

- Öffnen Sie das Terminal in R Studio (In RStudio befindet sich das Terminal in einer Registerkarte neben der Konsole.) oder das Eingabeaufforderungsfenster Ihres Betriebssystems.
- Navigieren Sie zu dem Verzeichnis, in das Sie das Repository herunterladen möchten, mithilfe des cd-Befehls (z.B. `cd ~/Dokumente`).
- Führen Sie den folgenden Befehl aus, um das Repository zu klonen:

```{bash}
git clone https://github.com/hubchev/temp_apa_de.git
```

### Methode 3a: Verwendung von Quarto

Verwenden Sie das Terminal (In RStudio befindet sich das Terminal in einer Registerkarte neben der Konsole.), um zu dem Verzeichnis zu navigieren, in das Sie die Vorlage kopieren möchten (z.B. cd pfad/zu/meinem/ordner). Stellen Sie sicher, dass das Verzeichnis leer ist und führen Sie diesen Befehl aus:

```{bash}
quarto use template hubchev/temp_apa_de
```


# Verwendung der Vorlage

Sobald Sie das Repository heruntergeladen haben, navigieren Sie zu dem Verzeichnis, in das Sie es heruntergeladen haben, und öffnen Sie die Datei `temp_apa_de.qmd` in RStudio oder Ihrem bevorzugten Editor. Passen Sie die Vorlage an, um Ihre eigene Arbeit zu erstellen!

Um die Quarto-Datei in das gewünschte Dokument (z.B. ein PDF oder HTML) umzuwandeln, "rendern" Sie die Datei `exam_template.qmd`. Sie können dies in RStudio tun, indem Sie die Datei öffnen und auf die Schaltfläche "Render" klicken oder indem Sie den folgenden Befehl in der R-Konsole ausführen:

```{r}
quarto_render("pfad/zu/temp_apa_de.qmd")
```

Ersetzen Sie "pfad/zu/temp_apa_de.qmd" durch den tatsächlichen Pfad zur Datei.


# Feedback

Wenn Sie Fragen haben oder Hilfe bei der Vorlage benötigen, zögern Sie nicht, via GitHub Änderungen per `pull request` einzuarbeiten oder mich zu kontaktieren. 