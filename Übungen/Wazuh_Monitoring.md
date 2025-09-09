# monitoring_mit_wazuh

## 1.0 Installation

Hier ist eine kurze Anleitung zur Installation von Wazuh. 

### 1.1 Ablauf

Lade die Wazuh Datei herunter und füge sie danach in Virtualbox ein.

https://packages.wazuh.com/4.x/vm/wazuh-4.12.0.ova

- Folge Der anleitung Online

##### Hinweis:
Verbinde dich mit einem Hotspot nicht Schulnetzwerk. Dies verhindert dass du keine IP bekommst.


### 1.2 Agent installieren

- Gehe auf folgende Seite und folge der Anleitung:
 https://documentation.wazuh.com/current/installation-guide/wazuh-agent/index.html

 - Führe die Befehle in Powershell als Administrator aus

 Jetzt sollte es so auf deinem Wazuh Agent aussehen:
 ![alt text](image-2.png)

 ### 1.3 Massnahmen zur Hertung

 - In Wazuh
 ![alt text](image-3.png)

 Ich sehe, dass ich ein paar Packages noch nicht geupdated habe. Desshalb ist mein Hardening Schritt, dies nun zu tun. 

 --- 
 Meine Updates führe ich via Powershell aus:
Ausnahme: Docker, kann ich in der GUI aktualisieren.

Mit winget kann ich die Updates von Windows herunterladen und installieren.

```bash
winget ugrade Python.Python.3.12
winget upgrade 7zip.7zip
winget upgrade oracle.virtualbox
winget upgrade wireguard.wireguard
```
Danach sieht es so aus:
![alt text](image-4.png)

Bei WireGuard hat es erstaunlicherweise keine Updates gegeben. 

### Hardening

Zur Härtung des Systems habe ich in erster Linie alle installierten Pakete und Programme auf den neuesten Stand gebracht. Durch das Einspielen von Updates und Sicherheits-Patches wurden bekannte Schwachstellen geschlossen und die Angriffsfläche des Systems reduziert. Dies betraf sowohl das Betriebssystem als auch zusätzliche Anwendungen wie VirtualBox, Docker Desktop oder Hilfsprogramme wie 7-Zip.

---

### Fazit

Mein Fazit zu Wazuh ist, dass es ein hilfreiches Werkzeug für die Überwachung und Analyse von Endpunkten ist. Besonders nützlich war für mich die Funktion zur Erkennung von Schwachstellen, da ich dadurch sofort sehen konnte, welche Software-Versionen ein Sicherheitsrisiko darstellen. Gelernt habe ich vor allem, wie wichtig es ist, Systeme regelmäßig aktuell zu halten und wie Wazuh dabei unterstützt, diese Prozesse transparent zu machen. Auch wenn die Einrichtung der Agents anfangs etwas aufwendig war, zeigt das Tool sehr gut, wo Handlungsbedarf besteht und trägt damit direkt zur Härtung der Systeme bei.