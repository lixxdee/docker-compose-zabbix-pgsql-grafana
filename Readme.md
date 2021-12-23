After install, check ip network zabbix-server and zabbix agent, rebuild container if its need.
docker inspect zabbix-agent | grep "IPAddress\": "
docker stop '.....'
docker-compose up -d
