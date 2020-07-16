cd d:/xxxxx
git clone https://github.com/sohutv/cachecloud.git
source cachecloud.sql;

(1). 本地启动:
在cachecloud根目录下运行
mvn clean compile install -Plocal
在cachecloud-open-web模块下运行
mvn spring-boot:run

上传cachecloud-init.sh到linux服务器
sh cachecloud-init.sh ddhCache
如果是ubuntu系统
sudo dpkg-reconfigure dash
选择no
sudo apt-get install -y gcc make