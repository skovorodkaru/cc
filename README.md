# XDDOS: An Advanced Minecraft Server Stress Tester

<p>
XDDOS is a powerful tool that you can use to test your server's resilience against bots. It has many advanced features that make it a must-have for anyone who wants to ensure the stability and performance of their Minecraft server.
</p>

## Features
XDDOS has the following features:

- 54 different attack methods to choose from
- Supports all versions of Minecraft
- A proxy scraper that gets the latest proxies from a URL before each attack (just put the links to scrape proxy from in urls.txt)
- A user-friendly command-line interface (CLI) that eliminates the need for difficult-to-remember startup commands
- Startup commands
- Auto IP resolver, which means that you can use the server IP or domain
- ANSI color support for better visuals in terminal

## System Requirements

- XDDOS is compiled using Java 17, which means that you can use Java 17 or above to run it.
- To get versions protocols, go to [this page](https://wiki.vg/Protocol_version_numbers)


## How to run XDDOS
<ol>
  <li>Download the XDDOS jar from [here](https://github.com/AnAverageBeing/XDDOS/raw/master/XDDOS.jar)</li>
  <li>Create a folder to store XDDOS.jar in it.</li>
  <li>In that folder, create a text file and name it `urls.txt`.</li>
  <li>Put the links to scrape socks4 proxies from in that file. If you don't have any links, you can use the following ones:
  </li>
<p>
<code>
https://raw.githubusercontent.com/TheSpeedX/PROXY-List/master/socks4.txt
https://raw.githubusercontent.com/ShiftyTR/Proxy-List/master/socks4.txt
https://raw.githubusercontent.com/monosans/proxy-list/main/proxies/socks4.txt
https://raw.githubusercontent.com/jetkai/proxy-list/main/online-proxies/txt/proxies-socks4.txt
</code>
</p>
  <li>To open the terminal, first navigate to the folder where the XDDOS jar file is stored. You can do this by using the cd command in the terminal and specifying the folder path. For example, if the XDDOS jar file is stored in the Downloads folder, you can navigate to it by typing cd Downloads in the terminal. Alternatively, you can open the folder where the XDDOS.jar file is stored in file explorer, and then type cmd in the address bar at the top of the window. This will open a terminal window in that folder.</li>
  <li>Use one of the commands below to start XDDOS.</li>
</ol>

### Startup Command: 

- For user-friendly CLI/auto mode with colors:
```
java -jar XDDOS.jar
```
- For user friendly CLI/auto mode without colors:
```
java -jar XDDOS.jar -noansi
```

- for manual startup with colors:
```
java -jar XDDOS.jar [ip] [protocol] [method] [time] [netty threads] [loop threads] [y/n]
```
- for manual startup without colors:
```
java -jar XDDOS.jar [ip] [protocol] [method] [time] [netty threads] [loop threads] [y/n] -noansi
```

#### NOTE! :-
**y/n** is optional. Use `y` if you want to scrape proxy from links in urls.txt and **n** to use your own proxies from proxies.txt 

## Example Attack Commands  

- To run botjoiner for 10 seconds with 3 netty threads and 1 loop thread and use auto proxy generator:
```
java -jar XDDOS.jar localhost:25565 47 botjoiner 10 3 1 y
```

- To run botjoiner for 10 seconds with 3 netty threads and 1 loop thread and use your own proxy:
```
java -jar XDDOS.jar localhost:25565 47 botjoiner 10 3 1 n
```

- To run botjoiner for 10 seconds with 10 netty threads and 2 loop threads and use auto proxy generator:
```
java -jar XDDOS.jar localhost:25565 47 botjoiner 10 10 2 y
```


## Methods avilable

- BigHandshake
- BigPacket
- BotJoiner
- BotRiad
- BungeeDowner
- ChatSpam
- ColorCrasher
- CpuDowner
- DoubleJoin
- EmptyNames
- EmptyPacket
- ExtremeJoin
- ExtremeKiller
- Handshake
- InstantDowner
- InvalidData
- InvalidNames
- InvalidSpoof
- IpSpooffFlood
- Join
- LegacyPing
- LegitnameJoin
- LocalHost
- LongHost
- LongNames
- Memory
- MOTD
- nAntiBot
- NettyDowner
- Network
- NewNullping
- NullPing
- Ping
- PingJoin
- Query
- Queue
- QuitExceptions
- RAM
- RandomExceptions
- RandomPacket
- ServerFucker
- Slapper
- SmartBot
- Spoof
- TCPBypass
- TCPHit
- UltimateKiller
- UltimateSmasher
- UnexpectedPacket
- uuidCrash
- WaterfallBypass
- XDJoin
- XDSpam


## FAQ:
### The colours are bugged
Use -noansi at the end of the command or try using another terminal like Windows Terminal

### XDDOS has a discord?
Yes. You can join [here](https://dsc.gg/TEAMXD)
