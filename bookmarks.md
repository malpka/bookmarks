# January 2023

## Cloud

- [Oracle Cloud Free Tier](https://www.oracle.com/cloud/free/) <br />
#cloud/vps/shell/bash/linux
Oracle gives totally for free a possibility to create a VPS linux machine, that you can manipulate using SSH. You can treat it as a development / testing environment.<br/>
<img src="https://raw.githubusercontent.com/malpka/bookmarks/main/images/2023-01-21_161317.png" alt="Oracle img" width="200" onmouseover="this.width='400'" onmouseout="this.width='200'"/>

## Programming

### Python

- [Python 3 Expressions](https://docs.python.org/3/reference/expressions.html) - 
#python3/python/programming
<br/>
Very helpful reference for magic things that you can do on your beginners journey using python, like
<br/>
`[x*y  for  x  in  range(10)  for  y  in  range(x,  x+10)]`.
```
def f(a, b):
...     print(a, b)
...
>>> f(b=1, *(2,))
2 1
```
BTW, If you ask - what is difference between `__str__` and `__repr__`? 
The str function is supposed to return a user friendly format, which is good for logging or to display some information about the object. And the __repr__ function is supposed to return an “official” string representation of the object, which can be used to construct the object again.
```
>>> import datetime
>>> now = datetime.datetime.now()
>>> now.__str__()
'2023-01-21 16:28:00.324317'
>>> now.__repr__()
'datetime.datetime(2023, 1, 21, 16, 28, 0, 324317)'
```

- [Python dictionary](https://www.tutorialspoint.com/python/python_dictionary.htm) - 
#python3/python/programming
<br/>
Methods to operate on python dictionary, and answers to questions like: when I should use dict.get("key") instead of dict["key"] 

- [The Python heapq Module: Using Heaps and Priority Queues](https://realpython.com/python-heapq-module/) #python3/python/programming

### .NET

- [Tutorial: Create a web API with ASP.NET Core](https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-5.0&tabs=visual-studio#add-a-database-context) 
Step by step official tutorial by Microsoft
- [Dependency injection in .NET](https://learn.microsoft.com/en-us/dotnet/core/extensions/dependency-injection#service-lifetimes) Important topic overall, and good thing to remember about Service Lifetime
- [Migration to ASP.NET Core in .NET 6](https://gist.github.com/davidfowl/0e0372c3c1d895c3ce195ba983b1e03d) -
by David Fowler
- [Bezpieczeństwo danych: aplikacja multi tenant .Net Core api](https://geek.justjoin.it/bezpieczenstwo-danych-aplikacja-multi-tenant-net-core-api/)
- [Tutorial: Create a web API with ASP.NET Core - Official guide by Microsoft](https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-5.0&tabs=visual-studio#add-a-database-context)
- [Various goodies from Dotnetos!](https://goodies.dotnetos.org/) .NET diagnostics, .NET async, .NET memory, SDRAM Anatomy Poster, .NET GC Tips & Tricks series slides, .NET GC Internals series slides, .NET in Pictures


## Bots

- [Bots for automated search for free timeslot for medical appointment](https://github.com/search?q=cov19.moderna&type=code)

## Jobs

- [Oferty pracy IT - Kariera z Diverse CG](https://dcg.pl/karierawit)
- [IT recruitment agency in Poland – RemoDevs](https://remodevs.com/)
- [Praca w IT TeamQuest](https://teamquest.pl/praca-zdalna/54820-praca-senior-net-engineer)

## Games

- [The most popular games on Epic Game Store](https://store.epicgames.com/en-US/collection/most-popular)<br/>
Currently list looks like below:<br/>
    1. Grand Theft Auto V: Premium Edition
    2. VALORANT
    3. NARAKA: BLADEPOINT
    4. Red Dead Redemption 2
    5. Bloons TD 6
    6. EA SPORTS™ FIFA 23 Standard Edition
    7. Among Us
    8. Gamedec - Definitive Edition
    9. Dishonored - Definitive Edition
    10. League of Legends

## Investing

- [4 Common Active Trading Strategies](https://www.investopedia.com/articles/active-trading/11/four-types-of-active-traders.asp)
  -   [1. Day Trading](https://www.investopedia.com/articles/active-trading/11/four-types-of-active-traders.asp#toc-1-day-trading)
  -   [2. Position Trading](https://www.investopedia.com/articles/active-trading/11/four-types-of-active-traders.asp#toc-2-position-trading)
  -   [3. Swing Trading](https://www.investopedia.com/articles/active-trading/11/four-types-of-active-traders.asp#toc-3-swing-trading)
  -   [4. Scalping](https://www.investopedia.com/articles/active-trading/11/four-types-of-active-traders.asp#toc-4-scalping)

## Software

- [VeraCrypt](https://documentation.help/VeraCrypt/Command%20Line%20Usage.html)
Full disk encryption software, replacement for TrueCrypt, which has been compromised.
# February 2023

## AI

- [OpenAI Products](https://openai.com/product) ChatGPT, DALL·E, Whisper

### Midjourney

- [Logo Design with Midjourney – AI Create Logo | Weird Wonderful AI Art](https://weirdwonderfulai.art/general/logo-design-with-midjourney-ai-create-logo/) <img src="https://weirdwonderfulai.art/wp-content/uploads/2022/09/logo-design-post-940x675.jpg"/>

## NAS

- [-Die sparsamsten Systeme (<30W Idle)- - Arkusze Google](https://docs.google.com/spreadsheets/d/1LHvT2fRp7I6Hf18LcSzsNnjp10VI-odvwZpQZKv_NCI/edit#gid=0) List of PC sets with low power consumption, ideal for DIY NAS
- [Cheap, Low power NAS build with 5x3,5 hdd - New Builds and Planning - Linus Tech Tips](https://linustechtips.com/topic/1477129-cheap-low-power-nas-build-with-5x35-hdd/#comment-15722949) Description of one of the sets based on Fujitsu box
- [The Free Software Media System | Jellyfin](https://jellyfin.org/) Jellyfin is the volunteer-built media solution that puts you in control of your media. Stream to any device from your own server, with no strings attached. Your media, your server, your way.

## Home automation

- [Node-RED](https://nodered.org/) Node-RED is a programming tool for wiring together hardware devices, APIs and online services in new and interesting ways. It provides a browser-based editor that makes it easy to wire together flows using the wide range of nodes in the palette that can be deployed to its runtime in a single-click.
- [Raspberry Pi – Zdalne sterowanie przy pomocy dataplicity – Starter Kit](https://starter-kit.nettigo.pl/2018/03/raspberry-pi-zdalne-sterowanie-przy-pomocy-dataplicity/)
- [Zigbee - jaką bramkę wybrać? Ogromne możliwości zamknięte standardy. - HejDom](https://hejdom.pl/blog/20-testy-porownawcze/131-zigbee-jaka-bramke-wybrac-ogromne-mozliwosci-zamkniete-standardy.html)
- [Home Assistant - Zigbee2MQTT (CC2531) - konfiguracja - HejDom](https://hejdom.pl/blog/22-home-assistant/96-home-assistant-zigbee2mqtt-cc2531-za-4-i-programowanie-przez-nodemcu.html)

## Web Scrapping 

- [How to detect, block and manage DataDome | by campo | Medium](https://medium.com/@campo1312/how-to-detect-block-and-manage-datadome-c6e94c74a4f4) In this article I will show you what my research on the new antibot called DataDome led me to. This tutorial is for informational purposes only. I guess you’ll add the code to your scripts, go ahead but quote me, thanks.
- [campo1312/DataDome: How to detect, block and manage DataDome.](https://github.com/campo1312/DataDome)


## Applications

- [PowerToys Video Conference Mute utility for Windows | Microsoft Learn](https://learn.microsoft.com/en-us/windows/powertoys/video-conference-mute)<br/><img src="https://learn.microsoft.com/en-us/windows/images/pt-vcm-source-in-app.png"/>
    - ⊞ Win+Shift+Q to toggle both audio and video at the same time
    - ⊞ Win+Shift+A to toggle microphone
    - ⊞ Win+Shift+O to toggle camera

## System tools

- [Can Windows tell me what is using my USB drive? - Super User](https://superuser.com/questions/87364/can-windows-tell-me-what-is-using-my-usb-drive)
    - [Sysinternals Process Explorer](http://technet.microsoft.com/en-us/sysinternals/bb896653.aspx)
    - [PowerToys File Locksmith utility for Windows | Microsoft Learn](https://learn.microsoft.com/en-us/windows/powertoys/file-locksmith)<br/><img src="https://learn.microsoft.com/en-us/windows/images/powertoys-file-locksmith.gif"/>
    - &gt; `wevtutil qe System /q:"*[System[(EventID=225)]]" /c:5 /f:text /rd:true`
    - PS&gt; `Get-EventLog -LogName System -after (Get-Date).AddHours(-1) | Where-Object {$_.EventID -eq 225} | Sort-Object TimeGenerated | Format-Table -Wrap`
    - PS&gt; `Get-WinEvent -MaxEvents 5 -FilterHashtable @{LogName='System';Id=225} | Format-Table -Wrap`

## Games

### Vermintide 2

- [Społeczność Steam :: Poradnik :: 【Updated to Patch 4.8】【All Careers】Legend Builds Collection](https://steamcommunity.com/sharedfiles/filedetails/?id=2034609078)
- [Społeczność Steam :: Poradnik :: 【Updated to Patch 4.8】How to optimize your gameplay with Bots](https://steamcommunity.com/sharedfiles/filedetails/?id=2068782454)
- [Piercing Waystalker - Waystalker Kerillian Build - Vermintide 2 | ranalds.gift](https://www.ranalds.gift/build/AKvHk8Q9QeqwZABmvtuH/view)
- [Momentum Slayer - Ranalds Gift](https://www.ranalds.gift/build/VJqdOmkXogqC9gnCqF4h/view)


## Lifestyle

- [Scarbir - Wireless Earphones Reviews](https://www.scarbir.com/) Honest reviews on true wireless earbuds under $100

## Jobs

- [Find DevOps Engineer Jobs with JobServe.com](https://www.jobserve.com/gb/en/JobListing.aspx?shid=512A9AA37511B776451B&q=DevOps%20Engineer&lq=England&src=51784C66D7&js=1)
- [talentify.io](https://affirm.talentify.io/job/staff-software-engineer-backend-purchasing-poland-maine-affirm-5272265003)
- [Jobs at Affirm](https://boards.greenhouse.io/affirm)

## Programming

- [nbedos/termtosvg: Record terminal sessions as SVG animations](https://github.com/nbedos/termtosvg) termtosvg is a Unix terminal recorder written in Python that renders your command line sessions as standalone SVG animations.<img src="https://github.com/nbedos/termtosvg/raw/develop/docs/examples/awesome_window_frame_powershell.svg">

### .NET

- [bflat - C# as you know it but with Go-inspired tooling (small, selfcontained, and native executables)](https://flattened.net/) bflat is a native compiler for C# that comes with everything you need to build C# apps for any of the supported platforms. No additional SDKs or NDKs needed.
    - Run C# with no operating system, on bare metal
    - Build native code or .NET bytecode

#  2023

## Applications

## System tools

## Games

### Vermintide 2

## Lifestyle

## AI

### Midjourney

### Chat-GPT


## NAS

## Home automation

## Web Scrapping 

## Jobs

## Programming

### .NET
