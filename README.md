<div align="center" width="100%">
    <img src="./public/icon.svg" width="128" alt="" />
</div>

# Uptime Kuma

Uptime Kuma is an easy-to-use self-hosted monitoring tool.

## 🥔 Live Demo

Try it!

- Tokyo Demo Server: https://demo.uptime.kuma.pet

It is a temporary live demo, all data will be deleted after 10 minutes. Use the one that is closer to you, but I suggest that you should install and try it out for the best demo experience.

## ⭐ Features

* Monitoring uptime for HTTP(s) / TCP / HTTP(s) Keyword / HTTP(s) Json Query / Ping / DNS Record / Push / Steam Game Server / Docker Containers
* Fancy, Reactive, Fast UI/UX
* Notifications via Telegram, Discord, Gotify, Slack, Pushover, Email (SMTP), and [90+ notification services, click here for the full list](https://github.com/louislam/uptime-kuma/tree/master/src/components/notifications)

## 🔧 How to Install


### 💪🏻 Non-Docker

Requirements:
- Platform
  - ✅ Major Linux distros such as Debian, Ubuntu, CentOS, Fedora and ArchLinux etc.
  - ✅ Windows 10 (x64), Windows Server 2012 R2 (x64) or higher
  - ❌ Replit / Heroku
- [Node.js](https://nodejs.org/en/download/) 14 / 16 / 18 / 20.4
- [npm](https://docs.npmjs.com/cli/) >= 7
- [Git](https://git-scm.com/downloads)
- [pm2](https://pm2.keymetrics.io/) - For running Uptime Kuma in the background

```bash
# Update your npm
npm install npm@9 -g

git clone https://github.com/louislam/uptime-kuma.git
cd uptime-kuma
npm run setup

# Option 1. Try it
node server/server.js

# (Recommended) Option 2. Run in the background using PM2
# Install PM2 if you don't have it:
npm install pm2 -g && pm2 install pm2-logrotate

# Start Server
pm2 start server/server.js --name uptime-kuma


```
Uptime Kuma is now running on http://localhost:3001

More useful PM2 Commands

```bash
# If you want to see the current console output
pm2 monit

# If you want to add it to startup
pm2 save && pm2 startup
```

## 🖼 More Screenshots

Light Mode:

<img src="https://uptime.kuma.pet/img/light.jpg" width="512" alt="" />

Status Page:

<img src="https://user-images.githubusercontent.com/1336778/134628766-a3fe0981-0926-4285-ab46-891a21c3e4cb.png" width="512" alt="" />

Settings Page:

<img src="https://louislam.net/uptimekuma/2.jpg" width="400" alt="" />

Telegram Notification Sample:

<img src="https://louislam.net/uptimekuma/3.jpg" width="400" alt="" />
