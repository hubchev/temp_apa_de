# Deutsche Vorlage entsprechend der APA 7 Richtlinien

Dieses Repository enthält eine Vorlage welche es ermöglicht einen Text entsprechend der APA 7 Richtlinien mit Quarto zu erstellen

# Herunterladen des Repos

## Methode 1: Verwendung von R

### Methode 1 a): usethis::use_course()

Installieren und laden Sie das usethis-Paket und laden Sie es mit use_course herunter:

```{r}
# install.packages("usethis")
library("usethis")
usethis::use_course("hubchev/temp_apa_de", destdir = getwd())
```

Standardmäßig wird das Repository in ein Verzeichnis heruntergeladen und in Ihrem Arbeitsverzeichnis gespeichert. Ersetzen Sie getwd() gerne durch "pfad/zum/ziel", d.h. den gewünschten Speicherort auf Ihrem System, an dem Sie das Repository herunterladen möchten.

### Methode 1 b): quarto_use_template()

Installieren Sie das quarto-Paket (Version = 1.4 oder höher). Das quarto-Paket ist nicht Quarto selbst, aber es bietet praktische Funktionen zur Interaktion mit Quarto und Quarto.

Wenn das quarto-Paket nicht installiert ist, können Sie es installieren, indem Sie diesen Code in der Konsole ausführen:

```{r}
install.packages("quarto")
```

Sobald das quarto-Paket installiert ist, können Sie die Vorlage kopieren, indem Sie Ihr Arbeitsverzeichnis auf das Verzeichnis setzen, in dem Sie die Vorlage installieren möchten (z.B. setwd("pfad/zu/meinem/ordner")). Stellen Sie sicher, dass das Verzeichnis leer ist und führen Sie diesen Befehl aus:

```{r}
quarto::quarto_use_template("hubchev/temp_apa_de")
```

Eine Eingabeaufforderung fragt, ob Sie dem Autor (mir) vertrauen, keinen schädlichen Code auszuführen. Um fortzufahren, antworten Sie mit Ja oder einfach J.

## Methode 2: Verwendung von Git

Wenn Sie Git auf Ihrem System installiert haben, können Sie dieses Repository mithilfe der Befehlszeile herunterladen:

- Öffnen Sie das Terminal in R Studio (In RStudio befindet sich das Terminal in einer Registerkarte neben der Konsole.) oder das Eingabeaufforderungsfenster Ihres Betriebssystems.
-  Navigieren Sie zu dem Verzeichnis, in das Sie das Repository herunterladen möchten, mithilfe des cd-Befehls (z.B. cd ~/Dokumente).
-   Führen Sie den folgenden Befehl aus, um das Repository zu klonen:

```{bash}
git clone https://github.com/hubchev/temp_apa_de.git
```

## Methode 3: Verwendung des Terminals

Verwenden Sie das Terminal (In RStudio befindet sich das Terminal in einer Registerkarte neben der Konsole.), um zu dem Verzeichnis zu navigieren, in das Sie die Vorlage kopieren möchten (z.B. cd pfad/zu/meinem/ordner). Stellen Sie sicher, dass das Verzeichnis leer ist und führen Sie diesen Befehl aus:

```{bash}
quarto use template hubchev/temp_apa_de
```

## Methode 4: Verwendung der Maus

### Methode 4a: Klicken in GitHub

Klicken Sie in GitHub auf die grüne Schaltfläche `<> Code v`; Code v, die Sie in diesem Repository finden. In dem sich öffnenden Kontextmenü finden Sie eine Schaltfläche namens `Download ZIP`. Klicken Sie darauf und Sie haben eine gezippte Kopie des Repos, die Sie entzippen und verwenden können.

### Methode 4b: Klicken Sie auf [diesen Link](https://github.com/hubchev/temp_apa_de/zipball/HEAD)

Sie können das Repository mithilfe [dieses Link](https://github.com/hubchev/temp_apa_de/zipball/HEAD) in einer gezippten Datei herunterladen. Jetzt können Sie es in ein Verzeichnis Ihrer Wahl entzippen.

# Verwendung der Vorlage

Sobald Sie das Repository heruntergeladen haben, navigieren Sie zu dem Verzeichnis, in das Sie es heruntergeladen haben, und öffnen Sie die Datei temp_apa_de.qmd in RStudio oder Ihrem bevorzugten Editor. Passen Sie die Vorlage an, um Ihre eigene Arbeit zu erstellen!

Um die Quarto-Datei in ein formatiertes Dokument (z.B. ein PDF oder HTML umzuwandeln), strangen Sie die exam_template.Rmd-Datei. Sie können dies in RStudio tun, indem Sie die Datei öffnen und auf die Schaltfläche "Stricken" klicken oder indem Sie den folgenden Befehl in der R-Konsole ausführen:

```{r}
quarto_render("pfad/zu/temp_apa_de.qmd")
```

Ersetzen Sie "pfad/zu/temp_apa_de.qmd" durch den tatsächlichen Pfad zur Datei.


# Feedback

Wenn Sie Fragen haben oder Hilfe bei der Vorlage benötigen, zögern Sie nicht, via GitHub Änderungen per `pull request` einzuarbeiten oder mich zu kontaktieren. 