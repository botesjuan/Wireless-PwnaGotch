# Wireless PwnaGotch Notes  

>This is quick few notes on using and connecting the Pwnagotchi to Windows and having it collecting wireless handshake authentication traffic for cracking with HashCat.

>Follow this video to setup and collect handshakes: [NetworkChuck Raspberry Pi Zero PwnAgothci Project](https://youtu.be/km81ph7pZz8?si=q5tOOcU6wzzCM3II&t=774)

>The original instructions for the project: [Pwnagotchi Project](https://pwnagotchi.ai/intro/) powered by [bettercap](https://www.bettercap.org/)  

>After raspberry pi zero been running in evironment capturing wireless handshakes the location of PCAP files stored All the handshakes Pwnagotchi captures are saved to `/root/handshakes/`.

## Connecting to Windows  

1. Connect with data usb cable to the usb port on Pi zero to Windows Desktop USB port.
2. Device Manager select COM PORT and update RNDIS drivers from [Windows 10 RNDIS drivers](https://modclouddownloadprod.blob.core.windows.net/shared/mod-rndis-driver-windows.zip)
3. Set IP address under networking RNDIS TCP/IP 4 to `10.0.0.1` as the Raspberry pi is set to `10.0.0.1`.
4. Use browser and connect `http://10.0.0.2:8080` with user name of `admin:admin`
5. From windows command line connect as ssh to raspberry pi `ssh pi@10.0.02` with default password as `raspberry`



