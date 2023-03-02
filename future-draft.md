# March 2023


## Applications

- [VeraCrypt - Free Open source disk encryption with strong security for the Paranoid](https://documentation.help/VeraCrypt/Command%20Line%20Usage.html) Command line. You can brute force password list for example.
- [Kalkulator finansowy](https://kalkulatorfinansowy.app/app/#/) The most versatile financial calculator for individuals in Poland
- [MobaXterm free Xserver and tabbed SSH client for Windows](https://mobaxterm.mobatek.net/)  MobaXterm Enhanced terminal for Windows with X11 server, tabbed SSH client, network tools and much more. Putty killer! It can easily use PEM keys for authehtication.
- [Personal online office](https://personal.onlyoffice.com/) Download free desktop app to edit files offline or connect to your cloud.<br/><img src="https://personal.onlyoffice.com/site-assets/screenshots/en-US/doc.png"/>
- [Duplicati 2.0 Free backup software to store encrypted backups online
For Windows, macOS and Linux](https://www.duplicati.com/)<br/><img src="https://www.duplicati.com/images/news/2016-03-20-New-UI.jpg"/>
- [Syncthing - continuous file synchronization program](https://syncthing.net/) Syncthing is a continuous file synchronization program. It synchronizes files between two or more computers in real time, safely protected from prying eyes. Your data is your data alone and you deserve to choose where it is stored, whether it is shared with some third party, and how it's transmitted over the internet. <br/><img src="https://syncthing.net/img/screenshot.png"/>


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

- [mailcow: dockerized - Blog](https://mailcow.email/) The integrated mailcow UI allows administrative work on your mail server instance as well as separated domain administrator and mailbox user access
- [Serwer Email z Postfix, Dovecot na bazie MySQL, Debian lub Ubuntu krok po kroku.](https://www.siemaszko.info/serwer-email-z-postfix-dovecot-na-bazie-mysql-debian-lub-ubuntu/) Email Server with Postfix, Dovecot, MySQL on Debian / Ubuntu

### Docker

- [Getting started with Docker for Arm on Linux](https://www.docker.com/blog/getting-started-with-docker-for-arm-on-linux/)
- [Nginx official Docker image](https://hub.docker.com/_/nginx) Usage help included
- [Oracle Cloud Run Always Free Docker Container on Oracle Cloud Infrastructure - AMIS, Data Driven Blog - Oracle & Microsoft Azure](https://technology.amis.nl/oracle-cloud/run-always-free-docker-container-on-oracle-cloud-infrastructure/) <br/><img src="https://technology.amis.nl/wp-content/uploads/2020/02/image_thumb-26.png"/>
- [Docker - Start containers automatically](https://docs.docker.com/config/containers/start-containers-automatically/) <br/>`docker run -d --restart unless-stopped redis`<br>`docker update --restart unless-stopped $(docker ps -q)`
- [Run the Docker daemon as a non-root user (Rootless mode)](https://docs.docker.com/engine/security/rootless/)

### Kubernetes

- [Principles for designing and deploying scalable applications on Kubernetes | Cloud Native Computing Foundation](https://www.cncf.io/blog/2022/02/17/principles-for-designing-and-deploying-scalable-applications-on-kubernetes/)


##  Windows

- [Logiciels pas cher : Clés de licences Windows, Office, antivirus, jeux-vidéos... | Destock Informatique](https://www.destock-informatique.com/) Windows and Office licenses


## Android

- [How do I get the APK of an installed app without root access?](https://stackoverflow.com/questions/11012976/how-do-i-get-the-apk-of-an-installed-app-without-root-access) <br/>
  ```adb shell pm list packages
  adb shell pm path your-package-name
  adb pull full/directory/of/the.apk
  for i in $(adb shell pm list packages | awk -F':' '{print $2}'); do 
    adb pull "$(adb shell pm path $i | awk -F':' '{print $2}')"
    mv base.apk $i.apk &> /dev/null 
  done
- [How can I export the list of open Chrome tabs? - Android Enthusiasts Stack Exchange](https://android.stackexchange.com/questions/56635/how-can-i-export-the-list-of-open-chrome-tabs/193858#193858)
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


## Bots / Web Scrapping 

- [Amazon-Price-Scrapper](https://github.com/Benyamin-Vala/Amazon-Price-Scrapper) With This Tool You Can Take the Price a Target Product In Amazon With Just That Url Address ;)
- [Amazon Seller Save - Chrome Extension](https://github.com/amafjarkasi/amazon-seller-chrome-extension) Chrome extension to save Amazon seller to Google Sheet webhook for future research via reverse search on products
- [SpikeHD/AmazonMonitor: Amazon price checker, item monitor and stock monitor, all shoved into a Discord bot](https://github.com/SpikeHD/AmazonMonitor)
- [PostMan i przeglądarka - Master Branch](https://masterbranch.pl/postman-i-przegladarka) How to use Chromedriver with Postman


### Telegram
- [Create Telegram Bot Using Python Tutorial with Examples](https://www.pragnakalp.com/create-telegram-bot-using-python-tutorial-with-examples/)
- [pragnakalp/telegram-bot-python: Create Telegram Bot Using Python Tutorial with Examples](https://github.com/pragnakalp/telegram-bot-python)
  - `https://api.telegram.org/botXXXXXXX/getUpdates` - getting bot updates without webhook turned on
  - `https://api.telegram.org/botXXXXXXX/getWebHookInfo`
  - `https://api.telegram.org/botXXXXXXX/setWebhook?url=URL` - setting a webhook to handle all requests to bot channel
- [ngrok - Online in One Line](https://ngrok.com/) ngrok is a simplified API-first ingress-as-a-service that adds connectivity, security, and observability to your apps with no code changes


## Jobs

- [Career at Proxet | Proxet Nation](https://nation.proxet.com/careers/)
- [SOLID.Jobs – Platforma rekrutacyjna dla specjalistów](https://solid.jobs/offers/it)


## Cloud

- [Principles for designing and deploying scalable applications on Kubernetes | Cloud Native Computing Foundation](https://www.cncf.io/blog/2022/02/17/principles-for-designing-and-deploying-scalable-applications-on-kubernetes/)
- [Opening port 80 on Oracle Cloud Infrastructure Compute node - Stack Overflow](https://stackoverflow.com/questions/54794217/opening-port-80-on-oracle-cloud-infrastructure-compute-node)
- [Ubuntu Manpage: netfilter-persistent - load, flush and save netfilter rule sets](https://manpages.ubuntu.com/manpages/xenial/man8/netfilter-persistent.8.html)
- [Make formerly Integromat | Work the way you imagine](https://www.make.com/en) From tasks and workflows to apps and systems, build and automate anything in one powerful visual platform. Free 1000 ops/month<br/>
<img src="https://www.make.com/_next/image?url=https%3A%2F%2Fimages.ctfassets.net%2Fqqlj6g4ee76j%2F3tAR2weCRJT0sKWJMDf6SH%2Fb2498e44da8caec3bf156eb2675850d0%2Fimage__20_.png&w=1920&q=90"/>
- [n8n.io - a powerful workflow automation tool](https://n8n.io/) Workflow automation for technical people. Build complex automations 10x faster, without fighting APIs. Allows to have self hosted env.<br/>
  <img src="https://n8niostorageaccount.blob.core.windows.net/n8nio-strapi-blobs-prod/assets/dropcontact_lemlist_workflow_654a24157f.png"/>
- [Najlepsza nazwa kanału YouTube - jaką wybrać i dlaczego jest tak ważna? | iCEA Group](https://www.grupa-icea.pl/najlepsza-nazwa-kanalu-youtube-jaka-wybrac-i-dlaczego-jest-tak-wazna/)
- [Jekyll • Simple, blog-aware, static sites | Transform your plain text into static websites and blogs](https://jekyllrb.com/)
- [chadgeary/cloudblock: Cloudblock deploys secure ad-blocking and VPN for all devices. Text and video guides included! 6 supported cloud providers, plus Ubuntu and Raspberry Pi. Cloudblock deploys Wireguard VPN, Pi-Hole DNS Ad-blocking, and DNS over HTTPS in a cloud provider - or locally - using Terraform and Ansible.](https://github.com/chadgeary/cloudblock/) End-to-end DNS encryption with DNS-based ad-blocking, built in the cloud automatically using Terraform with Ansible. Choose your cloud provider or a standalone installation. Combines wireguard (DNS VPN), pihole (adblock), and cloudflared (DNS over HTTPS) docker containers, as visualized:<br/><img src="https://github.com/chadgeary/cloudblock/raw/master/diagram.png"/>
- [chadgeary/cloudoffice: Cloudoffice deploys Nextcloud and OnlyOffice automatically with LetsEncrypt HTTPS certificates. Text and video instructions included. Six compatible cloud providers, or via Ubuntu/Raspberry Pi. Cloud provider deployments include low-cost object storage integration (e.g. S3).](https://github.com/chadgeary/cloudoffice) Nextcloud built in the cloud automatically using Terraform with Ansible. Now with optional duckdns.org/letsencrypt support!
Available for several major cloud providers, including: AWS (EC2 or Lightsail), Azure, Digital Ocean, GCP (Google), OCI (Oracle), Scaleway (scw) + standalone Raspberry Pi/Ubuntu Server deployment options. <br/><img src="https://github.com/chadgeary/cloudoffice/raw/master/cloudofficediagram.png"/>


## Programming

- [Quasar Framework](https://quasar.dev/) Effortlessly build high-performance & high-quality Vue.js 3 user interfaces in record time. First version of https://kalkulatorfinansowy.app/ was published using this Framework as I remember. Later it was moved to VueJS. https://quasar.dev/quasar-cli-webpack/routing
- [Vue Router](https://router.vuejs.org/) The official Router for Vue.js. Expressive, configurable and convenient routing for Vue.js
- [You Probably Don&#x27;t Need to Worry About MediatR](https://jimmybogard.com/you-probably-dont-need-to-worry-about-mediatr)
- [Reverse engineering STM32 firmware | by Alexander Olenyev | TechMaker | Medium](https://medium.com/techmaker/reverse-engineering-stm32-firmware-578d53e79b3)
- [radare](https://rada.re/r/) Radare is a portable reversing framework that can…
  - Disassemble (and assemble for) many different architectures
  - Debug with local native and remote debuggers (gdb, rap, webui, r2pipe, winedbg, windbg)
  - Run on Linux, *BSD, Windows, OSX, Android, iOS, Solaris and Haiku
  - Perform forensics on filesystems and data carving
  - Be scripted in Python, Javascript, Go and more
  - Support collaborative analysis using the embedded webserver
  - Visualize data structures of several file types
  - Patch programs to uncover new features or fix vulnerabilities
  - Use powerful analysis capabilities to speed up reversing
  - Aid in software exploitation<br/>
  <img src="https://rada.re/r/img/webui.png"/>
- [Challenging algorithms and data structures every programmer should try - Austin Z. Henley](https://austinhenley.com/blog/challengingalgorithms.html)


### .NET

- [TessFerrandez/BuggyBits: Debugging Labs - .NET and WinDbg](https://github.com/TessFerrandez/BuggyBits) Buggy Bits is source code for a set of .net post mortem (hang, crash, memory) debugging labs.
- [Introducing .NET MAUI - One Codebase, Many Platforms - .NET Blog](https://devblogs.microsoft.com/dotnet/introducing-dotnet-maui-one-codebase-many-platforms) 
- [Ten cholerny CORS dogłębnie](https://masterbranch.pl/ten-cholerny-cors-doglebnie/)
- [A modern alternative to the Microsoft Assembly Binding Log Viewer (FUSLOGVW.exe)](https://github.com/awaescher/Fusion) <img src="https://github.com/awaescher/Fusion/raw/master/_doc/Fusion++NoDetail.png"/>
- [Ten cholerny CORS dogłębnie - Master Branch](https://masterbranch.pl/ten-cholerny-cors-doglebnie) This bloody CORS in detail


## Security

- [SekurakTV - Jak skutecznie monitorować cyberbezpieczeństwo i od czego zacząć?](https://www.youtube.com/watch?v=dzaK-LgpJKs)
- [SekurakTV - Dlaczego hackowanie aplikacji webowych jest proste? Szkolenie od sekuraka](https://www.youtube.com/watch?v=2S15DyhTlsU)
- [Bezpieczeństwo Windows – czym jest LSASS dump. Jak się przed nim chronić?](https://sekurak.pl/bezpieczenstwo-windows-czym-jest-lsass-dump-jak-sie-przed-nim-chronic) Windows Security - what is LSASS dump and how to protect against it
- [The End of PPLdump | itm4n's blog](https://itm4n.github.io/the-end-of-ppldump/)
- [Signed driver malware moves up the software trust chain – Sophos News](https://news.sophos.com/en-us/2022/12/13/signed-driver-malware-moves-up-the-software-trust-chain/) BURNTCIGAR; signed driver; WinRing0; sc create; IoCreateDevice 
- [WMI for red and blue teams](https://www.fireeye.com/content/dam/fireeye-www/services/pdfs/sans-dfir-2015.pdf)
 

## Amateur Radio

- [Jak zostać krótkofalowcem? - HamNews.pl](https://hamnews.pl/jak-zostac-krotkofalowcem/) How to become a legal amateur radio user in Poland. Details about exams, tests.
- [Czestotliwosci - Pozwolenia Radiowe](https://czestotliwosci.pl.tl/Pozwolenia-Radiowe.htm) Important radio frequencies in Poland

## Oracle Cloud Free Tier resources

- [Oracle Cloud Free Tier](https://www.oracle.com/cloud/free/) <br/> #cloud/vps/shell/bash/linux
  Oracle gives totally for free a possibility to create a VPS linux machine, that you can manipulate using SSH. You can treat it as a development / testing environment.<br/>
  <img src="https://raw.githubusercontent.com/malpka/bookmarks/main/images/2023-01-21_161317.png" alt="Oracle img" width="200" onmouseover="this.width='400'" onmouseout="this.width='200'"/>
- [Darmowy serwer VPS ARM z 4 Rdzeniami, 24 GB RAM i 200 GB Dysk za darmo. | Pepper](https://www.pepper.pl/promocje/darmowy-serwer-vps-arm-z-4-procesorami-24-gb-ram-i-200-gb-pamieci-za-darmo-618087)
- [How to create a free Oracle VPS with Python script (Out of capacity)? - Tri Nguyen](https://www.hintdesk.com/2022/01/15/how-to-create-a-free-oracle-vps-with-python-script-out-of-capacity/) With Telegram notification
- [Github - automatic Oracle Free instance creator | chacuavip10/oci_auto](https://github.com/chacuavip10/oci_auto)
- [Opening port 80 on Oracle Cloud Infrastructure Compute node - Stack Overflow](https://stackoverflow.com/questions/54794217/opening-port-80-on-oracle-cloud-infrastructure-compute-node)
- [Ubuntu Manpage: netfilter-persistent - load, flush and save netfilter rule sets](https://manpages.ubuntu.com/manpages/xenial/man8/netfilter-persistent.8.html)
- [Getting started with Docker for Arm on Linux](https://www.docker.com/blog/getting-started-with-docker-for-arm-on-linux/)
- [Run the Docker daemon as a non-root user (Rootless mode)](https://docs.docker.com/engine/security/rootless/)

## Music 

-[10 Folk Metal Bands that Should be in Your Library in 2022 - MetalheadCommunity.com](https://metalheadcommunity.com/10-folk-metal-bands-that-should-be-in-your-library-in-2022/)


## Web development

- [Dribbble - Discover the World’s Top Designers & Creative Professionals](https://dribbble.com/) Inspiration for portfolio / logos / screens <br/><img src="https://cdn.dribbble.com/userupload/4399645/file/original-c92639d76a07ed953945f69303deb91a.png?compress=1&resize=400x300&vertical=top"/>


## Other

- [Z-Library Project - Electronic library. Download books free](https://z-lib.is/)

