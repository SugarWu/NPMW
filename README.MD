# linode Promo Code
https://promo.linode.com/podcastinit/?r=637a37066ce28fc35fbe9fcb300573b3f9ae3584
<br>推薦碼(Referral Code) :  637a37066ce28fc35fbe9fcb300573b3f9ae3584
<br>送 $ 20美金優惠碼(Promo Code): PodcastInIt2017

# Centos 7 
# 1/2 install docker 
sudo yum install -y yum-utils wget ; sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo ; sudo yum makecache fast ; sudo yum -y install docker-ce ; systemctl start docker ; systemctl enable docker ; docker --version

# 2/2 install docker-compose
curl -L "https://github.com/docker/compose/releases/download/1.11.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose ; chmod +x /usr/local/bin/docker-compose ; docker-compose --version

# Setup NPMW
1. mkdir {yourfolder} 
2. cd {yourfolder}
3. wget  https://github.com/SugarWu/NPMW/raw/master/npmw.tar.gz
4. tar -xzvf npmw.tar.gz
5. docker-compose up -d
6. docker exec {yourfolder}_php_1 chown -R www-data:www-data /var/www/html
