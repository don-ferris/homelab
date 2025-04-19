# SERVICE_NAME

**Container**: container_name  
**Server**: vps_or_local_server  
**Host Path**: `/path/to/container_dir`

---

## [▶️](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md?utm_source=chatgpt.com)  Overview

[Link_to_official_website](https://website_url) Description_of_service

---

## [⚙️](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md?utm_source=chatgpt.com)  Docker Configuration

| Key          | Value                |
|--------------|----------------------|
| Dockerized?  | Yes (docker-compose) |
| Compose File | [`docker-compose.yml`](./docker-compose.yml) |
| Env File     | [`.env`](./.env) |
| Bind Mounts  | `./data` → `/data`  |

## [:globe_with_meridians:](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md?utm_source=chatgpt.com) Docker Network

| Network  | IP Address  | Gateway  | MAC Address  |
|----------|-------------|----------|--------------|
| docker_network	| 172.23.0.2	| 172.23.0.1	| 00:00:00:00:00:00	 |

---

## [:key:](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md?utm_source=chatgpt.com)  Access

| Access Type     | Value / URL                             |
|------------------|------------------------------------------|
| Public Hostname  | [servicename.tikishack.com](https://servicename.tikishack.com) *(via [Cloudflare Tunnel](https://one.dash.cloudflare.com/0889c842407ffe50bd89d900e389f5b7/networks/tunnels/7f2310e1-5350-4ab6-9c94-bb92159f1851/public-hostname/budget.tikishack.com/1))* |
| VPS IP:PORT         | [107.172.201.30:12345](http://107.172.201.30:12345) |
| Auth Required?   | Yes |
| Username         | N/A |
| Password         | ChangeMe98765 |

---

## [☁️](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md?utm_source=chatgpt.com)  Cloudflare Tunnel

- **Tunnel Name**: `VPS`
- **Ingress Rule** (Caddy/Cloudflare config): N/A (_deferred_)

---

## [📎](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md?utm_source=chatgpt.com)  Notes & Customizations
- Any volumes, plugins, CLI overrides
- Any upgrade instructions
- App-specific tweaks

---

## [:books:](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md?utm_source=chatgpt.com)  References
- [Official Docs](https://docs.servicename.com
- [Github repo](https://github.com/service_dev/repo_name)
- [Support forum](https://community.example.com)
- [Reddit](https://www.reddit.com/r/subreddit)
- [Google Search](https://www.google.com/search?q=search_term)
- [Dokuwiki link](https://labdocs.donferris.me/service_name)
- [other links](https://example.com)

---

## [💾](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md?utm_source=chatgpt.com)  Backup & Restore

### Backup
- Backup archives stored in BACKUP/
- To create a new backup:
```bash
tar -czf BACKUP/actual-$(date +'%Y-%m-%d').tar.gz ./data
```
- Commit & push to GitHub to version it
```bash
git add . && git commit -m "Backup on $(date +'%Y-%m-%d') " && git push
```
### Restore
1.	Clone the repo
2.	Extract the desired archive to ./data:
```bash
tar -xzf BACKUP/actual-2025-04-18.tar.gz -C ./data
```
3. Recreate the container:
```bash
docker compose up -d
```

---

## [🛠️](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md?utm_source=chatgpt.com)  Useful Commands
### Start Docker container
```bash
docker compose up -d
```
### View Docker logs
```bash
docker compose logs -f
```
### Open shell inside Docker container
```bash
docker exec -it actual /bin/Backup on $(date +'%Y-%m-%d')sh
```
### Git - Stage + Commit + Push Changes
```bash
git add . && git commit -m "Update on $(date +'%Y-%m-%d')" && git push
``` 
### Git - View Current Status
```bash
git status
```
### Git - Pull Latest Changes
```bash
git pull
```
### Git - View Commit History (compact)
```bash
git log --oneline --graph --decorate --all
```
### Git - Revert the Most Recent Commit (preserve changes)
```bash
git reset --soft HEAD~1
```
### Git - Force Pull GitHub to Local— Overwrite Local
```bash
git fetch origin && git reset --hard origin/main
```
### Git - Force Push Local to GitHub — Overwrite Remote
```bash
git push origin main --force
```
### Git - Initial Repo Setup (one-time)
```bash
git init && \
git remote add origin git@github.com:don-ferris/repo_name.git && \
git add . && git commit -m "Initial commit" && \
git push -u origin main
```
