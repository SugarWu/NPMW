# Centos 7 
# 1/3 install docker 
sudo yum install -y yum-utils
sudo yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo
sudo yum makecache fast
sudo yum -y install docker-ce
sudo systemctl start docker
sudo systemctl enable docker
sudo docker --version

# 2/3 install docker-compose
curl -L "https://github.com/docker/compose/releases/download/1.11.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
docker-compose --version

# Setup NPMW
1. mkdir <yourfolder> 
2. cd <yourfolder>
3. wget npmw.tar.gz
4. tar -xzvf npmw.tar.gz
5. docker-compose up -d
6. docker exec <yourfolder>_php_1 chown -R www-data:www-data /var/www/html
