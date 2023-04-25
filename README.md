# How to start project
1. Add folders for prometheus and grafana:
```bash
mkdir grafana_data
mkdir prometheus_data
```
2. Change them owners:
```bash
sudo chown -R 1001:1001 grafana_data
sudo chown -R 1001:1001 prometheus_data
```
3. Set your own coinmarketcap key (and don't forget to add him to .gitignore) in all-cmc-up-compose.yml at `CMC_API_KEY`

4. `docker-compose -f all-cmc-up-compose.yml up`
