# zsh-history-cleaner

A small zsh script to securely wipe bash and zsh history in one shot.

## Requirements

Install toilet before running the script:
```bash
sudo apt install toilet
```
## Usage

1. Download the script:
```
curl -O https://raw.githubusercontent.com/mynameisnobody211/zsh-history-cleaner/main/history_delete.sh
```
2. Make it executable:
```
chmod +x history_delete.sh
```
3. Run it with source:
```
source history_delete.sh
```
## Important

Use **ONLY** source to run this script.
Do NOT use `./` or `bash` — they create a separate subshell that cannot access the current session history, so the cleanup won't work properly.

With `source` the script runs inside the current shell and clears everything correctly.

