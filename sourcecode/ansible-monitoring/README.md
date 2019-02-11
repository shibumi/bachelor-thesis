README
======

Um drei virtuelle Maschinen als Testumgebung zu starten wird das
Werkzeug `Vagrant` benötigt. Das Werkzeug ist herunterladbar über
folgende Webseite:

`https://www.vagrantup.com/`

Unterstützte Betriebssysteme sind Windows, Mac OS X und Linux.
Um die drei virtuellen Maschinen zu starten ist es nur nötig, dass in
das Verzeichnis `ansible-monitoring` gewechselt wird. Danach können die
drei virtuellen Maschinen mit dem folgenden Kommando gestartet werden:

`vagrant up`

Auf die einzelnen Maschinen kann via SSH zugegriffen werden über das
Kommando `vagrant ssh <hostname>`. Ein Beispiel dafür ist:

`vagrant ssh puppetmaster`

Sind die drei virtuellen Maschinen gestartet ist es möglich, dass
Ansible Deployment vorzunehmen. Für das Ansible Deployment muss Ansible
installiert sein. Ansible steht aktuell nur auf Linux und Mac OS X zur
Verfügung. Es gibt jedoch den Weg Ansible über Windows 10 und "Windows
Subsystem for Linux" zu benutzen. Eine Dokumentation welche die
Installation auf Linux erklärt ist hier zu finden:

`https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html`

Eine Installation von Ansible auf Linux via Windows Subsystem for Linux
ist in diesem Blogartikel erklärt:

`https://www.jeffgeerling.com/blog/2017/using-ansible-through-windows-10s-subsystem-linux`

Ist Ansible installiert kann das Deployment über das folgende Kommando
gestartet werden. Es ist wichtig, dass man sich mit der Kommandozeile in
dem Verzeichnis `ansible-monitoring` befindet:

`ansible-playbook playbooks/monitoring.yml`
