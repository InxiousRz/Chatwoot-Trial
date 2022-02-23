## How To Deploy.

Prepare Docker Compose

```text codeBlock_jd64 thin-scrollbar
docker-compose run --rm rails bundle exec rails db:chatwoot_prepare
```

Get the service up and running.

```text codeBlock_jd64 thin-scrollbar
docker-compose up -d
```

Your Chatwoot installation is complete. Please note that the containers are not exposed to the internet and they only bind to the localhost. Setup something like Nginx or any other proxy server to proxy the requests to the container.
