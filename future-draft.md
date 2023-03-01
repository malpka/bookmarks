# March 2023

## Applications

- [VeraCrypt - Free Open source disk encryption with strong security for the Paranoid](https://documentation.help/VeraCrypt/Command%20Line%20Usage.html) Command line. You can brute force password list for example.
- [Kalkulator finansowy](https://kalkulatorfinansowy.app/app/#/) The most versatile financial calculator for individuals in Poland
- [MobaXterm free Xserver and tabbed SSH client for Windows](https://mobaxterm.mobatek.net/)  MobaXterm Enhanced terminal for Windows with X11 server, tabbed SSH client, network tools and much more. Putty killer! It can easily use PEM keys for authehtication.
- [Personal online office](https://personal.onlyoffice.com/) Download free desktop app to edit files offline or connect to your cloud.<br/><img src="https://personal.onlyoffice.com/site-assets/screenshots/en-US/doc.png">

## System tools

- [Windows 10: Built-in tools for Hard Disk Health check](https://social.technet.microsoft.com/wiki/contents/articles/53235.windows-10-built-in-tools-for-hard-disk-health-check.aspx)<br/>
  `wmic diskdrive get status`<br/>
  `wmic diskdrive get`<br/>
  `PS> Get-CimInstance -class "win32_diskdrive"`
- [How to get full PC memory specs (speed, size, type, part number, form factor) on Windows 10](https://www.windowscentral.com/how-get-full-memory-specs-speed-size-type-part-number-form-factor-windows-10)
  `wmic memorychip get devicelocator, manufacturer`<br/>
  `wmic memorychip get devicelocator, partnumber`<br/>
  `wmic memorychip get devicelocator, serialnumber`<br/>
  `wmic memorychip get banklabel, serialnumber`<br/>
  `wmic memorychip get devicelocator, capacity`<br/>
  `systeminfo | findstr /C:"Total Physical Memory"`<br/>
  `wmic memorychip get devicelocator, speed`<br/>
  `wmic memorychip get devicelocator, memorytype`<br/>
  `wmic memorychip get devicelocator, formfactor`<br/>
  `wmic memorychip list full`<br/>
  `wmic memorychip get devicelocator, manufacturer, partnumber, serialnumber, capacity, speed, memorytype, formfactor`<br/>

## Linux

- [Tmux Cheat Sheet & Quick Reference](https://tmuxcheatsheet.com/)
- [How do I scroll in tmux?](https://superuser.com/questions/209437/how-do-i-scroll-in-tmux)<br/>
  `Ctrl-b then [ then arrows`
- [How to run SSH server on multiple ports](https://www.simplified.guide/ssh/run-multiple-ports)
- [How to view connected users to open vpn server?](https://serverfault.com/questions/571592/how-to-view-connected-users-to-open-vpn-server)<br/>
  `cat /etc/openvpn/openvpn-status.log`<br/>
  `server.conf -> 'management localhost 7505'`<br/>
  `telnet localhost 7505`
- [linux mint - OpenSSL: error:0A00018E:SSL routines::ca md too weak - Super User](https://superuser.com/questions/1737052/openssl-error0a00018essl-routinesca-md-too-weak)<br/>
  `tls-cipher "DEFAULT:@SECLEVEL=0"`
- [Pakiet: apt-utils (2.5.6) Programy narzędziowe związane z zarządzaniem pakietami](https://packages.debian.org/pl/sid/apt-utils)
- [NetToolsDeprecation](https://wiki.debian.org/NetToolsDeprecation) Debian
- [ss(8) — Linux manual page](https://man7.org/linux/man-pages/man8/ss.8.html) ss - another utility to investigate sockets<br/>
  You can use ss just like netstat:<br/>
  `ss -tanp`<br/>
  `ss -u -a`
- [Deprecated Linux networking commands and their replacements](https://dougvitale.wordpress.com/2011/12/21/deprecated-linux-networking-commands-and-their-replacements/#netstat)


|Deprecatedcommand|Replacement command(s)|
|:-----------------|:----------------------|
|arp|ip n (ip neighbor)|
|ifconfig|ip a (ip addr), ip link, ip -s (ip -stats)|
|iptunnel|ip tunnel|
|iwconfig|iw|
|nameif|ip link, ifrename|
|netstat|ss, ip route (for netstat-r), ip -s link (for netstat -i), ip maddr (for netstat-g)|
|route|ip r (ip route)|
-

### Docker

- [Getting started with Docker for Arm on Linux](https://www.docker.com/blog/getting-started-with-docker-for-arm-on-linux/)
- [Nginx official Docker image](https://hub.docker.com/_/nginx) Usage help included

## Android

- [How do I get the APK of an installed app without root access?](https://stackoverflow.com/questions/11012976/how-do-i-get-the-apk-of-an-installed-app-without-root-access) <br/>
  ```adb shell pm list packages
  adb shell pm path your-package-name
  adb pull full/directory/of/the.apk
  for i in $(adb shell pm list packages | awk -F':' '{print $2}'); do 
    adb pull "$(adb shell pm path $i | awk -F':' '{print $2}')"
    mv base.apk $i.apk &> /dev/null 
  done
- [Android Debug Bridge (adb) &nbsp;|&nbsp; Android Developers](https://developer.android.com/studio/command-line/adb) Command line

## Hardware

- [8 Best Motherboards for Ryzen 9 5950X in 2021](https://finaldesktop.com/motherboards/best-motherboard-for-ryzen-9-5950x#asus-tuf-gaming-x570-plus-wi-fi)
  1. Asus ROG Strix X570-E
  2. GIGABYTE X570 ELITE
  3. ASUS PRIME X570-PRO
  4. MSI MPG X570 PLUS
  5. ASUS TUF X570-Plus
  6. MSI MPG X570 EDGE WIFI
  7. Gigabyte B550M PRO-P
  8. ASUS ROG STRIX X570-I

## NAS

- [Google Images for NAS DIY from recent year](https://www.google.com/search?q=nas+diy&sa=X&biw=2085&bih=1279&tbs=qdr:y&tbm=isch&source=iu&ictx=1&vet=1)
- [Forum: [DIY] NAS bez kompromisów - OpenLinksys](https://www.openlinksys.info/forum/viewthread.php?thread_id=22708) Really nice description of self designed and made NAS
- [Procesor Intel® Core™ i5-6500T Cache 6 MB, nawet do 3,10 GHz](https://www.intel.pl/content/www/pl/pl/products/sku/88183/intel-core-i56500t-processor-6m-cache-up-to-3-10-ghz/specifications.html) i5-6500T Processor ideal for NAS 4C/4T
- [Xpenology: The Definitive Guide to Running Xpenology (2020 Update)](https://xpenology.org/) Xpenology: Run Synology DSM Software on Your Own Hardware

## Cryptocurrency

- [RTX 2070 Super Mining Settings](https://miningchamber.com/gpus/rtx-2070-super/mining-settings)

## System tools

## E-Shop

- [Integracje API oraz z popularnymi platformami - epaka.pl biznes](https://www.epaka.pl/biznes/integracje) Woocommerce Prestashop Allegro.pl Shoper
- [Integracje - Furgonetka.pl](https://furgonetka.pl/konto/integracje/)
- [Woo Marketplace Grow your business with hundreds of solutions to solve all your logistical, technical, and marketing needs.](https://woocommerce.com/products/) 

## Games

### Vermintide 2

## Lifestyle

## Health

- [7 ćwiczeń na kręgosłup piersiowy - Rehabilitacja](https://www.rehafit.org/cwiczenia-zwiekszajace-ruchomosc-kregoslupa/)

## Investing 

- [Wskaźniki wartości rynkowej MFO - BiznesRadar.pl](https://www.biznesradar.pl/wskazniki-wartosci-rynkowej/MFO)

## 3D Print

- [How to edit STL files | Complete Guide 2023](https://www.crealitycloud.com/blog/tutorials/how-to-edit-stl-files)

## AI

- [Office of Innovation &amp; Technology](https://gse-it.stanford.edu/)

### Midjourney

## NAS

## Home automation

## Web Scrapping 

## Jobs

- [Career at Proxet | Proxet Nation](https://nation.proxet.com/careers/)
- [SOLID.Jobs – Platforma rekrutacyjna dla specjalistów](https://solid.jobs/offers/it)

## Cloud

- [Principles for designing and deploying scalable applications on Kubernetes | Cloud Native Computing Foundation](https://www.cncf.io/blog/2022/02/17/principles-for-designing-and-deploying-scalable-applications-on-kubernetes/)
- [Opening port 80 on Oracle Cloud Infrastructure Compute node - Stack Overflow](https://stackoverflow.com/questions/54794217/opening-port-80-on-oracle-cloud-infrastructure-compute-node)
- [Ubuntu Manpage: netfilter-persistent - load, flush and save netfilter rule sets](https://manpages.ubuntu.com/manpages/xenial/man8/netfilter-persistent.8.html)

## Programming

- [Quasar Framework](https://quasar.dev/) Effortlessly build high-performance & high-quality Vue.js 3 user interfaces in record time. First version of https://kalkulatorfinansowy.app/ was published using this Framework as I remember. Later it was moved to VueJS. https://quasar.dev/quasar-cli-webpack/routing
- [Vue Router](https://router.vuejs.org/) The official Router for Vue.js. Expressive, configurable and convenient routing for Vue.js
- [You Probably Don&#x27;t Need to Worry About MediatR](https://jimmybogard.com/you-probably-dont-need-to-worry-about-mediatr)

### .NET

- [TessFerrandez/BuggyBits: Debugging Labs - .NET and WinDbg](https://github.com/TessFerrandez/BuggyBits) Buggy Bits is source code for a set of .net post mortem (hang, crash, memory) debugging labs.
- [Introducing .NET MAUI - One Codebase, Many Platforms - .NET Blog](https://devblogs.microsoft.com/dotnet/introducing-dotnet-maui-one-codebase-many-platforms) 
- [Ten cholerny CORS dogłębnie](https://masterbranch.pl/ten-cholerny-cors-doglebnie/)
- [A modern alternative to the Microsoft Assembly Binding Log Viewer (FUSLOGVW.exe)](https://github.com/awaescher/Fusion) <img src="https://github.com/awaescher/Fusion/raw/master/_doc/Fusion++NoDetail.png">

## Security

- [SekurakTV - Jak skutecznie monitorować cyberbezpieczeństwo i od czego zacząć?](https://www.youtube.com/watch?v=dzaK-LgpJKs)
- [SekurakTV - Dlaczego hackowanie aplikacji webowych jest proste? Szkolenie od sekuraka](https://www.youtube.com/watch?v=2S15DyhTlsU)
- [Bezpieczeństwo Windows – czym jest LSASS dump. Jak się przed nim chronić?](https://sekurak.pl/bezpieczenstwo-windows-czym-jest-lsass-dump-jak-sie-przed-nim-chronic) Windows Security - what is LSASS dump and how to protect against it
- [The End of PPLdump | itm4n's blog](https://itm4n.github.io/the-end-of-ppldump/)
- [Signed driver malware moves up the software trust chain – Sophos News](https://news.sophos.com/en-us/2022/12/13/signed-driver-malware-moves-up-the-software-trust-chain/) BURNTCIGAR; signed driver; WinRing0; sc create; IoCreateDevice 
 

## Amateur Radio

- [Jak zostać krótkofalowcem? - HamNews.pl](https://hamnews.pl/jak-zostac-krotkofalowcem/) How to become a legal amateur radio user in Poland. Details about exams, tests.
- [Czestotliwosci - Pozwolenia Radiowe](https://czestotliwosci.pl.tl/Pozwolenia-Radiowe.htm) Important radio frequencies in Poland

## Oracle Cloud Free Tier resources

- [Oracle Cloud Free Tier](https://www.oracle.com/cloud/free/) <br/> #cloud/vps/shell/bash/linux
  Oracle gives totally for free a possibility to create a VPS linux machine, that you can manipulate using SSH. You can treat it as a development / testing environment.<br/>
  <img src="https://raw.githubusercontent.com/malpka/bookmarks/main/images/2023-01-21_161317.png" alt="Oracle img" width="200" onmouseover="this.width='400'" onmouseout="this.width='200'"/>
- [Opening port 80 on Oracle Cloud Infrastructure Compute node - Stack Overflow](https://stackoverflow.com/questions/54794217/opening-port-80-on-oracle-cloud-infrastructure-compute-node)
- [Ubuntu Manpage: netfilter-persistent - load, flush and save netfilter rule sets](https://manpages.ubuntu.com/manpages/xenial/man8/netfilter-persistent.8.html)
