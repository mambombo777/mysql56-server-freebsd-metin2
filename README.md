# mysql56-server-freebsd13-14-metin2
mysql56-server-freebsd-metin2

I just find more than files to install the mysql56-server/client , and i know is hard to up install on this system..
i let here maybe is helpfull..

pkg install openssl

pkg install -y wget

pkg install -y unzip

unzip mysql.zip

(***find / -iname "libssl.so.111" && find / -iname "libcrypto.so.111"
this command should this result as they are installed

/usr/lib/libssl.so.111
/lib/libcrypto.so.111***)

tar -xzf libs_64bit_mysql.tgz -C /

tar -xzf libs_32bit_mysql.tgz -C /

pkg install mysql56-client-5.6.51.pkg mysql56-server-5.6.51.pkg

sysrc mysql_enable=YES

service mysql-server start

mysql_secure_installation
