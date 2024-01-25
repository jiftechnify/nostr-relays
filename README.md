# Nostr relays operated by jiftechnify

## Memo: How to Deploy Relays

1. clone repo

    ```bash
    git clone git@github.com:jiftechnify/nostr-relays.git --recursive
    ```

1. create Docker network

    ```bash
    docker network create nostr_relays
    ```

1. build nozokimado for shiritori relay

    ```bash
    cd shiritori
    npm run build
    ```

1. deploy Yomi API server (for shiritori relay) to somewhere
1. fill .env files: `.env` and `shiritori/.env`
1. start up containers!

    ```bash
    docker compose up -d
    ```