# BigBoss Playlist Auto Updater

The GitHub Action downloads the configured source playlist and creates/updates
`bigboss.m3u` with only entries whose `#EXTINF` line contains `BigBoss`.

## GitHub Secrets

Repository → Settings → Secrets and variables → Actions → New repository secret

Add:

- `PLAYLIST_URL` = source playlist URL
- `PLAYLIST_USER_AGENT` = required User-Agent

The source URL and User-Agent are kept out of the repository.

The workflow runs every 30 minutes and can also be started manually from
Actions → Update BigBoss Playlist → Run workflow.
