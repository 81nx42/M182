# Risikoanalyse


## Ausgangslage

Sie arbeiten als IT-Sicherheitsbeauftragte bzw. -beauftragter in einem mittelständischen Unternehmen mit rund 50 Mitarbeitenden. Das Unternehmen betreibt verschiedene IT-Systeme, unter anderem zur Kundenkommunikation, zur Datenverarbeitung sowie für den Betrieb eines Onlineshops. Ihre Aufgabe ist es, eine qualitative Risikoanalyse für ausgewählte Systeme durchzuführen und daraus geeignete Massnahmen abzuleiten.


### Aufgabe 1: Risikoanalyse für drei Systeme

Analysieren Sie für jedes der folgenden Systeme potenzielle Risiken. Füllen Sie dazu die folgende Tabelle aus:

#### Systeme zur Analyse



- Webserver (öffentlich zugänglich, betreibt den Onlineshop)

- Datenbankserver (intern, enthält sensible Kundendaten)

- Notebook eines Support-Mitarbeitenden (mobil im Einsatz, mit VPN-Zugang ins interne Netz)

| System | Bedrohung | Schwachstelle | Eintrittswahrscheinlichkeit (selten / gelegentlich / häufig) | Schweregrad bei Eintritt (gering / mittel / hoch / kritisch) | Betroffene Schutzziele (C / I / A) | Risikobewertung (niedrig / mittel / hoch / kritisch) |
| ------ | --------- | ------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---------------------------------- | ---------------------------------------------------- |
| Webserver (Onlineshop) | Sicherheitslücken für angriffe wie: SQL-Injection oder DDoS | Alte Software-Versionen kein Patch-Management | häufig | kritisch | C, I, A | kritisch |
| Datenbankserver (Kundendaten) | Datenextraktion durch internen oder externen Angreifer | Schlechte Verschlüsselung, Falsch Konfigurierte Zugriffsrechte, unsichere Passwörter | gelegentlich | hoch | C, I | hoch |
| Notebook (Support-Mitarbeiter, mobil) | Verlust oder Diebstahl heisst: unbefugter Zugriff ins Unternehmensnetz | Keine Festplattenverschlüsselung, schwache Passwortrichtlinien | gelegentlich | hoch | C, I, A | hoch |

### Aufgabe 2: Massnahmendefinition

Für zwei Risiken mit hoher oder kritischer Bewertung sollen Sie jeweils geeignete Massnahmen vorschlagen, um das Risiko zu reduzieren. Tragen Sie diese in folgende Tabelle ein:

| System | Identifiziertes Risiko | Schutzmassnahme | Erwartete Wirkung |
| ------ | ---------------------- | --------------- | ----------------- |
| Webserver (Onlineshop) | SQL-Injection, DDoS | - Regelmässige Patch Windows  und Updates<br>- Web Application Firewall (WAF)<br>- Penetrationstests durchführen (Evtl von Externen Testern) | Reduziert Eintrittswahrscheinlichkeit durch Patches und Schweregrad mit dem Pentesting zum Vorbäugen |
| Notebook (Support-Mitarbeiter) | Verlust oder Diebstahl gibt unbefugter Zugriff and dritt Personen | - Vollständige Festplattenverschlüsselung wie BitLocker <br>- Multi-Faktor-Authentifizierung für VPN<br>- Mobile Device Management (Remote-Löschung) | Reduziert Schweregrad gestohlene Geräte enthalten nun keine nutzbaren Daten und Eintrittswahrscheinlichkeit mit MFA erschwert Zugriff|


