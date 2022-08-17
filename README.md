# Steps

Repo assumes use of Grafana cloud

- Run tlsCreate script
- Create web auth pws for node exporter and prometheus
- edit .env file
- run docker compose

## Create web auth pws for node exporter and prometheus
```
sudo apt install apache2-utils
```
Run 2x
```
htpasswd -nBC 10 "" | tr -d ':\n'
```
Save, and be prepared to add to .env
