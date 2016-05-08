# centos6-apache-php-sqlite2
Dockerfile for php5.3.3 with sqlite2 and apache on CentOS6.
Using only yum (and yumdownloader, gcc).

    $ docker run -it paijp/centos6-apache-php-sqlite2
    PDO Driver for SQLite 3.x => enabled
    SQLite Library => 3.6.20
    SQLite
    SQLite support => enabled
    SQLite Library => 2.8.17        /* sqlite2 enabled. */
    SQLite Encoding => iso8859
    SQLite3 support => enabled
    SQLite3 module version => 0.7-dev
    SQLite Library => 3.6.20
    
    $ docker run -it -p 80:80 paijp/centos6-apache-php-sqlite2 /bin/bash
    # yum install php-gd php-mbstring
    # /etc/init.d/httpd start
