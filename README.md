# SIP-Fehleranalyse – Downloads

Dieses Repository enthält ausschließlich die offiziellen Windows-Releases der SIP-Fehleranalyse.

## Download

Die aktuelle Version befindet sich unter [Releases](https://github.com/Ichbinsnur92/TK_Tool-Releases/releases/latest). Dort stehen bereit:

- die portable Windows-Anwendung als ZIP-Datei
- der Windows-Installer
- die Release Notes
- `SHA256SUMS.txt` zur Prüfung der heruntergeladenen Dateien
- `update-manifest.json` und `update-manifest.sig` für kryptografisch abgesicherte In-App-Updates

## Sichere One-Click-Updates

Ab SIP-Fehleranalyse 1.6.2 kann eine neuere Version direkt innerhalb der Anwendung heruntergeladen und installiert werden. Vor der Installation prüft die Anwendung das separat ECDSA-signierte Update-Manifest sowie Dateigröße und SHA-256 des ausgewählten Pakets. Ohne gültiges `update-manifest.json` und `update-manifest.sig` wird kein automatisches Update ausgeführt.

Version 1.6.5 stellt diese sichere Updatekette nach dem fehlerhaften 1.6.4-Release wieder vollständig her. Installationen von 1.6.3 können daher direkt auf 1.6.5 aktualisieren.

## Integrität prüfen

Nach dem Download kann die SHA-256-Prüfsumme in PowerShell verglichen werden:

```powershell
Get-FileHash .\SIP-Fehleranalyse-v1.6.5-Setup.exe -Algorithm SHA256
```

Der ausgegebene Hash muss mit dem entsprechenden Eintrag in `SHA256SUMS.txt` übereinstimmen.

Die veröffentlichte Anwendung enthält zusätzlich ein signiertes Integritätsmanifest und prüft ihre eigene Programmdatei sowie den Update-Helfer beim Start.

## Windows-Sicherheitshinweis

Die Dateien sind derzeit nicht kommerziell code-signiert. Windows SmartScreen kann deshalb beim ersten Start vor einem unbekannten Herausgeber warnen. Dateien sollten ausschließlich aus diesem Release-Bereich geladen werden.

## Datenschutz

Dieses Repository enthält keinen Quellcode, keine Lizenzschlüssel, keine Lizenzgeneratoren, keine Testlizenzen, keine Zugangsdaten und keine Kundendaten.

© 2026 SIP-Fehleranalyse Projekt. Alle Rechte vorbehalten.
