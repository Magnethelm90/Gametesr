# GHOST//SHELL

Ein kleines Hacking-Puzzle im Terminal-Look – spielbar direkt im Browser, optimiert fürs Handy.
Alles ist **rein fiktiv**: erfundene Server, erfundene Personen, keine echten Exploits und keine echten Zugangsdaten.

![Screenshot von Level 2: Caesar-Chiffre knacken](docs/screenshot.png)

## Spielen

**[https://magnethelm90.github.io/Gametesr](https://magnethelm90.github.io/Gametesr)**

Oder lokal: Datei `index.html` herunterladen und im Browser öffnen. Es gibt keine Abhängigkeiten und keinen Build-Schritt.

## So spielst du

Du bist „Ghost“ und löst 60 Missionen. Gib Befehle ein oder tippe die Knöpfe unten am Bildschirm an.

| Level | Aufgabe |
|-------|---------|
| 1 – Das Passwort | Finde in Notizen, Profil und Chat heraus, wie das Passwort lautet. |
| 2 – Die Chiffre | Knacke eine Caesar-Chiffre und finde das Codewort. |
| 3 – Der Eindringling | Werte eine Logdatei aus und finde die IP-Adresse des Täters. |
| 4 – Das Datendepot | Wandle ein Base64-Datenpaket zurück und finde das Schlüsselwort. |
| 5 – Das Signal | Lies eine Bitfolge (8 Bit pro Zeichen) und finde die PIN. |
| 6 – Der Netzscan | Finde im fiktiven Firmennetz den Rechner, der am dringendsten abgesichert werden muss. |
| 7 – Der Tresor | Drei Teile, drei Verfahren (ROT13, Hex, rückwärts). |
| 8 – Das Funkfeuer | Knacke eine Vigenère-Chiffre. Das Schlüsselwort steckt in einem Rätsel. |
| 9 – Das Morsesignal | Übersetze ein Lichtsignal in Morsecode. |
| 10 – Die Geheimmail | Finde die versteckte Botschaft in harmlosen Mails (Akrostichon). |
| 11 – Das Alibi | Logikrätsel: Wer von vier Verdächtigen ist der Täter? |
| 12 – Das Mainframe | Navigiere mit `ls`, `cd` und `cat` durch ein Dateisystem und finde das versteckte Passwort. |
| 13 – Die Kurznachricht | Entschlüssele eine SMS aus der Zeit der Handytasten (Multi-Tap). |
| 14 – Der Lizenzschlüssel | Finde die geheime Regel hinter gültigen Schlüsseln und wähle den richtigen. |
| 15 – Der Serverraum | Mini-Textadventure: Keycard und Code finden, Tür öffnen. |
| 16 – Die Zwiebel | Drei Schichten Verschleierung (Base64, ROT13, rückwärts) abtragen. |
| 17 – Der Tresorcode | Mastermind mit zufälligem 4-stelligem Code. |
| 18–28 | Chiffren-Werkstatt: Atbash, Polybius-Gitter, Zahlencode, Buchstabieralphabet, URL-Kodierung, Leetspeak, Zaunschiene, verrutschte Tastatur, XOR, Mehrfachschichten, ASCII. Die Werkzeuge wirken nacheinander auf den aktuellen Text. |
| 29–31 | Logik: zwei weitere Alibi-Rätsel und ein Zahlenschloss mit Hinweisen. |
| 32–35 | Quiz und Zahlen: Zahlenfolgen, Netzwerk-Quiz, Krypto-Quiz, Zahlenraten (binäre Suche). |
| 36–45 | Knobeln: Lichter aus (3x3 und 4x4), zwei Sudokus, zwei Labyrinthe (eins im Dunkeln), Türme von Hanoi (3 und 4 Scheiben), Streichhölzer gegen den Computer, Wort-Ratespiel. |
| 46–49 | Praxis: Passwort per Recherche, Firewall-Regeln prüfen, Backup-Archiv im Dateisystem, Textadventure im Gebäude. |
| 50 – Die große Zwiebel | Vier Schichten, du wählst Werkzeuge und Reihenfolge selbst. |
| 51 – Der Passwort-Knacker | Simulation: Wörterbuch-Angriff auf erfundene Hashes. Welche Passwörter sind zu schwach? |
| 52 – Der Anruf | Gesprächsbaum: Du bist der Verteidiger und erkennst einen Social-Engineering-Anruf. |
| 53 – Der Aufzug | Transport-Rätsel im Rechenzentrum: Virus, Datei und Backup sicher auf die andere Seite bringen. |
| 54 – Der Schaltkreis | Logik-Gatter (UND, ODER, NICHT, XOR): Stelle die Schalter so, dass die richtigen Lampen leuchten. |
| 55 – Operation Dämmerung | Mini-Kampagne in fünf Kapiteln mit zwei Wegen, Rätseln und einer Gewissensentscheidung. |
| 56 – Die Datenbank | Abfragen mit `wo`, `sortiere` und `zeige`: Finde den Verdächtigen im Zugriffsprotokoll. |
| 57 – Der Schlüsselaustausch | Diffie-Hellman mit kleinen Zahlen: Warum es mit großen Zahlen sicher ist, mit winzigen aber nicht. |
| 58 – Das Schiebepuzzle | Acht Kacheln und eine Lücke, in die richtige Reihenfolge bringen. |
| 59 – Das Minenfeld | Logik-Minensucher auf 6x6 Feldern, ganz ohne Raten lösbar. |
| 60 – Das Bilderrätsel | Finale: Nonogramm. Die Zahlen am Rand verraten das Bild. |

Wichtige Befehle (mit `hilfe` siehst du immer alle):

- `hilfe` – Befehlsübersicht
- `level <n>` – Mission starten (jedes Level schaltet das nächste frei)
- `menu alle` – alle 60 Level anzeigen (`menu` zeigt nur die nächsten)
- `hinweis` – Tipp zur aktuellen Mission (mehrstufig)
- `status` – Fortschritt anzeigen
- `sound an|aus` – Ton ein- oder ausschalten (oder oben rechts auf den Knopf tippen)
- `reset` – Spielstand löschen

Die Klänge werden live im Browser erzeugt (Web Audio API), es gibt keine Audiodateien. In Level 9 kannst du das Morsesignal mit `abspielen` auch anhören.

Dein Fortschritt wird im Browser (`localStorage`) gespeichert. Es werden keine Daten an einen Server gesendet.

**Spoiler-Hinweis:** Das Spiel ist eine einzelne Datei. Die Lösungen stehen im Quelltext – wer selbst rätseln will, schaut nicht hinein.

## Sicherheit

- Das Spiel läuft komplett im Browser und sendet nichts an einen Server. Eine eingebaute Content Security Policy blockiert Netzwerkzugriffe, Fremd-Skripte und Formular-Versand.
- Eingaben werden nur als Text angezeigt (`textContent`), nie als HTML.
- Der gespeicherte Spielstand (`localStorage`) wird beim Laden geprüft. Defekte oder manipulierte Daten werden ignoriert.
- Alle Namen, Passwörter und Zugangsdaten im Spiel sind frei erfunden.
- Sicherheitslücke gefunden? Bitte als [Issue](https://github.com/Magnethelm90/Gametesr/issues) melden.

## Projektstruktur

```
index.html   Das komplette Spiel (HTML, CSS, JavaScript)
docs/        Screenshot für die README
README.md    Diese Datei
LICENSE      MIT-Lizenz
.gitignore   Ignorierte Dateien
```

## Lizenz

[MIT](LICENSE)

## Dank & Quellen

- Der Terminal-Stil ist inspiriert von dem Spiel „The Operator“. Es wurde kein Code, keine Grafik und kein Text daraus übernommen.
- Die IP-Adressen in Level 3 stammen aus den für Dokumentation reservierten Bereichen nach [RFC 5737](https://www.rfc-editor.org/rfc/rfc5737) und sind damit nie echten Rechnern zugeordnet.
