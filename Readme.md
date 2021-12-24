<code>git clone https://github.com/lixxdee/docker-compose-zabbix-pgsql-grafana.git</code>

<code>cd docker-compose-zabbix-pgsql-grafana</code>

<code>docker-compose up -d</code>

<code>docker ps -a</code> - make sure all containers are is running

<code>docker inspect zabbix-agent | grep "IPAddress\\": "</code> - result ip address you need change in web interface zabbix server.

<code>docker restart zabbix-agent</code> - restart zabbix-agent container

Enjoy! :)
