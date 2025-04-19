# SERVICE_NAME
**Container**: CONTAINER_NAME  
**Server**: WHICH_SERVER  
**Host Path**: `CONTAINER_PATH`

---

### [▶️](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)  Overview

[SERVICE_OFFICIAL_NAME](OFFICIAL_WEBSITE) SERVICE_DESCRIPTION

---

### [⚙️](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)  Docker Configuration

| Key          | Value                |
|--------------|----------------------|
| Dockerized?  | Yes (docker-compose) |
| Compose File | [`docker-compose.yml`](./docker-compose.yml) |
| Env File     | [`.env`](./.env) |
| Bind Mounts  | `./data` → `/data`  |

---

### [:globe_with_meridians:](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md) Docker Network

| Network  | IP Address  | Gateway  | MAC Address  |
|----------|-------------|----------|--------------|
| docker_network	| 172.23.0.2	| 172.23.0.1	| 00:00:00:00:00:00	 |

---

### [:key:](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)  Access

| Access Type     | Value / URL                             |
|------------------|------------------------------------------|
| Public Hostname  | [PUBLIC_HOSTNAME](https://PUBLIC_HOSTNAME) *(via [Cloudflare Tunnel](CLOUDFLARE_TUNNEL_URL))* |
| VPS IP:PORT         | [107.172.201.30:SERVICE_PORT](http://107.172.201.30:SERVICE_PORT) |
| Auth Required?   | Yes |
| Admin Username   | ADMIN_USERNAME |
| Password (1)     | ADMIN_PASSWORD |
| Username (1)     | USERNAME_1 |
| Password (1)     | PASSWORD_1 |
| Username (2)     | USERNAME_2 |
| Password (2)     | PASSWORD_2 |

---

### [☁️](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)  Cloudflare Tunnel

- **Tunnel Name**: `VPS`
- **Ingress Rule** (Caddy/Cloudflare config): N/A (_deferred_)

---

### [📎](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)  Notes & Customizations
- Any volumes, plugins, CLI overrides
- Any upgrade instructions
- App-specific tweaks

---

### [:books:](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)  References
- [Official Docs](DOCS_URL)
- [Github repo](OFFICIAL_GITHUB_URL)
- [Support URL](SUPPORT_URL)
- [Reddit](REDDIT_URL)
- [Google Search](https://www.google.com/search?q=GOOGLE_SEARCH_TERM)
- [Dokuwiki link](https://labdocs.donferris.me/DOKUWIKI_PAGE_NAME)
- [other links](https://example.com)

---

### [💾](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)  Backup & Restore

#### Backup
- Backup archives stored in BACKUP/
- To create a new backup:
```bash
tar -czf BACKUP/SERVICE_NAME-$(date +'%Y-%m-%d').tar.gz ./data
```
- Commit & push to GitHub to version it
```bash
git add . && git commit -m "Backup on $(date +'%Y-%m-%d') " && git push
```
#### Restore
1.	Clone the repo
2.	Extract the desired archive to ./data:
```bash	
tar -xzf BACKUP/SERVICE_NAME-[backup_date].tar.gz -C ./data
```
3. Recreate the container:
```bash
docker compose up -d
```

---

## [🛠️](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)  Useful Commands
### Docker
#### Start Docker container
```bash
docker compose up -d
```
#### View Docker logs
```bash
docker compose logs -f
```
#### Open shell inside Docker container
```bash
docker exec -it CONTAINER_NAME /bin/Backup on $(date +'%Y-%m-%d')sh
```
### Git
#### Git - Stage + Commit + Push Changes
```bash
git add . && git commit -m "Tweaks/Minor refinements - $(date +'%Y-%m-%d')" && git push
``` 
#### Git - View Current Status
```bash
git status
```
#### Git - Pull Latest Changes
```bash
git pull
```
#### Git - View Commit History (compact)
```bash
git log --oneline --graph --decorate --all
```
#### Git - Revert the Most Recent Commit (preserve changes)
```bash
git reset --soft HEAD~1
```
#### Git - Force Pull GitHub to Local— Overwrite Local
```bash
git fetch origin && git reset --hard origin/main
```
#### Git - Force Push Local to GitHub — Overwrite Remote
```bash
git push origin main --force
```
#### Git - Initial Repo Setup (one-time)
```bash
git init && \
git remote add origin git@github.com:don-ferris/repo_name.git && \
git add . && git commit -m "Initial commit" && \
git push -u origin main
```
