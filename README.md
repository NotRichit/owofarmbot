dWdnY2Y6Ly9iY3JhLmZjYmd2c2wucGJ6L2dlbnB4LzVwc2tIZ1B4Y3hQVkVlWGxxVVhGb1kgcm90MTM= </br>
6 28 15 26 15<br> {/\_\_/}</br>( • . •)</br>/ > 🤍

If you make a video about using the farmbot, upload it to YouTube with the hashtag #thankumid0 and let me know.

<h1 align="center">OwO Farm Bot V1.0.6.7</h1>

<p align="center">

<a href="https://github.com/Mid0aria/owofarmbot"><img src="https://hits.sh/github.com/Mid0aria/owofarmbot.svg?view=today-total&label=Repo%20Today/Total%20Views&color=770ca1&labelColor=007ec6"/></a>
<a href="https://github.com/Mid0aria/owofarmbot"><img src="https://img.shields.io/github/last-commit/mid0aria/owofarmbot" /></a><br>
Tutorial needed? (PC) <a href="https://youtu.be/sso05qx8Hac">Click Here</a><br>
~~Tutorial 2 (replit) <a href="https://www.youtube.com/watch?v=tiSd99NEhb4">Click Here</a> (Thanks Hiếu LoneLy)~~(no longer works due to replit's measures against selfbots)<br>
Tutorial 3 (TERMUX) <a href="https://www.youtube.com/watch?v=78XrZgDtEXU">Click Here</a> (Thanks OwO Sever)<br>
Tutorial 4 (Termux) [Click Here](#-termux-installation)
Need midoservices_authkey or Need Help? <a href ="https://discord.gg/WzYXVbXt6C">Join Discord Server</a>

</p>

# Contents

[⭐・Star History](#star-history)<br>
[❗・Important](#important)<br>
[👑・Features](#features)<br>
[⚙・Config.json example](#configjson-example)<br>
[⚙・.env example](#dotenv-example)<br>
[💎・Get Token](#get-token)<br>
[📍・OwO DM channel id](#owo-dm-channel-id)<br>
[📚・Discord RPC](#discord-rpc)<br>
[⚠️・Captcha Alert](#captcha-alert)<br>
[📡・Socket Client](#socket-client)<br>
[🔗・Required Links](#required-links)<br>
[🎈・Installation](#Installation)<br>
[🚀・Termux Installation](#-termux-installation)<br>
[🥰・Thanks for contribution](#thanks-for-contribution)<br>

## ⭐・Star History

<h2 align="center">Goal: <a href="https://github.com/Mid0aria/owofarmbot/stargazers"><img src="https://img.shields.io/github/stars/Mid0aria/owofarmbot" /></a> / 512</h2>
⭐⭐⭐ You can also give this repository a star to show more people and they can use this repository<br>

[![Star History Chart](https://api.star-history.com/svg?repos=Mid0aria/owofarmbot,mid0aria/owofarmbot_ui&type=Date)](https://star-history.com/#Mid0aria/owofarmbot&mid0aria/owofarmbot_ui&Date)

## ❗・Important (Anyone using the bot is deemed to have read and accepted these)

-   We would like to point out that long-term use of farm bots may result in a ban from owo and we do not accept responsibility.
-   Discord may restart as a result of discord rpc overload.
-   It can detect virus due to captcha(ban) bypasser please turn off your antivirus.
-   DO NOT USE ONE CHANNEL FOR TWO ACCOUNTS, USE IT FOR 1 ACCOUNT ONLY
-   We use a diagnostic report system to understand and correct errors in the farmbot. The information we keep on our servers:
    -   userkey
    -   project name
    -   systeminformation (system, osInfo, uuid, versions, cpu (we get this datas from the "systeminformation" library))
    -   report (error log)

## 👑・Features

-   Auto Hunt
-   Auto Battle
-   Inventory Check
    -   Auto Gem Use (beta)
    -   Auto Lootbox Use
    -   Auto Fabled Lootbox Use
    -   Auto Crate Use
    -   Auto Eventbox Use (like anniversary present or valentine's day)
-   Auto Gamble
    -   Auto Coinflip
    -   Auto Slots
-   Auto Animals Sell OR Sacrifice,
-   Auto Upgrade Autohunt
-   Auto Pray
-   Auto CheckList (beta)
    -   Auto Quest
    -   Auto Daily
    -   Auto Cookie
-   Captcha(Ban) Protection v0.1.8 (beta)
-   Discord-RPC
-   Typing Indicator
-   **Extra Token**
    -   All Main Token Features
    -   Auto Pray for Main Token

## ⚙・config.json example

```
{
    "midoservices_authkey": "", / Enter ur midoservices auth key. If you don't have one, join the discord server and get one now.
    "windowssettings": { "controlcdetect": false },
    "settings": {
        "times": {
            "enable": "", true or false
            "huntbottom": 11000,  / The time to be entered must be entered in milliseconds. Minimum time to run hunt command.
            "hunttop": 16000, / The time to be entered must be entered in milliseconds. Maximum time to run hunt command.
            "battlebottom": 10000,  / The time to be entered must be entered in milliseconds. Minimum time to run battle command.
            "battletop": 16000, / The time to be entered must be entered in milliseconds. Maximum time to run battle command.

            "intervals": {
                "huntbattle": {
                    "enable": true, true or false
                    "time": 17000  / The time to be entered must be entered in milliseconds.
                },
                "animals": {
                    "enable": true, true or false
                    "time": 1200000  / The time to be entered must be entered in milliseconds.
                },
                "pray": {
                    "enable": true, true or false
                    "time": 303000  / The time to be entered must be entered in milliseconds.
                },
                "curse": {
                    "enable": true, true or false
                    "time": 303500  / The time to be entered must be entered in milliseconds.
                },
                "upgrade": {
                    "enable": true, true or false
                    "time": 1205000  / The time to be entered must be entered in milliseconds.
                },
                "gamble": {
                    "enable": true, true or false
                    "coinflip": {
                        "time": 25000  / The time to be entered must be entered in milliseconds.
                    },
                    "slots": {
                        "time": 23000  / The time to be entered must be entered in milliseconds.
                    }
                }
            }
        },
        "prefix": "", owo bot's prefix on your server
        "huntandbattle": "", true or false
        "banbypass": "", true or false
        "discordrpc": "", true or false
        "typingindicator": "", true or false
        "pray": "", true or false
        "extratoken": "", true or false
        "autoquest": "", true or false
        "inventory": {
            "inventorycheck": "", true or false
            "gemcheck": "", true or false
            "lootboxcheck": "", true or false
            "fabledlootboxcheck": "", true or false
            "cratecheck": "", true or false
            "eventcheck": "" true or false
        },
        "animals": {
            "enable": "", true or false
            "type": "" sell or sacrifice
            "animaltype": {
                "common": "", true or false
                "uncommon": "", true or false
                "rare": "", true or false
                "epic": "", true or false
                "mythical": "", true or false
                "patreon": "", true or false
                "cpatreon": "", true or false
                "legendary": "", true or false
                "gem": "", true or false
                "bot": "", true or false
                "distorted": "", true or false
                "fabled": "", true or false
                "special": "", true or false
                "hidden": "" true or false
            }
        },
        "upgradeautohunt": {
            "enable": "", true or false
            "type": "" efficiency, duration, cost, gain, exp or radar
        },
        "gamble": {
            "coinflip": {
                "default_amount"= , Enter the amount you want to start from
                "max_amount": 250000, Enter the amount where the bot will not bet more than that
                "multipler": , Enter a number by which the lost amount will be multipled by
                "enable": "", true or false
                "amount": "1"
            },
            "slots": {
                "enable": "", true or false
                "amount": "1"
            }
        }
    },
    "main":{
        "token":"", main token (if you use replit please edit .env file)
        "userid":"", token user id
        "channelid":"", channel id for main token
        "owodmchannelid":"", owo bot dm channel id
        "gamblechannelid":"", channel if for gambling
        "autoquestchannelid":"" auto quest channel id
    },
    "extra":{
        "token":"", extra token (if you use replit please edit .env file)
        "userid":"", extra token user id
        "channelid":"", channel id for extra token
        "gamblechannelid":"", channel if for gambling
        "owodmchannelid":"" extra token owo bot dm channel id
    }
}


```

## ⚙・dotenv example

If you use replit, you must enter your tokens in the .env file for the security of your tokens!

```
MAIN_TOKEN=mysupermaintokenblabla
EXTRA_TOKEN=mysuperextratokenblabla
```

## 💎・Get Token
### PC
1. Open Chrome and login to discord.com/app
2. Press CTRL + Shift + i and then click console
3. Paste the following code
4. The string provided will be your token.
```js
(webpackChunkdiscord_app.push([
    [""],
    {},
    (e) => {
        m = [];
        for (let c in e.c) m.push(e.c[c]);
    },
]),
m)
    .find((m) => m?.exports?.default?.getToken !== void 0)
    .exports.default.getToken();
```
### Mobile/Android
1. Open chrome
2. Create a bookmark (by clicking on star button in 3 dots menu)
3. Edit it and set name to token finder and url to the following code:
   ```javascript
   javascript: (webpackChunkdiscord_app.push([    [""],    {},    (e) => {        m = [];        for (let c in e.c) m.push(e.c[c]);    },]),m)    .find((m) => m?.exports?.default?.getToken%20!==%20void%200)%20%20%20%20.exports.default.getToken();
   ```
4. Open Discord.com/app (website) and log in.
5. Tap on search bar and type token Finder (don't search it just type)
6. A Star Icon with Name Token Fonder will appear
7. Click on that
8. A new page will open , the string in the page will be your token.
## 📍・OwO DM channel id

![](https://raw.githubusercontent.com/Mid0aria/owofarmbot/main/images/owochannelid.jpg)

## 📚・Discord RPC

![](https://raw.githubusercontent.com/Mid0aria/owofarmbot/main/images/rpc.jpg)

## ⚠️・Captcha Alert

!!! If you want the captcha alert to work properly, turn off do not disturb

![](https://raw.githubusercontent.com/Mid0aria/owofarmbot/main/images/captchaalert.png)

## 📡・Socket Client

![](https://raw.githubusercontent.com/Mid0aria/owofarmbot/main/images/socketclient.png)
Only works on **windows** using **Terminal**
## 🔗・Required Links

[NodeJS](https://nodejs.org/en/)<br>
[Terminal](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701)<br>
[Farm Bot Zip File](https://github.com/Mid0aria/owofarmbot/archive/refs/heads/main.zip)

## 🎈・Installation

```
> YOU NEED LATEST NODEJS !
> download zip file or run git clone https://github.com/Mid0aria/owofarmbot.git
> edit config.json
```

```bash
$ cd owofarmbot
$ npm install (only in the first installation)
$ node bot.js
```

## 🚀・ Termux Installation

```bash
> Install

$ apt update -y && apt upgrade -y && pkg install wget
$ wget https://raw.githubusercontent.com/mid0aria/owofarmbot/main/termux-setup.sh
$ sh termux-setup.sh

> Edit config.json:

$ cd owofarmbot
$ nano config.json
```

## 🥰・Thanks for contribution

VihaanReddyM <a href="https://github.com/VihaanReddyM">(Github)</a><br>
Random-629671 <a href="https://github.com/Random-629671">(Github)</a><br>
Le-Khuong <a href="https://github.com/Le-Khuong">(Github)</a><br>
mallusrgreatv2 <a href="https://github.com/mallusrgreatv2">(Github)</a><br>
Le-Khuong <a href="https://github.com/Le-Khuong">(Github)</a><br>
NotRichit <a href="https://github.com/NotRichit">(Github)</a><br>
Hiếu LoneLy <a href="https://www.youtube.com/watch?v=tiSd99NEhb4">(Youtube)</a><br>
OwO Sever <a href="https://www.youtube.com/watch?v=78XrZgDtEXU">(Youtube)</a>
