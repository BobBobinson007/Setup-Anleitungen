# Memos installieren
![](images/memos.png)
## Voraussetzungen

Prüfe zunächst, ob Docker installiert ist:

```bash
docker --version
```

Falls Docker noch nicht installiert ist, folge zuerst [Docker installieren](docker.md) und fahre anschließend mit dieser Anleitung fort.

## Memos starten

Container starten:

```bash
docker run -d \
  --name memos \
  -p 5230:5230 \
  -v ~/.memos:/var/opt/memos \
  neosmemo/memos:stable
```

Prüfen, ob der Container läuft:

```bash
docker ps
```

## Ersteinrichtung

Memos im Browser öffnen:

```text
http://<SERVER-IP>:5230
```

Den Anweisungen auf der Website folgen.

---

## Daten

Alle Daten werden dauerhaft unter folgendem Verzeichnis gespeichert:

```text
~/.memos
```
