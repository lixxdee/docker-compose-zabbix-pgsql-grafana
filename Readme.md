git clone https://github.com/lixxdee/docker-compose-zabbix-pgsql-grafana.git

cd docker-compose-zabbix-pgsql-grafana

docker-compose up -d

docker ps -a

<code>docker inspect zabbix-agent | grep "IPAddress\\": " // this is ip adress you need change in web interface zabbix server.

docker inspect zabbix-server | grep "IPAddress\\": " // check network and edit in docker-compose.yml file ip adress ZBX_SERVER_HOST if its need.

docker stop/start <your containers>
  
docker-compose up -d // build or rebuild docker-compose.yml
