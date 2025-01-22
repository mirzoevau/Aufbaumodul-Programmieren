# Aufbaumodul-Programmieren
Projektbeschreibung: Einkaufsliste Assistent
Dieses Python-Projekt, das im Rahmen des Moduls Macromedia Python-Projekt 2 als objektorientiertes Programm entwickelt wurde, konzentriert sich auf die Erstellung eines Einkaufslisten-Assistenten mit dem Schwerpunkt auf objektorientierter Programmierung (OOP). Dabei wurden wesentliche Änderungen und Verbesserungen im Vergleich zu einem ursprünglich funktionsorientierten Ansatz vorgenommen.
1. Umstellung auf JSON statt CSV
Die ursprünglich verwendeten CSV-Operationen wurden durch das flexiblere und besser für komplexe Datenstrukturen geeignete JSON-Format ersetzt. Die Einkaufsliste wird nun in einer JSON-Datei gespeichert und geladen. 
2. Dateistruktur des Projekts
Das Projekt wurde in Form eines Python-Pakets organisiert, das aus zwei Hauptteilen besteht:
•	einkaufsliste_paket: Enthält das Modul mit den Klassen und Methoden zur Verwaltung der Einkaufsliste.
•	main.py: Das Hauptprogramm, das die Einkaufsliste über ein Menü steuert und mit dem Nutzer interagiert.
3. Objektorientierter Ansatz (OOP)
Das Projekt wurde auf OOP umgestellt, wobei alle Funktionen in Klassen strukturiert wurden. Eine Basisklasse namens EinkaufslisteBasis wurde erstellt, die Grundfunktionen wie das Hinzufügen, Bearbeiten und Entfernen von Artikeln bereitstellt. 
Zusätzlich wurde eine abgeleitete Klasse ErweiterteEinkaufsliste eingeführt, die zusätzlichen Funktionalitäten wie das Sortieren, Anzeigen von Statistiken und Suchen von Artikeln bietet.
Grundlegende Methoden der Basisklasse:
__init__: Initialisiert die Einkaufsliste, indem sie aus einer JSON-Datei geladen wird.
artikel_anzeigen: Zeigt die Artikel der Liste an.
artikel_hinzufügen: Fügt neue Artikel zur Einkaufsliste hinzu oder aktualisiert die Menge eines vorhandenen Artikels.
artikel_bearbeiten: Ermöglicht das Bearbeiten der Menge eines Artikels.
artikel_entfernen: Entfernt Artikel aus der Liste.
lade_einkaufsliste: Lädt die Einkaufsliste aus einer JSON-Datei.
speichere_einkaufsliste: Speichert die aktuelle Einkaufsliste in einer JSON-Datei.
Erweiterte Funktionalitäten in der abgeleiteten Klasse:
artikel_sortieren: Sortiert die Artikel alphabetisch.
einkaufsliste_leeren: Leert die Einkaufsliste komplett.
statistik_anzeigen: Zeigt Statistiken über die Artikel (z.B. Artikel mit der höchsten/niedrigsten Menge).
artikel_suchen: Sucht nach Artikeln in der Einkaufsliste.

4. Farbausgabe mit colorama
Für eine benutzerfreundliche Darstellung von wichtigen Informationen in der Konsole werden farbige Ausgaben über das Modul colorama unterstützt.
5. Virtuelle Umgebung und Abhängigkeiten
Das Projekt wurde in einer virtuellen Umgebung ausgeführt, um die Entwicklungsumgebung von der globalen Python-Installation zu isolieren. Alle notwendigen Abhängigkeiten des Projekts, einschließlich colorama und json, wurden in einer requirements.txt Datei gespeichert, um eine einfache Reproduzierbarkeit der Umgebung zu gewährleisten. Diese Datei listet alle notwendigen Python-Pakete und deren Versionen auf, die für den reibungslosen Ablauf des Programms erforderlich sind.
Zusammenfassung
Das Projekt stellt eine vollständig objektorientierte Lösung für die Verwaltung einer Einkaufsliste bereit. Durch die Nutzung von JSON zur Speicherung und die Einführung einer Vererbungshierarchie bietet es flexible und erweiterbare Funktionen. Die Farbausgabe in der Konsole verbessert zudem die Benutzerfreundlichkeit.
