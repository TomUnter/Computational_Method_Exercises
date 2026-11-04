# Computational Methods – Coursework Revisited

Überarbeitete Python-Versionen früherer MATLAB-Studienübungen aus numerischen Methoden und Computational Biology. Das Jupyter-Notebook verbindet kurze Erklärungen mit Implementierungen, Beispielen, Visualisierungen und grundlegenden Tests.

## Inhalt

- **Monte-Carlo-Schätzung von π** mit Standardfehler und Konvergenzgrafik.
- Monte-Carlo-Integration als einfache Variante und mit kumulativem Konvergenzverlauf.
- Needleman–Wunsch für globales Sequenzalignment mit linearen Gap-Kosten und Traceback.
- Ziffernklassifikation mit einem kleinen neuronalen Netz, Baseline und Konfusionsmatrix.
- Zulässige Nachbarzustände und Simulated Annealing für das 0/1-Rucksackproblem; exakte Enumeration als Referenz für kleine Beispiele.

## Installation und Ausführung

Voraussetzung: Python 3.10 oder neuer.

```bash
python -m pip install numpy pandas matplotlib scikit-learn jupyter
jupyter notebook
```

Das Notebook `Computational_Methods_Uebungen.ipynb` öffnen und alle Zellen von oben nach unten ausführen. Nach einer gemeinsamen Importzelle folgt eine eigene Codezelle pro Übung. Der Zifferndatensatz wird mit scikit-learn mitgeliefert; zusätzliche Datendateien oder Downloads sind nicht erforderlich.

## Reproduzierbarkeit und Grenzen

Die Beispiele verwenden feste Zufallsseeds und enthalten grundlegende Assertions. Bibliotheksversionen werden zu Beginn ausgegeben. Ergebnisse können sich zwischen Softwareversionen unterscheiden; die Tests sind keine vollständige Verifikation.

Simulated Annealing garantiert kein globales Optimum. Die Ziffernklassifikation ist ein didaktisches MLP-Beispiel, kein Residual Network und keine diagnostische Anwendung.

## Herkunft

Die ursprünglichen MATLAB-Dateien entstanden als Studienübungen und waren teilweise unvollständig. Dieses Notebook enthält nachträglich überarbeitete Python-Neufassungen für die Lehre während dem Masterstudium. Für das neuronale Netz wurden Datensatz und Bibliothek ersetzt; die Rucksackoptimierung wurde zu einer vollständigen Heuristik ergänzt.

Autor der ursprünglichen Übungen und nachträgliche Überarbeitung: Tom Unterleiter.

Datensatzinformationen: Dokumentation von `sklearn.datasets.load_digits`.


