# XDDOS, an advanced minecraft server stresser

XDDOS is an advanced tool for attacking and testing your server against bots.

## Features avilable

XDDOS has the following features:

- 54 different attack methods
- Supports all versions 
- proxy scraper that gets latest proxies from url before each attack (just put the links to scrape proxy from in urls.txt)
- user friendly CLI dont worry about hard to remeber startup commands
- Startup commands 
- Auto ip resolver. That means that you can use the server IP or the domain
- Ansi Colours supported

## How to use XDDOS

### Things to know

- About netty and loop threads
**NETTY THREDS** those are threds that netty use in its event loop group if u dont know what to put
               just put (no. of threads in ur system / 2) netty threads
**Loop Thread** it request bootstrap to connect to server. 
If u dont know what to put try 1 or 2
- Jar is compiled used java 17. That means that you an use java 17 or above to run XDDOS
- To get versions protocols go [here](https://wiki.vg/Protocol_version_numbers)

### Steps to take to run XDDOS:
 1) Download the jar -> [Download](https://github.com/AnAverageBeing/XDDOS/raw/master/XDDOS.jar)
 2) Create a folder to store XDDOS
 3) Now make a file called urls.txt in that folder
 4) Put the links to scrape socks4 proxies from in that file
   #### If you don't have links to scrape proxy from here are some
   <br>
  just put these in url.txt and enjoy
  
  ```
  https://raw.githubusercontent.com/TheSpeedX/PROXY-List/master/socks4.txt
  https://raw.githubusercontent.com/ShiftyTR/Proxy-List/master/socks4.txt
  https://raw.githubusercontent.com/monosans/proxy-list/main/proxies/socks4.txt
  https://raw.githubusercontent.com/jetkai/proxy-list/main/online-proxies/txt/proxies-socks4.txt
  ```
  
 5) Now open your terminal and go to the directory (you can write `cmd` in the folder path of where xddos.jar is and the terminal will open in that folder)
 6) Now use one of the commands below for starting

### Startup Command: 

- For user friendly CLI/auto mode with colors:
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
