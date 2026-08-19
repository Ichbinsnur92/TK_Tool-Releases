# SIP-Fehleranalyse – Downloads

Dieses Repository enthält ausschließlich die offiziellen Windows-Releases der SIP-Fehleranalyse.

## Download

Die aktuelle Version befindet sich unter [Releases](https://github.com/Ichbinsnur92/TK_Tool-Releases/releases/latest). Dort stehen bereit:

- die portable Windows-Anwendung als ZIP-Datei
- der Windows-Installer
- die Release Notes
- `SHA256SUMS.txt` zur Prüfung der heruntergeladenen Dateien

## Update-Prüfung

Die SIP-Fehleranalyse prüft auf Wunsch beziehungsweise regelmäßig, ob in diesem öffentlichen Repository eine neuere Version veröffentlicht wurde. Wird eine neuere Version gefunden, kann die offizielle GitHub-Release-Seite direkt aus der Anwendung geöffnet und das neue Paket von dort installiert werden.

## Integrität prüfen

Nach dem Download kann die SHA-256-Prüfsumme in PowerShell verglichen werden:

```powershell
Get-FileHash .\SIP-Fehleranalyse-v1.6.4-Setup.exe -Algorithm SHA256
```

Der ausgegebene Hash muss mit dem entsprechenden Eintrag in `SHA256SUMS.txt` übereinstimmen.

Die veröffentlichte Anwendung enthält zusätzlich ein signiertes Integritätsmanifest und prüft ihre eigene Programmdatei beim Start.

## Windows-Sicherheitshinweis

Die Dateien sind derzeit nicht kommerziell code-signiert. Windows SmartScreen kann deshalb beim ersten Start vor einem unbekannten Herausgeber warnen. Dateien sollten ausschließlich aus diesem Release-Bereich geladen werden.

## Datenschutz

Dieses Repository enthält keinen Quellcode, keine Lizenzschlüssel, keine Lizenzgeneratoren, keine Testlizenzen, keine Zugangsdaten und keine Kundendaten.

© 2026 SIP-Fehleranalyse Projekt. Alle Rechte vorbehalten.
