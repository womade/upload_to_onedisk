# upload_to_onedisk


### 上传文件
```
sudo -E apt-get -qq install php php-curl
wget https://github.com/womade/upload_to_onedisk/raw/main/o.tar.gz
tar -zxvf o.tar.gz
wget ${{ secrets.CONFIG }} -O config.tar.gz
tar -zxvf config.tar.gz
php onedisk/one.php upload:file /本地文件 /云端文件
php onedisk/one.php upload:folder /本地文件夹 /云端文件夹
```
