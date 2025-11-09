# mysql56-server-freebsd13-14-metin2
mysql56-server-freebsd-metin2

I just find more than files to install the mysql56-server/client , and i know is hard to up install on this system..
i let here maybe is helpfull..

pkg install openssl

pkg install -y wget

pkg install -y unzip

   - 'wget https://github.com/mambombo777/mysql56-server-freebsd-metin2/archive/refs/heads/main.zip'
    - 'unzip -o main.zip'
    - 'cd mysql56-server-freebsd-metin2-main'
    - 'unzip -o mysql56.zip'
    - 'cd mysql56'
    - 'tar -zxzf libs_64bit_mysql.tgz -C /'
    - 'tar -zxvf libs_64bit_mysql.tgz -C /'
    - 'pkg install -y mysql56-client-5.6.51.pkg mysql56-server-5.6.51.pkg'
    - 'sysrc mysql_enable=YES'
    - 'service mysql-server start'
    - 'mysql_secure_installation
