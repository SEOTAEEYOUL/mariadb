# mariadb
<pre>
[PhpMyAdmin]
Environment variables summary
  PMA_ARBITRARY - when set to 1 connection to the arbitrary server will be allowed
  PMA_HOST - define address/host name of the MySQL server
  PMA_VERBOSE - define verbose name of the MySQL server
  PMA_PORT - define port of the MySQL server
  PMA_HOSTS - define comma separated list of address/host names of the MySQL servers
  PMA_VERBOSES - define comma separated list of verbose names of the MySQL servers
  PMA_PORTS - define comma separated list of ports of the MySQL servers
  PMA_USER and PMA_PASSWORD - define username to use for config authentication method
  PMA_ABSOLUTE_URI - define user-facing URI
For more detailed documentation see https://docs.phpmyadmin.net/en/latest/setup.html#installing-using-docker
Please report any issues with the Docker container to https://github.com/phpmyadmin/docker/issues
[MariaDB]

[DEPLOY]
kubectl -f mariadb-data-pvc.yaml
kubectl -f mariadb-pass.yaml
kubectl -f mariadb-deploy.yaml
kubectl -f mariadb-svc.yaml
kubectl -f phpmyadmin-deploy.yaml
kubectl -f phpmyadmin-svc.yaml 

[Grafana Dashboard]
mariadb_dashboard.json
</pre>
