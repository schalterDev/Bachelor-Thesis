Bachelorthesis von Martin Schalter geschrieben an der [HS-Mannheim](https://www.hs-mannheim.de/) für [CROSSLOAD](https://crossload.org).

# Technische Informationen

Diese Thesis wurde mithilfe der [LaTeX-Vorlage der HS-Mannheim](https://github.com/informatik-mannheim/thesis-template) erstellt.

## Lokale Entwicklungsumgebungen

Zum Erzeugen der fertigen Arbeit dienen die Skripte `create` und `clean`. Die .cmd-Version ist für Windows, die .sh für Unix/Linux.

Zusätzlich liegt im Verzeichnis `/tex` noch ein Makefile mit dem man die Quellen mit Hilfe von `make` übersetzen kann. Der Vorteil hiervon ist, dass `make` erkennt, ob sich Inhalte geändert haben und nur dann die Arbeit neu übersetzt.

Sie können auch eine integrierte Entwicklungsumgebung verwenden. Hierbei haben sich folgende bewährt:

  * [TeXnicenter](http://www.texniccenter.org/) für Windows (siehe unten)
  * [Texmaker](http://www.xm1math.net/texmaker/) für Windows, MacOS und Linux

Ausserdem müssen sie LaTeX auf Ihrem Rechner installieren. Bei Linux erfolgt dies einfach über den Paketmanager der verwendeten Distribution, z.B. `sudo apt install texlive-full` für Ubuntu. Für Windows und MacOS empfehlen sich:

  * [MikTeX](http://miktex.org/) für Windows
  * [MacTeX](http://tug.org/mactex/) für MacOS

Für die Verwaltung der Literaturliste wird das BibTeX-Format verwendet (Datei `literatur.bib`). Obwohl Sie diese Datei auch von Hand bearbeiten können, empfiehlt es sich, hierfür ein Werkzeug einzusetzen. Bewährt haben sich:

  * [JabRef](http://jabref.sourceforge.net/) für Windows, MacOS und Linux
  * [BibDesk](http://bibdesk.sourceforge.net/) für MacOS

Achten Sie darauf, die Dokumente im UTF-8-Format abzulegen. Nur so ist eine plattformunabhängige Verwendung gewährleistet. 

## Aufbau der Vorlage

  * `thesis.tex` - Hauptdokument. Hier werden weitere Kapitel aus dem Ordner `kapitel` inkludieren.
  * `docinfo.tex` - Bibliografische Informationen zur Arbeit
  * `kapitel/abkuerzungen.tex` - Liste der in der Arbeit verwendeten Abkürzungen
  * `kapitel/kapitel1.tex` - Einleitung
  * `kapitel/kapitel2.tex` - Grundlagen
  * `kapitel/kapitel3.tex` - Anforderungsanalyse
  * `kapitel/kapitel4.tex` - Konzeption
  * `kapitel/kapitel-5.tex` - Implementierung
  * `kapitel/kapitel-6.tex` - Evaluation und Reflexion
  * `kapitel/kapitel-7.tex` - Zusammenfassung und Ausblick
  * `literatur.bib` - Literaturdatenbank im BibTeX-Format

Normalerweise nicht verändern müssen Sie

  * `preambel.tex` - Einstellungen zum Dokument.
  * `titelblatt.tex` - Titelblatt der Arbeit

Die Vorlage ist für doppelseitigen Druck optimiert. Wenn Sie die Arbeit einseitig ausdrucken, sieht das Ergebnis seltsam aus, weil es unnötig viele leere Seiten enthält und die Seitenzahlen zwischen rechtem und linkem Rand springen. Für **einseitigen Druck** müssen sie die Datei `preambel.tex` ändern und `twoside=on` in `twoside=off` ändern.

Es gibt drei Ordner

  * `/kapitel` - Ablageort für die einzelnen Kapitel
  * `/bilder` - Ablageort für die verwendeten Bilder
  * `/src` - Ablageort für die verwendeten Quelltexte von Programmen, die in der Arbeit gezeigt werden sollen.
