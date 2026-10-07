# GHOST//SHELL

Ein kleines Hacking-Puzzle im Terminal-Look – spielbar direkt im Browser, optimiert fürs Handy.
Alles ist **rein fiktiv**: erfundene Server, erfundene Personen, keine echten Exploits und keine echten Zugangsdaten.

> **Screenshot:** *folgt* – lege später ein Bild unter `docs/screenshot.png` ab und ersetze diese Zeile durch `![Screenshot](docs/screenshot.png)`.

## Spielen

**[https://magnethelm90.github.io/Gametesr](https://magnethelm90.github.io/Gametesr)**

Oder lokal: Datei `index.html` herunterladen und im Browser öffnen. Es gibt keine Abhängigkeiten und keinen Build-Schritt.

## So spielst du

Du bist „Ghost“ und löst siebzehn Missionen. Gib Befehle ein oder tippe die Knöpfe unten am Bildschirm an.

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
| 17 – Der Tresorcode | Finale: Mastermind mit zufälligem 4-stelligem Code. |

Wichtige Befehle (mit `hilfe` siehst du immer alle):

- `hilfe` – Befehlsübersicht
- `level <n>` – Mission starten (jedes Level schaltet das nächste frei)
- `hinweis` – Tipp zur aktuellen Mission (mehrstufig)
- `status` – Fortschritt anzeigen
- `reset` – Spielstand löschen

Dein Fortschritt wird im Browser (`localStorage`) gespeichert. Es werden keine Daten an einen Server gesendet.

**Spoiler-Hinweis:** Das Spiel ist eine einzelne Datei. Die Lösungen stehen im Quelltext – wer selbst rätseln will, schaut nicht hinein.

## Projektstruktur

```
index.html   Das komplette Spiel (HTML, CSS, JavaScript)
README.md    Diese Datei
LICENSE      MIT-Lizenz
.gitignore   Ignorierte Dateien
```

## Lizenz

[MIT](LICENSE)

## Dank & Quellen

- Der Terminal-Stil ist inspiriert von dem Spiel „The Operator“. Es wurde kein Code, keine Grafik und kein Text daraus übernommen.
- Die IP-Adressen in Level 3 stammen aus den für Dokumentation reservierten Bereichen nach [RFC 5737](https://www.rfc-editor.org/rfc/rfc5737) und sind damit nie echten Rechnern zugeordnet.
