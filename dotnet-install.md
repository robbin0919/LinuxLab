root@ubuntu00:/home/robbin0919# wget https://dot.net/v1/dotnet-install.sh -O dotnet-install.sh  
--2024-05-26 13:41:10--  https://dot.net/v1/dotnet-install.sh  
Resolving dot.net (dot.net)... 20.70.246.20, 20.76.201.171, 20.112.250.133, ...  
Connecting to dot.net (dot.net)|20.70.246.20|:443... connected.  
HTTP request sent, awaiting response... 301 Moved Permanently   
Location: https://dotnet.microsoft.com/download/dotnet/scripts/v1/dotnet-install.sh [following]  
--2024-05-26 13:41:11--  https://dotnet.microsoft.com/download/dotnet/scripts/v1/dotnet-install.sh  
Resolving dotnet.microsoft.com (dotnet.microsoft.com)... 13.107.246.73, 13.107.213.73, 2620:1ec:bdf::73, ...  
Connecting to dotnet.microsoft.com (dotnet.microsoft.com)|13.107.246.73|:443... connected.  
HTTP request sent, awaiting response... 200 OK  
Cookie coming from dotnet.microsoft.com attempted to set domain to dotnetwebsite.azurewebsites.net  
Cookie coming from dotnet.microsoft.com attempted to set domain to dotnetwebsite.azurewebsites.net  
Length: 63194 (62K) [application/x-sh]  
Saving to: ‘dotnet-install.sh’  
  
dotnet-install.sh                                      100%[=========================================================================================================================>]  61.71K   229KB/s    in 0.3s  
  
2024-05-26 13:41:12 (229 KB/s) - ‘dotnet-install.sh’ saved [63194/63194]   
  
root@ubuntu00:/home/robbin0919# chmod +x ./dotnet-install.sh  
root@ubuntu00:/home/robbin0919# ./dotnet-install.sh --channel 6.0  
dotnet-install: Attempting to download using aka.ms link https://dotnetcli.azureedge.net/dotnet/Sdk/6.0.422/dotnet-sdk-6.0.422-linux-x64.tar.gz  
dotnet-install: Remote file https://dotnetcli.azureedge.net/dotnet/Sdk/6.0.422/dotnet-sdk-6.0.422-linux-x64.tar.gz size is 187265855 bytes.  
dotnet-install: Extracting archive from https://dotnetcli.azureedge.net/dotnet/Sdk/6.0.422/dotnet-sdk-6.0.422-linux-x64.tar.gz  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
cp: warning: behavior of -n is non-portable and may change in future; use --update=none instead  
dotnet-install: Downloaded file size is 187265855 bytes.  
dotnet-install: The remote and local file sizes are equal.  
dotnet-install: Installed version is 6.0.422  
dotnet-install: Adding to current process PATH: `/root/.dotnet`. Note: This change will be visible only when sourcing script.  
dotnet-install: Note that the script does not resolve dependencies during installation.  
dotnet-install: To check the list of dependencies, go to https://learn.microsoft.com/dotnet/core/install, select your operating system and check the "Dependencies" section.  
dotnet-install: Installation finished successfully.  

