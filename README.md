# Steps

Repo assumes use of Grafana cloud

- Run tls script
- Create web auth pws for node exporter and prometheus

## Create web auth pws for node exporter and prometheus

Run 2x
```
htpasswd -nBC 10 "" | tr -d ':\n'
```
Save, and be prepared to add to web.yml and prometheusweb.yml

