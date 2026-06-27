# Docker installieren
![Alternativer Text](images/docker.png)
## Installation

Docker installieren:

```bash
curl -fsSL https://get.docker.com | sh
```



## Docker-Dienst starten

Docker starten:

```bash
sudo systemctl start docker
```

Docker beim Systemstart automatisch aktivieren (empfohlen):

```bash
sudo systemctl enable docker
```



## Installation überprüfen

Prüfen, ob Docker korrekt installiert wurde:

```bash
docker --version
```



## Wichtige Docker Commands

### Container Verwaltung

<details>
<summary>Container anzeigen</summary>

```bash
docker ps
```

Alle Container anzeigen (auch gestoppte):

```bash
docker ps -a
```

</details>

<details>
<summary>Container starten / stoppen / restart</summary>

Container starten:

```bash
docker start <container-name>
```

Container stoppen:

```bash
docker stop <container-name>
```

Container neu starten:

```bash
docker restart <container-name>
```

</details>

<details>
<summary>Container Logs ansehen</summary>

```bash
docker logs -f <container-name>
```

</details>



### Images Verwaltung

<details>
<summary>Images anzeigen / löschen</summary>

Images anzeigen:

```bash
docker images
```

Image löschen:

```bash
docker rmi <image-name>
```

</details>



### System Cleanup

<details>
<summary>Aufräumen</summary>

Ungenutzte Ressourcen entfernen:

```bash
docker system prune
```

Alles inklusive unbenutzter Images entfernen:

```bash
docker system prune -a
```

</details>
