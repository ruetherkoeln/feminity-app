# Feminity Oberkassel — App-Prototyp

Single-Page React/Tailwind-Prototyp, ausgeliefert via nginx in Docker.

## Lokal starten

```bash
docker compose up -d --build
```

Aufruf: http://localhost:8080

Stoppen: `docker compose down`

## In GitHub Codespaces starten

1. Auf GitHub: **Code → Codespaces → Create codespace on main**
2. Codespace startet den Container automatisch (`postCreateCommand`)
3. Port 8080 wird automatisch weitergeleitet — Browser öffnet sich

## Dateien

- `index.html` — App-Prototyp (React + Tailwind via CDN)
- `Dockerfile` — nginx:alpine, served auf Port 80
- `nginx.conf` — SPA-Routing + Cache-Header
- `docker-compose.yml` — Port-Mapping 8080:80
- `.devcontainer/devcontainer.json` — Codespaces-Konfiguration
