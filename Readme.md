<code>git clone https://github.com/lixxdee/docker-compose-zabbix-pgsql-grafana.git</code> - download project.

<code>cd docker-compose-zabbix-pgsql-grafana</code> - go to directory with docker-compose.yml file.

<code>docker-compose up -d</code> - build containers.

<code>docker ps -a</code> - make sure all containers are is running.

<code>docker inspect zabbix-agent | grep "IPAddress\\": "</code> - received ip address you need change in web interface zabbix instead of '127.0.0.1'.

<code>docker restart zabbix-agent</code> - restart zabbix-agent container.

Grafana will be available by http://YourIP:3000/, default login:admin, password:admin.

Enjoy! :)
