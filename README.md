# task18
yum update
dnf install https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm -y
dnf install http://rpms.remirepo.net/enterprise/remi-release-8.rpm
yum install wget vim
yum module install php:remi-7.4
yum install mysql -y
yum install httpd -y
systemctl start httpd
systemctl enable httpd
yum install mysqlnd -y
wget http://wordpress.org/latest.tar.gz
tar -xvzf latest.tar.gz -C /var/www/html
