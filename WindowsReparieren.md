# Windows 10 Reparatur

## Für wen ist der Guide?

- Windows Updates lassen sich nicht installieren.
- Manche Windows-Komponenten funktionieren nicht wie sie sollen.
- Allgemeine Probleme mit Windows.
- Du wurdest hierher geschickt.

## Was muss ich tun?

###  Schon neugestartet?
Nein wirklich, ein Neustart löst oft einige Probleme.

### Backup?
Heute schon gesichert? Stellt bitte *vorher* sicher, dass eure Daten gesichert sind. Dieser Guide sollte natürlich keinen Datenverlust verursachen, dennoch lässt es sich nie ausschließen.

### CMD
*Was ist die CMD?* Die CMD oder auch Eingabeaufforderung ist das Terminal von Windows. 

*Wie rufe ich die CMD auf?* Klickt auf das Startmenü und gebt dort entweder "Eingabeaufforderung" oder "cmd" ein. Falls hier im Guide erwähnt wird, dass ihr es als Administrator ausführen sollt, klickt mit rechts auf das Suchergebnis und wählt "Als Administrator ausführen" aus. Wenn ihr alles richtig gemacht habt, erscheint ein schwarzes Fenster mit dem Titel "Eingabeaufforderung" oder "Administrator Eingabeaufforderung".

### Reparatur mit DISM
Daten gesichert? Dann geht's los.

- Öffnet eine Eingabeaufforderung als Administrator.
- `DISM /Online /Cleanup-Image /RestoreHealth` eingeben und mit Enter bestätigen.
- Für diesen Befehl wird eine Internetverbindung benötigt.
- Ihr könnt die Reparatur auch mit einem originalen, offline, Windows Image durchführen, [hier](https://docs.microsoft.com/de-de/windows-hardware/manufacture/desktop/repair-a-windows-image) findet ihr die Anleitung von Microsoft.
- Windows prüft nun eure Installation auf Fehler und versucht diese zu reparieren.
- [Die Prüfung sollte so aussehen.](https://i.imgur.com/moxcTrB.png)
- [Nachdem die Prüfung und Reparatur abgeschlossen ist](https://i.imgur.com/gPdJAgf.png), führt bitte einen Neustart durch.
- Prüft im Anschluss, ob euer Problem behoben wurde.

### Reparatur mit SFC
Daten gesichert? Dann geht's los.

- Öffnet eine Eingabeaufforderung als Administrator.
- `sfc /scannow` eingeben und mit Enter bestätigen.
- Windows prüft nun eure Installation auf Fehler und versucht diese zu reparieren.
- [Die Prüfung sollte so aussehen.](https://i.imgur.com/PgyF9Ax.png)
- [Nachdem die Prüfung und Reparatur abgeschlossen ist](https://i.imgur.com/zTAsGZv.png), führt bitte einen Neustart durch.
- Prüft im Anschluss, ob euer Problem behoben wurde.

### Windows mit Bordmitteln wiederherstellen
Daten gesichert? Dann geht's los.

- Öffnet die Windows Einstellungen.
- Klickt auf den Punkt "Update und Sicherheit".
- Klickt links im Menü auf "Wiederherstellung".
- Klickt beim Punkt "Diesen PC zurücksetzen" auf "Los geht's".
- Ihr könnt nun auswählen, ob ihr eure Dateien und Programm behalten wollt oder ob ihr Windows komplett zurücksetzen wollt.
- **Achtung:** Der letzte Punkt löscht eure Daten! Stellt sicher, dass ihr ein Backup habt! Der erste Punkt *sollte* eure Daten nicht löschen, stellt trotzdem sicher, dass ihr ein Backup habt.

### Windows mit der ISO wiederherstellen
Daten gesichert? Dann geht's los.

- Einen umfangreichen Guide findet ihr [hier.](https://www.microsoft.com/de-de/software-download/windows10)

### Was, wenn alles nichts hilft?

> Aber /u/efflicto, ich habe alles getan und mein Problem besteht weiterhin!

- Gebt bitte ein genaues Feedback, falls ihr aus einem Thread hierhergeschickt wurdet.
- Erstellt einen Thread im /r/de_EDV Subreddit mit genauen Informationen.
- Schreibt alle Informationen, Logs etc. rein, lieber mehr, als zuwenig!
