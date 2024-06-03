robbin0919@ubuntu00:~$ sudo apt-get install -y dotnet-sdk-6  
[sudo] password for robbin0919:  
Reading package lists... Done  
Building dependency tree... Done  
Reading state information... Done  
E: Unable to locate package dotnet-sdk-6  
robbin0919@ubuntu00:~$ dotnet --list-sdks
robbin0919@ubuntu00:~$ sudo add-apt-repository ppa:dotnet/backports  
PPA publishes dbgsym, you may need to include 'main/debug' component  
Repository: 'Types: deb  
URIs: https://ppa.launchpadcontent.net/dotnet/backports/ubuntu/  
Suites: noble  
Components: main  
'
Description:  
The backports archive provides source-built .NET packages in cases where a   versi                                                             on of .NET is not available in the archive for an Ubuntu release.  

Currently available Ubuntu releases and .NET backports:
  
Ubuntu 24.04 LTS (Noble Numbat)  
├── .NET 6.0 (End of Life on November 12th, 2024)  
└── .NET 7.0 (End of Life on May 14th, 2024)  

Canonical provides best-effort support for packages contained in this archive,   which is limited to the upstream lifespan or the support period of the particular Ubuntu version. See the upstream support policy [1] for more information about the upstream support lifespan of .NET releases or the Ubuntu Releases Wiki entry  [2] for more information about the support period of any Ubuntu version.

Any build enters ppa:dotnet/backports-proposed [3] first and migrates to this archive if no regressions are reported within a week.  

[1] https://dotnet.microsoft.com/en-us/platform/support/policy/dotnet-core  
[2] https://wiki.ubuntu.com/Releases  
[3] https://launchpad.net/~dotnet/+archive/ubuntu/backports-proposed  
More info: https://launchpad.net/~dotnet/+archive/ubuntu/backports  
Adding repository.  
Press [ENTER] to continue or Ctrl-c to cancel.  
Hit:1 http://tw.archive.ubuntu.com/ubuntu noble InRelease  
Get:2 http://tw.archive.ubuntu.com/ubuntu noble-updates InRelease [126 kB]  
Get:3 http://tw.archive.ubuntu.com/ubuntu noble-backports InRelease [126 kB]  
Get:4 http://tw.archive.ubuntu.com/ubuntu noble-updates/main amd64 Packages [96.9 kB]  
Get:5 http://tw.archive.ubuntu.com/ubuntu noble-updates/main Translation-en [27.9 kB]  
Get:6 http://tw.archive.ubuntu.com/ubuntu noble-updates/main amd64 Components [8,564 B]  
Get:7 http://tw.archive.ubuntu.com/ubuntu noble-updates/restricted amd64 Components [212 B]  
Get:8 http://tw.archive.ubuntu.com/ubuntu noble-updates/universe amd64 Packages [44.9 kB]  
Get:9 http://tw.archive.ubuntu.com/ubuntu noble-updates/universe Translation-en [17.0 kB]
Get:10 http://tw.archive.ubuntu.com/ubuntu noble-updates/universe amd64 Components [45.0 kB]
Get:11 http://tw.archive.ubuntu.com/ubuntu noble-updates/multiverse amd64 Components [212 B]
Get:12 http://tw.archive.ubuntu.com/ubuntu noble-backports/main amd64 Components [208 B]
Get:13 http://tw.archive.ubuntu.com/ubuntu noble-backports/restricted amd64 Components [216 B]
Get:14 http://tw.archive.ubuntu.com/ubuntu noble-backports/universe amd64 Components [17.6 kB]
Get:15 http://tw.archive.ubuntu.com/ubuntu noble-backports/multiverse amd64 Components [212 B]
Get:16 http://security.ubuntu.com/ubuntu noble-security InRelease [126 kB]
Get:17 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble InRelease [24.1 kB]
Get:18 http://security.ubuntu.com/ubuntu noble-security/main amd64 Packages [88.0 kB]
Get:19 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main amd64 Packages [3,688 B]
Get:20 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main Translation-en [1,696 B]
Get:21 http://security.ubuntu.com/ubuntu noble-security/main Translation-en [24.5 kB]
Get:22 http://security.ubuntu.com/ubuntu noble-security/main amd64 Components [6,876 B]
Get:23 http://security.ubuntu.com/ubuntu noble-security/restricted amd64 Components [212 B]
Get:24 http://security.ubuntu.com/ubuntu noble-security/universe amd64 Packages [34.9 kB]
Get:25 http://security.ubuntu.com/ubuntu noble-security/universe Translation-en [13.4 kB]
Get:26 http://security.ubuntu.com/ubuntu noble-security/universe amd64 Components [8,632 B]
Get:27 http://security.ubuntu.com/ubuntu noble-security/multiverse amd64 Components [208 B]
Fetched 844 kB in 3s (287 kB/s)
Reading package lists... Done
robbin0919@ubuntu00:~$ sudo apt-get install -y dotnet-sdk-6
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
E: Unable to locate package dotnet-sdk-6
robbin0919@ubuntu00:~$ sudo apt-get install -y dotnet-sdk-6.0
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages were automatically installed and are no longer required:
  aspnetcore-targeting-pack-8.0 dotnet-apphost-pack-8.0 dotnet-hostfxr-8.0 dotnet-targeting-pack-8.0 dotnet-templates-8.0
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  aspnetcore-runtime-6.0 aspnetcore-targeting-pack-6.0 dotnet-apphost-pack-6.0 dotnet-hostfxr-6.0 dotnet-runtime-6.0
  dotnet-targeting-pack-6.0 dotnet-templates-6.0
