# SIP-Fehleranalyse – Downloads

Dieses Repository enthält ausschließlich die offiziellen Windows-Releases der SIP-Fehleranalyse.

## Download

Die aktuelle Version befindet sich unter [Releases](https://github.com/Ichbinsnur92/TK_Tool-Releases/releases/latest). Dort stehen bereit:

- die portable Windows-Anwendung als ZIP-Datei
- der Windows-Installer
- die Release Notes
- `SHA256SUMS.txt` zur Prüfung der heruntergeladenen Dateien
- `update-manifest.json` und `update-manifest.sig` für kryptografisch abgesicherte In-App-Updates

## One-Click-Updates ab Version 1.6.2

SIP-Fehleranalyse 1.6.2 enthält erstmals den integrierten One-Click-Updater. Nachfolgende korrekt veröffentlichte Versionen können direkt innerhalb der Anwendung gesucht, heruntergeladen, kryptografisch geprüft und installiert werden.

Der Wechsel von 1.6.1 auf 1.6.2 muss einmalig über den normalen Installer beziehungsweise das vollständige Portable-Paket erfolgen, da 1.6.1 den separaten Update-Helfer noch nicht enthält.

## Integrität prüfen

Nach dem Download kann die SHA-256-Prüfsumme in PowerShell verglichen werden:

```powershell
Get-FileHash .\SIP-Fehleranalyse-v1.6.2-Setup.exe -Algorithm SHA256
```

Der ausgegebene Hash muss mit dem entsprechenden Eintrag in `SHA256SUMS.txt` übereinstimmen.

Die Anwendung selbst akzeptiert automatische Updates nur, wenn das Release ein gültiges ECDSA-signiertes Update-Manifest enthält und Dateigröße sowie SHA-256-Prüfsumme des heruntergeladenen Pakets mit den signierten Metadaten übereinstimmen.

## Windows-Sicherheitshinweis

Die Dateien sind derzeit nicht kommerziell code-signiert. Windows SmartScreen kann deshalb beim ersten Start vor einem unbekannten Herausgeber warnen. Dateien sollten ausschließlich aus diesem Release-Bereich geladen werden.

## Datenschutz

Dieses Repository enthält keinen Quellcode, keine Lizenzschlüssel, keine Lizenzgeneratoren, keine Testlizenzen, keine Zugangsdaten und keine Kundendaten.

© 2026 SIP-Fehleranalyse Projekt. Alle Rechte vorbehalten.
