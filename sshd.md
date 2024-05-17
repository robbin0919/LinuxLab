 
Ubuntu Server 重新安裝或安裝 OpenSSH Server 的其他版本
----

1. 更新 apt 存儲庫  
```
sudo apt update  
```
2. 安裝 OpenSSH Server
```
sudo apt install openssh-server
```
3. 驗證 SSH 服務是否已啟動  
```
sudo systemctl status sshd
```
如果輸出顯示 active (running)，則 SSH 服務已啟動。

4. 允許來自客戶端電腦的 SSH 連線  

您可以使用以下命令添加防火牆規則來允許來自特定 IP 地址的 SSH 連線：  
```
sudo ufw allow <client_ip_address> 22
```
例如，要允許來自 192.168.1.100 的 SSH 連線，您可以使用以下命令：  
```
sudo ufw allow 192.168.1.100 22
```
5. 如果您想允許來自多個 IP 地址的 SSH 連線，可以使用以下命令添加通配符規則：  
```
sudo ufw allow from <subnet> 22
```
例如，要允許來自 192.168.1.0/24 網段的 SSH 連線，您可以使用以下命令：  
```
sudo ufw allow from 192.168.1.0/24 22
```
6. 完成上述所有步驟後，您就可以從客戶端電腦使用 SSH 登入伺服器了。打開 SSH 客戶端軟體，並輸入以下命令：  
```
ssh username@server_ip_address
```
例如，要使用用戶名 ubuntu 登入伺服器 IP 地址為 192.168.1.100 的伺服器，您可以使用以下命令：  
```
ssh ubuntu@192.168.1.100
``` 
您會被提示輸入密碼。輸入密碼後，您將登入伺服器。  

以下是一些使用 SSH 登入 Ubuntu Server 的其他提示：  

您可以使用 SSH 密鑰來提高安全性。SSH 密鑰是一種加密的認證方法，可讓您無需輸入密碼即可登入伺服器。  
您可以使用 SSH 配置檔案來指定默認用戶名、端口號和其他 SSH 連線設置。  
您可以使用 SSH 轉發來將本地端口轉發到伺服器上的端口。這對於訪問伺服器上的服務（例如 Web 伺服器或資料庫伺服器）很有用。  