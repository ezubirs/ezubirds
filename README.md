# My Proxy Bot ([@By123bot](http://t.me/By123bot))
* [By123bot](http://t.me/By123bot) -- full-featured Bot-In-The-Middle for Telegram.
* [Ezadin jemal](http://t.me/ezubirdsbot) -- webhook version on Flask.
* [Merryzedo](http://t.me/merryzedo) -- botfabric creating ProxyBots for Telegram users.

## Proxy Bot
You can use it as your second account. 
Start it and share its username. Others will be able to contact you using this bot without the risk of being reported for spam (you can block them though). And you will be able to answer them without the risk for you! (Telegram's spam report system is kinda broken).

### Features

#### Message Log
The bot stores full message history and allows you to review it.

#### Rich messages
The bot is able to recieve from users and resend from an admin all types of Telegram messages.

#### Customization
The bot forces you to set all the special messages for your users. It will be using them later for autoreply.

* Start message -- autoreply on `/start` command
```
Hello there! Write me to contact Admin.
```
* Block message -- autoreply to blocked users
```
Oops, you were blocked. Sorry!
```
* Unavailable message -- autoreply to users' messages. It is sent when admin was not showing up for last hour. Should notify user that his message is properly delivered, but bot cant guarantee fast reply from admin.
```
Thank you! It might take a while...
```

### Thanks
The original idea and the very first version of `proxybot` are came from [By123bot](http://t.me/By123bot).
Some extra features came from the repo it was forked from: [By123bot](http://t.me/By123bot)'s patched version.

## Webhook Proxy bot
Flask app for webhook version of [ProxyBot](#proxy-bot). Nothing supercool, though..

## Webhook Master bot
Flask app that is a special bot that can spawn webhook version of [By123bot](http://t.me/By123bot) for every telegram user. 

## Prerequisites
* Python 3 (works only with Python3);
* [By123bot](http://t.me/By123bot) library (with bot 2.0 support);
* Flask (optional for webhook versions)

## Remember!
I understand, that "proxy" bots can be used to prevent spammers from being reported, so if you encounter such bots that are used to do "bad" things, feel free to report them: [By123bot](http://t.me/By123bot)

## F.A.Q
#### 1. Will this bot work in groups/supergroups/channels?
The ProxyBot works only in private chats because it would be a big load on db to store all messages in couple busy groups. And it would be spammy.
It can work in group chats, but to enable this feature you need to obtain your own copy of repo, comment out one function in `proxy_bot.py` and run either it or webhook version.

#### 2. Can I use Emojis in my saved messages (start, block and unavailable)?
For now you can only use emojis in pre-saved messages.

#### 3. Can I add more admins?
No, the bot work for only single Telegram account.

## Contact
You can contact me via my [By123bot](http://t.me/By123bot).
