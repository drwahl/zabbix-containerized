# ansible-zabbix-containerized
An all-in-one zabbix server deployment using mysql backend and in docker containers.

Users can configure the deployment by providing the following variable(s) in all.yml:

```
zabbix:
    mysql_container_name: "zabbix_mysql"
    mysql_password: "changeitorcry"
    mysql_container_image: "mysql"
    mysql_container_image_tag: 5
    server_container_name: "zabbix_server"
    server_container_image: "zabbix/zabbix-server-mysql"
    server_container_image_tag: "ubuntu-3.4.11"
    web_container_image: "zabbix/zabbix-web-nginx-mysql"
    web_container_image_tag: "ubuntu-3.4.11"
    web_container_name: "zabbix_web"
    PHP_TZ: 'UTC'
```
