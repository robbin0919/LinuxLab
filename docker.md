https://docs.docker.com/engine/install/ubuntu/  
安裝步驟　　

參考官網4提供的步驟。下方簡單做個講解,可以大致了解每個步驟的用途後,到官網複製指令。

■ 設定儲存庫(repository),也就是文件中的「Set up the repository」所列出來的步驟:　　

#更新套件管理器(apt)的索引　　
$ sudo apt-get update　　

#安裝必要的套件　　
$ sudo apt-get install ca-certificates curl gnupg　　

#增加 Docker 的官方GPG key,這一步可以用來驗證Docker儲存庫下載的軟體包的完整性。　　

$ sudo install -m 0755 -d /etc/apt/keyrings　　

#如果在以下這個步驟有遇到curl:(60)SSL: no alternative certificate subject　name matches target host name 'download.docker.com'這個錯誤訊息,可以試著在cur1指令加上-k參數(curl -fsSL -k …… 略)　　

$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg |sudo gpg　　-- dearmor -o /etc/apt/keyrings/docker.gpg　　

$ sudo chmod a+r /etc/apt/keyrings/docker.gpg　　

#設定Docker官方的儲存庫　　　　

$ echo \　　
"deb [arch="$(dpkg -- print-architecture)" signed-by=/etc/apt/keyrings/　　
docker.gpg] https://download.docker.com/linux/ubuntu \　　
"$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" / \　　
sudo tee /etc/apt/sources.list.d/docker.list > /dev/null　　

$ echo 　"deb [arch="$(dpkg -- print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] 　https://download.docker.com/linux/ubuntu "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" /　sudo tee /etc/apt/sources.list.d/docker.list > /dev/null　　

#在設定完Docker官方的儲存庫後,記得要再更新一次apt的索引　　

#注意:這一步官網是放在「Install Docker Engine」步驟中,但以理解來說,放在這一步驟裡,應該會有較好的連結。　　

$ sudo apt-get update　　

