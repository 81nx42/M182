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




### Aufgabe 3: Diskussion und Bewertung

Beantworten Sie die folgenden Fragen schriftlich:

##### Bei welchem System sehen Sie den grössten Handlungsbedarf? Begründen Sie Ihre Einschätzung.

Ich sehe den grössten Handlungsbedarf beim Notebook. Dies hat viele Gründe. Zum einen ist das verlieren eines Notebooks nicht unüblich und kann durchaus vorkommen. Auch konzentrieren sich Hacker oftmals auf die Mitarbeiter zu erst, was heisst dass bei einem geplanten Angriff dies die einfachste und zugleich Fatalste Lücke ist. 

Das Heisst, das schwächste glied in der Sicherheitskette ist und bleibt der Mensch. 


##### Wie verändert sich die Risikobewertung, wenn eine Schwachstelle vollständig behoben wird, die Bedrohung jedoch weiterhin besteht?

Wenn eine Schwachstelle vollständig behoben wird, sinkt die Eintrittswahrscheinlichkeit deutlich, weil Angreifer den bekannten Angriffsweg nicht mehr ausnutzen können. Jedoch bleibt die Bedrohung selbst bestehen, nun richtet sich diese Schwachstelle aber in einen leeren Angriffspfad.

Das heisst bei der Risikobewertung verschiebt sich dieser Fall von hoch/kritisch auf niedrig oder mittel, abhängig davon, wie gut die Schwachstelle geschlossen wurde. Ein restrisiko bleibt bestehen, aber die Eintrittswahrscheinlichkeit ist deutlich reduziert. 


##### Warum ist es wichtig, nicht nur technische, sondern auch organisatorische Massnahmen (z. B. Schulungen, Prozesse) zu berücksichtigen?

Diese Massnahmen sind Präventiv. Sie helfen uns nicht-IT affine Mitarbeiter die Risiken zu identifizieren und reduzieren. Ohne solche schulungen fallen Fishing-Mails zum beispiel, deutlich schlimmer aus und bilben eine Angriffsfläche, die verhindert werden hätte können. Wie oben bereits erwähnt, der mensch ist der schwächste glied in der Sicherheitskette. 
