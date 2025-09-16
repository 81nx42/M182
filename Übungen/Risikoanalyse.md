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
| Webserver (Onlineshop) | Hackerangriff über Sicherheitslücken (z. B. SQL-Injection, DDoS) | Veraltete Software-Versionen, fehlendes Patch-Management | häufig | kritisch | C, I, A | kritisch |
| Datenbankserver (Kundendaten) | Datendiebstahl durch internen oder externen Angreifer | Fehlende Verschlüsselung, schwache Zugriffsrechte, unsichere Passwörter | gelegentlich | hoch | C, I | hoch |
| Notebook (Support-Mitarbeiter, mobil) | Verlust oder Diebstahl → unbefugter Zugriff ins Unternehmensnetz | Keine Festplattenverschlüsselung, fehlendes MDM, schwache Passwortrichtlinien | gelegentlich | hoch | C, I, A | hoch |
