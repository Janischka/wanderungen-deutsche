# Wanderungsbewegungen deutscher Staatsbürger:innen (1991–2024)

## Projekt

Wie haben sich die Zu- und Fortzüge deutscher Staatsbürger:innen seit 1991 entwickelt?

Dieses Datenprojekt untersucht die Wanderungsbewegungen zwischen Deutschland und dem Ausland. Ein besonderer Fokus liegt auf dem Einfluss der (Spät-)Aussiedlerzuwanderung auf den Wanderungssaldo.

**[Interaktive Visualisierung auf Datawrapper](https://www.datawrapper.de/_/px7xn/)**

## Datenquellen
Die Analyse basiert auf vier amtlichen Datentabellen des Statistischen Bundesamtes (Destatis):

| Daten | Originalquelle |
|---|---|
| Wanderungen deutscher Staatsbürger:innen, historische Daten | [Destatis](https://www.destatis.de/DE/Themen/Gesellschaft-Umwelt/Bevoelkerung/Wanderungen/Tabellen/wanderungen-zwischen-deutschland-und-dem-ausland-jahr-02.html) |
| Wanderungen deutscher Staatsbürger:innen, neuere Daten | [GENESIS 12711-0005](https://genesis.destatis.de/datenbank/online/statistic/12711/table/12711-0005) |
| (Spät-)Aussiedlerzuzüge, historische Daten | [Destatis](https://www.destatis.de/DE/Themen/Gesellschaft-Umwelt/Bevoelkerung/Wanderungen/Tabellen/wanderungen-deutsche.html) |
| Spätaussiedlerzuzüge, neuere Daten | [GENESIS 12711-0030](https://genesis.destatis.de/datenbank/online/statistic/12711/table/12711-0030) |

## Methodik

Die Daten wurden mit **Python und Pandas** bereinigt, zusammengeführt und ausgewertet.

Neben den amtlichen Wanderungszahlen wurden zwei zusätzliche Kennzahlen berechnet:

- **Bereinigte Zuzüge:** Zuzüge deutscher Staatsangehöriger minus (Spät-)Aussiedlerzuzüge.
- **Bereinigter Wanderungssaldo:** Amtlicher Wanderungssaldo minus (Spät-)Aussiedlerzuzüge.

Die bereinigten Werte sind eigene rechnerische Kennzahlen. Ihre Aussagekraft hängt davon ab, inwieweit die abgezogenen (Spät-)Aussiedler bereits in den deutschen Zuzügen enthalten sind. Änderungen der statistischen Erfassung können zudem die Vergleichbarkeit einzelner Jahre beeinflussen.

## Reproduzierbarkeit

Der vollständige Analysecode befindet sich im Jupyter-Notebook [`analyse_wanderungen.ipynb`](analyse_wanderungen.ipynb).

Die benötigten CSV-Dateien sind ebenfalls im Repository enthalten. Zur Ausführung werden **Python, Pandas und Jupyter Notebook** benötigt. Alle Dateien müssen im selben Verzeichnis liegen.
