# Docker
docker pull influxdb


#grafana
sudo add-apt-repository "deb https://packages.grafana.com/oss/deb beta main"
curl https://packages.grafana.com/gpg.key | sudo apt-key add -
sudo apt-get update
sudo apt-get -y install grafana
sudo systemctl start grafana-server
sudo systemctl enable grafana-server
sudo ufw allow proto tcp from any to any port 3000