The following NEW packages will be installed:
  aspnetcore-runtime-6.0 aspnetcore-targeting-pack-6.0 dotnet-apphost-pack-6.0 dotnet-hostfxr-6.0 dotnet-runtime-6.0 dotnet-sdk-6.0
  dotnet-targeting-pack-6.0 dotnet-templates-6.0
0 upgraded, 8 newly installed, 0 to remove and 35 not upgraded.
Need to get 121 MB of archives.
After this operation, 434 MB of additional disk space will be used.
Get:1 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main amd64 dotnet-hostfxr-6.0 amd64 6.0.129-0ubuntu1~24.04.1~ppa1 [158 kB]
Get:2 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main amd64 dotnet-runtime-6.0 amd64 6.0.129-0ubuntu1~24.04.1~ppa1 [23.4 MB]
Get:3 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main amd64 aspnetcore-runtime-6.0 amd64 6.0.129-0ubuntu1~24.04.1~ppa1 [7,194 kB]
Get:4 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main amd64 aspnetcore-targeting-pack-6.0 amd64 6.0.129-0ubuntu1~24.04.1~ppa1 [1,437 kB]
Get:5 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main amd64 dotnet-apphost-pack-6.0 amd64 6.0.129-0ubuntu1~24.04.1~ppa1 [3,736 kB]
Get:6 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main amd64 dotnet-targeting-pack-6.0 amd64 6.0.129-0ubuntu1~24.04.1~ppa1 [2,214 kB]
Get:7 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main amd64 dotnet-templates-6.0 amd64 6.0.129-0ubuntu1~24.04.1~ppa1 [2,611 kB]
Get:8 https://ppa.launchpadcontent.net/dotnet/backports/ubuntu noble/main amd64 dotnet-sdk-6.0 amd64 6.0.129-0ubuntu1~24.04.1~ppa1 [79.9 MB]
Fetched 121 MB in 5min 21s (376 kB/s)
Selecting previously unselected package dotnet-hostfxr-6.0.
(Reading database ... 84310 files and directories currently installed.)
Preparing to unpack .../0-dotnet-hostfxr-6.0_6.0.129-0ubuntu1~24.04.1~ppa1_amd64.deb ...
Unpacking dotnet-hostfxr-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Selecting previously unselected package dotnet-runtime-6.0.
Preparing to unpack .../1-dotnet-runtime-6.0_6.0.129-0ubuntu1~24.04.1~ppa1_amd64.deb ...
Unpacking dotnet-runtime-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Selecting previously unselected package aspnetcore-runtime-6.0.
Preparing to unpack .../2-aspnetcore-runtime-6.0_6.0.129-0ubuntu1~24.04.1~ppa1_amd64.deb ...
Unpacking aspnetcore-runtime-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Selecting previously unselected package aspnetcore-targeting-pack-6.0.
Preparing to unpack .../3-aspnetcore-targeting-pack-6.0_6.0.129-0ubuntu1~24.04.1~ppa1_amd64.deb ...
Unpacking aspnetcore-targeting-pack-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Selecting previously unselected package dotnet-apphost-pack-6.0.
Preparing to unpack .../4-dotnet-apphost-pack-6.0_6.0.129-0ubuntu1~24.04.1~ppa1_amd64.deb ...
Unpacking dotnet-apphost-pack-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Selecting previously unselected package dotnet-targeting-pack-6.0.
Preparing to unpack .../5-dotnet-targeting-pack-6.0_6.0.129-0ubuntu1~24.04.1~ppa1_amd64.deb ...
Unpacking dotnet-targeting-pack-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Selecting previously unselected package dotnet-templates-6.0.
Preparing to unpack .../6-dotnet-templates-6.0_6.0.129-0ubuntu1~24.04.1~ppa1_amd64.deb ...
Unpacking dotnet-templates-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Selecting previously unselected package dotnet-sdk-6.0.
Preparing to unpack .../7-dotnet-sdk-6.0_6.0.129-0ubuntu1~24.04.1~ppa1_amd64.deb ...
Unpacking dotnet-sdk-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Setting up dotnet-apphost-pack-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Setting up dotnet-targeting-pack-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Setting up aspnetcore-targeting-pack-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Setting up dotnet-hostfxr-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Setting up dotnet-templates-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Setting up dotnet-runtime-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Setting up aspnetcore-runtime-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Setting up dotnet-sdk-6.0 (6.0.129-0ubuntu1~24.04.1~ppa1) ...
Scanning processes...  
Scanning linux images...  
  
Running kernel seems to be up-to-date.  
  
No services need to be restarted.  
  
No containers need to be restarted.  
  
No user sessions are running outdated binaries.  
  
No VM guests are running outdated hypervisor (qemu) binaries on this host.  
robbin0919@ubuntu00:~$ dotnet --list-sdks  
6.0.129 [/usr/lib/dotnet/sdk]  
robbin0919@ubuntu00:~$  
