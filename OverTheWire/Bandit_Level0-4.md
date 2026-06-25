markdown
OverTheWire — Bandit Level 0-4

Level 0
SSH-Verbindung aufbauen:
ssh bandit0@bandit.labs.overthewire.org -p 2220
Passwort: bandit0

Mit `ls` die Datei gefunden, mit `cat readme` das Passwort gelesen.

Level 1
Datei heißt `-` (Sonderzeichen). Normales `cat -` funktioniert nicht.
Lösung: `cat ./-`

Level 2
Datei mit Sonderzeichen im Namen.
Lösung: `cat ./- -`

Level 3
Datei liegt in einem Ordner, ist versteckt.
cd inhere
ls -a
cat ...Hiding-From-You

Level 4
Mehrere Dateien im Ordner, nur eine ist lesbar.
file ./-file*
cat ./-file07

Gelernt
- SSH-Verbindung aufbauen
- Dateien mit Sonderzeichen lesen
- Versteckte Dateien finden mit `ls -a`
- Dateitypen prüfen mit `file`
