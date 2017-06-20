# Hands-On Ansible und Docker

Dieses Repository enthält den Inhalt eines 3-tägigen Workshops über das Provisionierungstools Ansible und Docker. Ziel ist es zu zeigen, wie wir Ansible nutzen können um sowohl VM- als auch Container-Architekturen zu verwalten. Der Fokus in diesem Workshop liegt auf dem Hands-On. Wissen prägt sich am effektivsten ein, wenn es angewendet wird. Daher beschränken sich die Folien auf ein absolutes Minimum und werden durch Live-Nutzung der Tools mit Leben gefüllt. Am Ende jedes Abschnitts sollen die Teilnehmer dann das vorgestellte direkt praktisch anwenden.

Im ersten Teil werden wir die Basics zu Ansible kennenlernen und Ad-Hoc erste Tasks anwenden. Sobald die Verbindung zu den Remote Maschinen steht, werden wir ein Durchgängiges Anwendungsbeispiel verwenden:

- Bootstrapping neuer Instanzen
- Apache2 Webserver installieren und konfigurieren

In der heutigen Welt ist alles hochverfügbar. Wir werden das Anwendungsbeispiel dahingehend ausbauen:

- Apache2 hinter Loadbalancer
- Rolling updates

Und dann kommen noch Container ins Spiel. Wir werden die Vorteile von Docker motivieren und das Zusammenspiel mit Ansible zeigen. Ziel ist es Docker zu nutzen, um erneut einen Apache2 aufzusetzen. Zudem wollen wir keycloak als Authentifizierungsdienst einbauen und das Apache modul mod_auth_openidc nutzen. Anhand dieses komplexen Beispiels werden wir docker compose vorstellen.

Um zu zeigen, wie Ansible und Docker zusammenspielen werden wir:

- den Docker Host mit Ansible installieren und konfigurieren
- Container mit Ansible orchestrieren
- Ansible-Container nutzen

Abschließend werden wir besprechen, wie wir die erstellten Skripte in einer CI Umgebung nutzen können und gehen kurz auf Best-Practices im Bezug auf sensible Daten ein.

## Tag 1
* **[G]** Vorstellung [Persönliche Vorstellung, Kenntnisse, Erwartungen]
* **[V]** Roadmap
* **[V]** Ansible Grundlagen
* **[P]** PONG?
* **[V]** Ansible Playbooks
* **[P]** Bootstrap
* **[V]** Ansible Rollenkonzept
* **[P]** Apache2
* **[V]** Ansible Variablen
* **[P]** Apache2 && Keycloak
* **[G]** Retro

## Tag 2
* **[V]** Ansible Orchestrierung
* **[P]** HAProxy && Updates
* **[V]** Ansible Zusammenfassung
* **[V]** Docker Grundlagen
* **[P]** Ansible Docker Host
* **[P]** Erster Container
* **[V]** Docker Compose
* **[P]** Einmal alles, bitte
* **[G]** Retro

## Tag 3
* **[V]** Ansible Docker
* **[P]** Container Orchestrierung
* **[V]** Ansible Container
* **[P]** Container && VMs 
* **[V]** Automatisierung
* **[P]** Jenkins
* **[V]** Sicherheit
* **[P]** Ansible Vault
* **[G]** Retro

ToDo:
* Jump-Host / Proxy?
* https://github.com/ansible/ansible-container
* https://linuxacademy.com/howtoguides/posts/show/topic/13750-managing-docker-containers-with-ansible
* https://www.ansible.com/blog/six-ways-ansible-makes-docker-compose-better
* Return values
* Pipelining?
* https://github.com/geerlingguy/ansible-role-haproxy
* Handlers (in V Playbooks)
* http://docs.ansible.com/ansible-container/ Container - Alternative zu Docker Compose
* Variablen : Group by?
