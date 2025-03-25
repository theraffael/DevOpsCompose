# DevOpsCompose

```console

PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker pull mediawiki:1.42.3
1.42.3: Pulling from library/mediawiki
bc0965b23a04: Pulling fs layer
a56d4dc94542: Pulling fs layer
e77051345783: Pulling fs layer
15d92b0225a7: Pulling fs layer                                                                                                                                                                        
f059e1da2c1e: Pulling fs layer                                                                                                                                                                        
6821f8f24c9f: Pulling fs layer                                                                                                                                                                        
216ccc352f53: Pulling fs layer                                                                                                                                                                        
0baa94707405: Pulling fs layer                                                                                                                                                                        
ecea461af7af: Pulling fs layer                                                                                                                                                                        
83dc701d2fac: Pulling fs layer                                                                                                                                                                        
812968a297fd: Pulling fs layer                                                                                                                                                                        
27889ed59626: Pulling fs layer                                                                                                                                                                        
72b8e148074e: Pulling fs layer                                                                                                                                                                        
4f4fb700ef54: Pulling fs layer                                                                                                                                                                        
5e237fa8adfd: Pulling fs layer                                                                                                                                                                        
7dd89652abcc: Pulling fs layer                                                                                                                                                                        
bc0965b23a04: Pull complete
a56d4dc94542: Pull complete
e77051345783: Pull complete
15d92b0225a7: Pull complete
f059e1da2c1e: Pull complete
6821f8f24c9f: Pull complete
216ccc352f53: Pull complete
0baa94707405: Pull complete
ecea461af7af: Pull complete
83dc701d2fac: Pull complete
812968a297fd: Pull complete
27889ed59626: Pull complete
72b8e148074e: Pull complete
4f4fb700ef54: Pull complete
5e237fa8adfd: Pull complete
7dd89652abcc: Pull complete
e3e9a55ef041: Pull complete
6984861c786d: Pull complete
8e91f3c91f28: Pull complete
377cbcba9703: Pull complete
88fb7727753d: Pull complete
Digest: sha256:e8d020d41b6f5bf516875f1e4142ab17e25f56ddd5cd812183fef8acd885143b   
Status: Downloaded newer image for mediawiki:1.42.3
docker.io/library/mediawiki:1.42.3

What's next:
    View a summary of image vulnerabilities and recommendations → docker scout quickview mediawiki:1.42.3
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker run --name some-mediawiki -p 8081:80 -v -d mediawiki:1.42.3
AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
[Tue Mar 25 13:23:21.363247 2025] [mpm_prefork:notice] [pid 1:tid 1] AH00163: Apache/2.4.62 (Debian) PHP/8.1.31 configured -- resuming normal operations
[Tue Mar 25 13:23:21.363307 2025] [core:notice] [pid 1:tid 1] AH00094: Command line: 'apache2 -D FOREGROUND'
172.17.0.1 - - [25/Mar/2025:13:24:13 +0000] "GET / HTTP/1.1" 200 911 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
172.17.0.1 - - [25/Mar/2025:13:24:13 +0000] "GET /resources/assets/mediawiki.png HTTP/1.1" 200 13829 "http://localhost:8081/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"       
172.17.0.1 - - [25/Mar/2025:13:24:14 +0000] "GET /favicon.ico HTTP/1.1" 200 835 "http://localhost:8081/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
172.17.0.1 - - [25/Mar/2025:13:24:18 +0000] "GET /mw-config/index.php HTTP/1.1" 200 10577 "http://localhost:8081/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
172.17.0.1 - - [25/Mar/2025:13:24:18 +0000] "GET /resources/lib/codex/codex.style.css HTTP/1.1" 200 10268 "http://localhost:8081/mw-config/index.php" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
172.17.0.1 - - [25/Mar/2025:13:24:18 +0000] "GET /mw-config/config.js HTTP/1.1" 200 3111 "http://localhost:8081/mw-config/index.php" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
172.17.0.1 - - [25/Mar/2025:13:24:18 +0000] "GET /resources/lib/jquery/jquery.js HTTP/1.1" 200 84435 "http://localhost:8081/mw-config/index.php" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
172.17.0.1 - - [25/Mar/2025:13:24:18 +0000] "GET /mw-config/index.php?css=1 HTTP/1.1" 200 1784 "http://localhost:8081/mw-config/index.php" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
172.17.0.1 - - [25/Mar/2025:13:24:18 +0000] "GET /mw-config/images/installer-logo.png?62486 HTTP/1.1" 200 16735 "http://localhost:8081/mw-config/index.php?css=1" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
172.17.0.1 - - [25/Mar/2025:13:24:19 +0000] "GET /favicon.ico HTTP/1.1" 200 854 "http://localhost:8081/mw-config/index.php" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
[Tue Mar 25 13:24:28.029099 2025] [mpm_prefork:notice] [pid 1:tid 1] AH00170: caught SIGWINCH, shutting down gracefully
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker run --name some-mediawiki -p 8081:80 -v mediawiki:/var/www/html -d mediawiki:1.42.3
docker: Error response from daemon: Conflict. The container name "/some-mediawiki" is already in use by container "fa79876c9467d7763f72c31f07cf009aa40df841c8a35a9649c683e6c66e44fd". You have to remove (or rename) that container to be able to reuse that name.
See 'docker run --help'.
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker run --name some-mediawiki -p 8081:80 -v mediawiki:/var/www/html -d mediawiki:1.42.3        
9df0c3d9214fd7c8d174b526d81749da4bc28d067ea1612538df5dfe1019356f
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker run --name local-mysql -e MYSQL_ROOT_PASSWORD=12345 -e MYSQL_DATABASE=wordpress -e MYSQL_USER=wordpress -e MYSQL_PASSWORD=wordpress -v mysql-data:/var/lib/mysql -d mysql:9.1.0
Unable to find image 'mysql:9.1.0' locally
9.1.0: Pulling from library/mysql
2c0a233485c3: Pull complete
cb5a6a8519b2: Pull complete
570d30cf82c5: Pull complete
a841bff36f3c: Pull complete
80ba30c57782: Pull complete
5e49e1f26961: Pull complete
ced670fc7f1c: Pull complete
0b9dc7ad7f03: Pull complete
cd0d5df9937b: Pull complete
1f87d67b89c6: Pull complete
Digest: sha256:0255b469f0135a0236d672d60e3154ae2f4538b146744966d96440318cc822c6
Status: Downloaded newer image for mysql:9.1.0
fd4cfc11d71107e6c3d959c148b327499d0e5d6a6b7227c87532203a31db612a
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker run --name local-wordpress -p 8082:80 -v wordpress-data:/var/www/html -d wordpress:6.7.0-php8.3
Unable to find image 'wordpress:6.7.0-php8.3' locally
6.7.0-php8.3: Pulling from library/wordpress
2d429b9e73a6: Pull complete
7d111fc47c43: Pull complete
193b424feb9d: Pull complete
0217fa02fd5f: Pull complete
119202f2b319: Pull complete
e41950bab19c: Pull complete
0941d9a564d8: Pull complete
c3b04b7031fb: Pull complete
7bd375cf222d: Pull complete
566d672bde14: Pull complete
4f4fb700ef54: Pull complete
5fa7a68b53ce: Pull complete
0c6f25e4a7f1: Pull complete
e437f813648f: Pull complete
59e8ebe8db40: Pull complete
bacd944e309b: Pull complete
5af5555375ad: Pull complete
790e4644a44f: Pull complete
17cfd6d1aa5e: Pull complete
Digest: sha256:427f0fafc99907a32cf10481c444d67c32d400ed568088f84f8053d8a6231aa1
Status: Downloaded newer image for wordpress:6.7.0-php8.3
98cec29cce48cd3c89116ae15f833f92894e9808aaf866ca9147ad546c54f5da
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker network create --attachable wordpress-network
c470a9adae7276c00b8cc5743ce5b98ab1b3c6e85cc484aa729fce8cd16faffe
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker network connect wordpress-network local-mysql
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker network connect wordpress-network local-wordpress
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker compose up
no configuration file provided: not found
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> docker-compose up
no configuration file provided: not found
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose> cd docker-compose
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose\docker-compose> cd docker-compose
cd : Cannot find path 'C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose\docker-compose\docker-compose' because it does not exist.
At line:1 char:1
+ cd docker-compose
+ ~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (C:\Users\raffa\...\docker-compose:String) [Set-Location], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Commands.SetLocationCommand

PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose\docker-compose> docker compose up
[+] Running 5/5
 ✔ Network docker-compose_default          Created                                                                                                                                               0.2s 
 ✔ Volume "docker-compose_mysql-data"      Created                                                                                                                                               0.0s 
 ✔ Volume "docker-compose_wordpress-data"  Created                                                                                                                                               0.0s 
 ✔ Container docker-compose-db-1           Created                                                                                                                                               0.1s 
 ✔ Container docker-compose-wordpress-1    Created                                                                                                                                               0.1s 
Attaching to db-1, wordpress-1
db-1         | 2025-03-25 13:36:30+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 9.1.0-1.el9 started.
db-1         | 2025-03-25 13:36:30+00:00 [Note] [Entrypoint]: Switching to dedicated user 'mysql'
db-1         | 2025-03-25 13:36:30+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 9.1.0-1.el9 started.
Gracefully stopping... (press Ctrl+C again to force)                                                                                                                                                  
[+] Stopping 1/2
 ✔ Container docker-compose-wordpress-1  Stopped                                                                                                                                                 0.0s 
 - Container docker-compose-db-1         Stopping                                                                                                                                                0.1s 
Error response from daemon: driver failed programming external connectivity on endpoint docker-compose-wordpress-1 (0adeae0034c27a1b45ac3d5e2af977cfc01cc9077a0e7c7d671bf28cfe055e42): Bind for 0.0.0.0:8082 failed: port is already allocated
PS C:\Users\raffa\Documents\ZHAW\FS25\DevOps\REPOS\DevOpsCompose\docker-compose> docker compose up
[+] Running 1/1
 ✔ Container docker-compose-db-1  Created                                                                                                                                                        0.0s 
Attaching to db-1, wordpress-1
db-1         | 2025-03-25 13:36:48+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 9.1.0-1.el9 started.
db-1         | 2025-03-25 13:36:48+00:00 [Note] [Entrypoint]: Switching to dedicated user 'mysql'
db-1         | 2025-03-25 13:36:48+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 9.1.0-1.el9 started.
wordpress-1  | WordPress not found in /var/www/html - copying now...
db-1         | 2025-03-25 13:36:48+00:00 [Note] [Entrypoint]: Initializing database files
db-1         | 2025-03-25T13:36:48.775474Z 0 [System] [MY-015017] [Server] MySQL Server Initialization - start.
db-1         | 2025-03-25T13:36:48.777180Z 0 [System] [MY-013169] [Server] /usr/sbin/mysqld (mysqld 9.1.0) initializing of server in progress as process 80
db-1         | 2025-03-25T13:36:48.797858Z 1 [System] [MY-013576] [InnoDB] InnoDB initialization has started.
wordpress-1  | Complete! WordPress has been successfully copied to /var/www/html                                                                                                                      
wordpress-1  | No 'wp-config.php' found in /var/www/html, but 'WORDPRESS_...' variables supplied; copying 'wp-config-docker.php' (WORDPRESS_DB_HOST WORDPRESS_DB_NAME WORDPRESS_DB_PASSWORD WORDPRESS_DB_USER)                                                                                                                                                                                              
wordpress-1  | AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 172.20.0.3. Set the 'ServerName' directive globally to suppress this message
wordpress-1  | AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 172.20.0.3. Set the 'ServerName' directive globally to suppress this message
wordpress-1  | [Tue Mar 25 13:36:49.042578 2025] [mpm_prefork:notice] [pid 1:tid 1] AH00163: Apache/2.4.62 (Debian) PHP/8.3.14 configured -- resuming normal operations
wordpress-1  | [Tue Mar 25 13:36:49.042627 2025] [core:notice] [pid 1:tid 1] AH00094: Command line: 'apache2 -D FOREGROUND'
db-1         | 2025-03-25T13:36:49.202758Z 1 [System] [MY-013577] [InnoDB] InnoDB initialization has ended.                                                                                           
db-1         | 2025-03-25T13:36:50.431735Z 6 [Warning] [MY-010453] [Server] root@localhost is created with an empty password ! Please consider switching off the --initialize-insecure option.
db-1         | 2025-03-25T13:36:53.107604Z 0 [System] [MY-015018] [Server] MySQL Server Initialization - end.
db-1         | 2025-03-25 13:36:53+00:00 [Note] [Entrypoint]: Database files initialized
db-1         | 2025-03-25 13:36:53+00:00 [Note] [Entrypoint]: Starting temporary server
db-1         | 2025-03-25T13:36:53.227954Z 0 [System] [MY-015015] [Server] MySQL Server - start.                                                                                                      
db-1         | 2025-03-25T13:36:53.434224Z 0 [System] [MY-010116] [Server] /usr/sbin/mysqld (mysqld 9.1.0) starting as process 130
db-1         | 2025-03-25T13:36:53.447029Z 1 [System] [MY-013576] [InnoDB] InnoDB initialization has started.                                                                                         
db-1         | 2025-03-25T13:36:53.749877Z 1 [System] [MY-013577] [InnoDB] InnoDB initialization has ended.                                                                                           
db-1         | 2025-03-25T13:36:54.126326Z 0 [Warning] [MY-010068] [Server] CA certificate ca.pem is self signed.
db-1         | 2025-03-25T13:36:54.126407Z 0 [System] [MY-013602] [Server] Channel mysql_main configured to support TLS. Encrypted connections are now supported for this channel.
db-1         | 2025-03-25T13:36:54.130391Z 0 [Warning] [MY-011810] [Server] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.                                                                                                                                                                           
db-1         | 2025-03-25T13:36:54.160061Z 0 [System] [MY-010931] [Server] /usr/sbin/mysqld: ready for connections. Version: '9.1.0'  socket: '/var/run/mysqld/mysqld.sock'  port: 0  MySQL Community Server - GPL.
db-1         | 2025-03-25T13:36:54.159995Z 0 [System] [MY-011323] [Server] X Plugin ready for connections. Socket: /var/run/mysqld/mysqlx.sock
db-1         | 2025-03-25 13:36:54+00:00 [Note] [Entrypoint]: Temporary server started.
db-1         | '/var/lib/mysql/mysql.sock' -> '/var/run/mysqld/mysqld.sock'                                                                                                                           
db-1         | Warning: Unable to load '/usr/share/zoneinfo/iso3166.tab' as time zone. Skipping it.
db-1         | Warning: Unable to load '/usr/share/zoneinfo/leap-seconds.list' as time zone. Skipping it.
db-1         | Warning: Unable to load '/usr/share/zoneinfo/leapseconds' as time zone. Skipping it.                                                                                                   
db-1         | Warning: Unable to load '/usr/share/zoneinfo/tzdata.zi' as time zone. Skipping it.
db-1         | Warning: Unable to load '/usr/share/zoneinfo/zone.tab' as time zone. Skipping it.
db-1         | Warning: Unable to load '/usr/share/zoneinfo/zone1970.tab' as time zone. Skipping it.                                                                                                  
db-1         | 2025-03-25 13:36:56+00:00 [Note] [Entrypoint]: Creating database wordpress
db-1         | 2025-03-25 13:36:56+00:00 [Note] [Entrypoint]: Creating user wordpress
db-1         | 2025-03-25 13:36:56+00:00 [Note] [Entrypoint]: Giving user wordpress access to schema wordpress
db-1         | 
db-1         | 2025-03-25 13:36:56+00:00 [Note] [Entrypoint]: Stopping temporary server
db-1         | 2025-03-25T13:36:56.764586Z 13 [System] [MY-013172] [Server] Received SHUTDOWN from user root. Shutting down mysqld (Version: 9.1.0).                                                  
db-1         | 2025-03-25T13:36:57.494459Z 0 [System] [MY-010910] [Server] /usr/sbin/mysqld: Shutdown complete (mysqld 9.1.0)  MySQL Community Server - GPL.
db-1         | 2025-03-25T13:36:57.494538Z 0 [System] [MY-015016] [Server] MySQL Server - end.
db-1         | 2025-03-25 13:36:57+00:00 [Note] [Entrypoint]: Temporary server stopped                                                                                                                
db-1         | 
db-1         | 2025-03-25 13:36:57+00:00 [Note] [Entrypoint]: MySQL init process done. Ready for start up.                                                                                            
db-1         |                                                                                                                                                                                        
db-1         | 2025-03-25T13:36:57.782636Z 0 [System] [MY-015015] [Server] MySQL Server - start.                                                                                                      
db-1         | 2025-03-25T13:36:57.991692Z 0 [System] [MY-010116] [Server] /usr/sbin/mysqld (mysqld 9.1.0) starting as process 1
db-1         | 2025-03-25T13:36:58.003914Z 1 [System] [MY-013576] [InnoDB] InnoDB initialization has started.
db-1         | 2025-03-25T13:36:58.301510Z 1 [System] [MY-013577] [InnoDB] InnoDB initialization has ended.                                                                                           
db-1         | 2025-03-25T13:36:58.636648Z 0 [Warning] [MY-010068] [Server] CA certificate ca.pem is self signed.
db-1         | 2025-03-25T13:36:58.636734Z 0 [System] [MY-013602] [Server] Channel mysql_main configured to support TLS. Encrypted connections are now supported for this channel.
db-1         | 2025-03-25T13:36:58.641101Z 0 [Warning] [MY-011810] [Server] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
db-1         | 2025-03-25T13:36:58.673898Z 0 [System] [MY-011323] [Server] X Plugin ready for connections. Bind-address: '::' port: 33060, socket: /var/run/mysqld/mysqlx.sock
db-1         | 2025-03-25T13:36:58.674139Z 0 [System] [MY-010931] [Server] /usr/sbin/mysqld: ready for connections. Version: '9.1.0'  socket: '/var/run/mysqld/mysqld.sock'  port: 3306  MySQL Community Server - GPL.                                                                                                                                                                                      
wordpress-1  | 172.20.0.1 - - [25/Mar/2025:13:37:41 +0000] "POST /wp-admin/admin-ajax.php HTTP/1.1" 302 405 "http://localhost:8082/wp-admin/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
wordpress-1  | 172.20.0.1 - - [25/Mar/2025:13:37:41 +0000] "GET /wp-admin/install.php HTTP/1.1" 200 4670 "http://localhost:8082/wp-admin/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
wordpress-1  | 172.20.0.1 - - [25/Mar/2025:13:37:46 +0000] "GET / HTTP/1.1" 302 404 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
wordpress-1  | 172.20.0.1 - - [25/Mar/2025:13:37:46 +0000] "GET /wp-admin/install.php HTTP/1.1" 200 4670 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
wordpress-1  | 172.20.0.1 - - [25/Mar/2025:13:37:49 +0000] "POST /wp-admin/install.php?step=1 HTTP/1.1" 200 2768 "http://localhost:8082/wp-admin/install.php" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Safari/537.36"
wordpress-1  | 172.20.0.1 - - [25/Mar/2025:13:38:38 +0000] "-" 408 0 "-" "-"
wordpress-1  | [Tue Mar 25 13:39:21.442620 2025] [mpm_prefork:notice] [pid 1:tid 1] AH00170: caught SIGWINCH, shutting down gracefully
wordpress-1 exited with code 0
db-1         | 2025-03-25T13:39:23.017613Z 0 [System] [MY-013172] [Server] Received SHUTDOWN from user <via user signal>. Shutting down mysqld (Version: 9.1.0).
db-1         | 2025-03-25T13:39:24.114347Z 0 [System] [MY-010910] [Server] /usr/sbin/mysqld: Shutdown complete (mysqld 9.1.0)  MySQL Community Server - GPL.
db-1         | 2025-03-25T13:39:24.114404Z 0 [System] [MY-015016] [Server] MySQL Server - end.
db-1 exited with code 0


```