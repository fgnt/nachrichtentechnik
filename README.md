# Python-Notebooks zur Übung Nachrichtentechnik

Die in diesem Repository enthaltenen Notebooks werden in der Übung zur Vorlesung
Nachrichtentechnik verwendet. Sie dienen der Visualisierung des Vorlesungsstoffs
und der Übungsaufgaben.

[Direktlink zu den Notebooks](https://github.com/fgnt/nachrichtentechnik/tree/master/notebooks/Uebungen)

## Überblick

Die Notebooks bestehen aus Zellen mit [Python](https://docs.python.org/3.6/)-Code und deren Ausgaben sowie aus
Zellen, in denen Erklärungen mit Markdown und Formeln mit LaTeX gesetzt sind.
Der Python-Code ist hauptsächlich dazu da, um Visualisierungen zu erstellen.
Einige der Visualisierungen sind animiert, d.h. es können z.B. durch
Schieberegler Parameter variiert und die Auswirkungen auf den Plot betrachtet
werden.

Für den Code werden Pakete aus dem [SciPy](http://scipy.org/)-Stack verwendet.
Damit erhält Python einen Funktionsumfang, der sehr nahe an den von MATLAB
heranreicht (es fehlt allerdings eine Alternative zu Simulink), ohne dass teure Lizenzen notwendig sind.
[Es gibt aber Unterschiede in Syntax und Semantik zwischen Python und MATLAB
](https://docs.scipy.org/doc/numpy-dev/user/numpy-for-matlab-users.html).

Die Darstellung der Notebooks erfolgt durch [jupyter](https://jupyter.org).
Für die numerischen Berechnungen werden die Pakete
[numpy](https://docs.scipy.org/doc/numpy/) und
[scipy](https://docs.scipy.org/doc/scipy/reference/) verwendet und
die Visualisierungen werden mit [matplotlib](http://matplotlib.org/index.html)
und [ipython](https://ipython.org/) erstellt.

## Download der Notebooks

Das ganze Notebook-Repository kann entweder mit
[git](https://git-scm.com/downloads) geklont werden [(GitHub Help:
Cloning a Repository)](https://help.github.com/articles/cloning-a-repository/):

```
$> git clone https://github.com/fgnt/nachrichtentechnik.git  PATH/TO/DESTINATION
```

oder als
[Zip-Datei](https://github.com/fgnt/nachrichtentechnik/archive/master.zip) heruntergeladen und entpackt werden.
Die Variante mit git wird empfohlen, weil häufig aktualisiert wird und die
Änderungen einfach mit

```
$> git pull
```

heruntergeladen werden können, wenn man sich im Verzeichnis des Repositories befindet.


## Installation und Start eines Jupyter-Servers

Die Notebooks können direkt auf github betrachtet werden. Um die Animationen
verwenden zu können, müssen sie aber durch einen jupyter-Notebookserver gerendert werden.
Dies kann durch eine der folgenden Alternativen erreicht werden:
 - Installation einer Python-Distribution für wissenschaftliches Programmieren (z.B.
    [anaconda](https://www.continuum.io/downloads))
 - Nutzung eines Online-Hostingservices (z.B.
   [SageMathCloud](https://cloud.sagemath.com/settings))


### Installation von Anaconda

Es gibt viele Möglichkeiten, um an eine geeignete Python-Distribution zu kommen.
Hier wird [anaconda](https://www.continuum.io/downloads) empfohlen.
Nach Download des Installationsprogramms für **python-3.5** und das passende
Betriebssystem (Hinweis für Linux-Nutzer: Der Ort des bin-Verzeichnisses von
anaconda sollte der PATH-Variable hinzugefügt werden, was das Install-Skript
aber ohnehin vorschlägt).

Im offenen Terminal kann dann in das Verzeichnis mit den Notebooks gewechselt
und mittels

```
$> jupyter noteboook
```

ein Server gestartet werden. Dadurch sollte ein Browserfenster mit dem Inhalt
des Verzeichnisses geöffnet werden. Ein Notebook kann dann durch Hinnavigieren
und anklicken geöffnet werden.

### Nutzung von SageMathCloud

Nach Aufruf der [Webseite](https://cloud.sagemath.com/) muss zunächst ein
Account erstellt werden. Dazu kann auch ein vorhandenes Google-, GitHub-,
Twitter- oder Facebook-Konto verwendet werden.

Nach erfolgter Anmeldung kann ein neues Projekt erstellt werden.
Nach einem Klick auf den Menüpunkt "+New" können die Notebook-Dateien dann
einzeln hochgeladen werden.

Ein Notebook kann dann durch Wechsel auf "Files" und anklicken geöffnet werden.
Der jupyter-Server läuft in der SageMathCloud und muss nicht selbst gestartet
werden.

## Kurzeinstieg in die Nutzung von Jupyter

Die Notebooks werden im Browser gerendert. Dazu wird der Inhalt in einzelne
Zellen unterteilt.

Mithilfe von **Ctrl+m h** kann die Hilfe angezeigt werden.

Einzelne Zellen können mit **Ctrl+Enter** oder **Shift+Enter** ausgeführt werden.
estart & Run All** ausgeführt werden.

Wird gerade keine Zelle editiert (sonst **Esc** drücken), kann durch Drücken von **a** oder
**b** eine neue Zelle vor oder nach der alten eingefügt werden (oder das "+" in
der Menüleiste drücken).

Der Modus einer Zelle kann mit **Ctrl+m m** und **Ctrl-m y** zwischen Markdown
und Python-Code gewechselt werden (Das geht auch über die Menüleiste).

### Python-Zellen
In eine Python-Zelle kann beliebiger Python-Code geschrieben und ausgeführt
werden. Alle Code-Zellen teilen sich einen globalen Gültigkeitsbereich für
Variablen, Klassen und Funktionen haben aber ihre eigenen lokalen
Gültigkeitsbereiche.

Wenn ein Paket verwendet wird, muss es zuvor per
[import](https://docs.python.org/3.6/tutorial/modules.html#packages) importiert werden.

### Markdown-Zellen
Nach Wechsel des Modus auf [Markdown](http://jupyter-notebook.readthedocs.io/en/latest/examples/Notebook/Working%20With%20Markdown%20Cells.html) 
per **Ctrl+m m** kann strukturierter Text eingegeben werden.
Damit ist es auch möglich, Gleichungen in LaTeX-Formelsyntax zu setzen.

