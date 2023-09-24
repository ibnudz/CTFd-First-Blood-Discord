# CTFd First Blood Discord

# ⚠️ Deprecation Notice ⚠️
I will no longer be maintaining this bot and I suggest you migrate to my Rust rewrite https://github.com/jordanbertasso/ctfd-solve-announcer-discord

---

This is a dockerised bot that uses Discords channel webhook feature to announce CTFd first bloods.

## Usage
1. [Create a Discord channel webhook](https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks) for the channel where you want the first bloods to be announced and copy the webhook link.

2. Create a CTFd API token in your user settings and copy that down.

3. Update `config.py` with the webhook link, CTFd API token and the API endpoint for your instance of CTFd.

4. Start with
    ```
    make run
    ```

You can customise the announcement template in `config.py` as well.

# Docker tutorial

## How to Stop All Docker Containers
    ```
    docker kill $(docker ps -q)
    ```
## How to Remove All Docker Containers
    ```
    docker rm $(docker ps -a -q)
    ```
## How To Remove All Docker Images
    ```
    docker rmi $(docker images -q)
    ```
