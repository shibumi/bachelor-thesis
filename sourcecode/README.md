README
======

Dieses Verzeichnis enthält die folgenden Dateien und
Unterverzeichnisse:

* ansible-monitoring
* dashboard.json
* procfs
* ssh.config

Das Verzeichnis `ansible-monitoring` beinhaltet alle Dateien um drei
virtuelle Maschinen via dem Werkzeug `Vagrant` zu starten und diese mit
Ansible zu konfigurieren.

Die Datei `dashboard.json` enthält das von mir gebaute Dashboard für
Grafana zur Anzeige aller nötigen Informationen. Das Dashboard ist auch
unter folgendem Link abrufbar: `https://grafana.com/dashboards/9719`

Das Verzeichnis `procfs` enthält die Prometheus Node Exporter Komponente
`procfs` mit den von mir hinzugefügten Dateien, für CIFS Support.

Die Datei `ssh.config` enthält eine Beispiel
OpenSSH-Client-Konfiguration mit welcher es möglich ist zu den
virtuellen Maschinen zu verbinden. Die Datei ist auf Linux
ausgelegt.
