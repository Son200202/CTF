<h1 align= center><b>⭐️ Binary Exploitation CTF ⭐️</b></h1>
<h3 align = center> Nơi lưu lại quá trình khai thác binary exploitation trên picoctf và demo lại quá trình tạo đề, giải đề, cách nhận flag của một bài ctf </h3>
<p align="center">
<a href="https://www.kali.org/"><img src="https://www.bleepstatic.com/content/hl-images/2020/01/03/Kali_Linux_4.jpg" width="200" height="80" alt="made-with-c"></a>
</p>

## ✨ <a name="features"></a>Exploit picoctf

### ⚡ Buffer overflow 0
Starts streaming your inputs while downloading and converting them. Also, it
doesn't make produce files.
### 👮🏻‍♀️ Buffer overflow 1
Restricts control and sensitive commands to admins.
### 🗑 Buffer overflow 2
Deletes old playing trash to keep your chats clean.
### 😎 Two sum
Lets you switch stream mode, loop, pause, resume, mute, unmute anytime.
### 🖼 RPS
Response your commands with cool thumbnails on the chat.
### 😉 Function overwrite
You can stream audio or video files, YouTube videos with any duration,
YouTube lives, YouTube playlists and even custom live streams like radios or m3u8 links or files in
the place it is hosted!
### 📊 Tictac
Allows you to stream different things in multiple chats simultaneously. Each
chat will have its own song queue.

## ✨ <a name="features"></a>Demo
### 🗣 Speaks different languages
Music Player is multilingual and speaks [various languages](#languages),
thanks to the translators.
## 🚀 <a name="deploy"></a>Deploy
[![Deploy on Heroku](https://www.herokucdn.com/deploy/button.svg)](https://deploy.safone.tech)
Note: `First Fork The Repo Then Click On Deploy To Heroku Button!`
## ☁️ <a name="self_host"></a>Self Host
- Legecy Method
```bash
$ git clone https://github.com/AsmSafone/MusicPlayer
$ cd MusicPlayer
$ sudo apt install git curl python3-pip ffmpeg -y
$ pip3 install -U pip
$ curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -
$ sudo apt install -y nodejs
$ sudo apt install build-essential
$ sudo npm install pm2@latest -g
$ pip3 install -U -r requirements.txt
$ cp sample.env .env


# < edit .env with your own values >
$ python3 main.py
```
Or you can use this One-Liner to save your time :
```
git clone https://github.com/AsmSafone/MusicPlayer && cd MusicPlayer && sudo apt install git curl python3-pip ffmpeg -y && pip3 install -U pip && curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash - && sudo apt install -y nodejs && sudo apt install build-essential && sudo npm install pm2@latest -g && pip3 install -U -r requirements.txt
```
Make sure to edit the .env file accordingly,
```
cp sample.env .env
```
Run it using,
```
python3 main.py
```
- Docker Build Method
```bash
$ git clone https://github.com/AsmSafone/MusicPlayer
$ cd MusicPlayer
$ cp sample.env .env
# < edit .env with your own values >
$ sudo docker build . -t musicplayer
$ sudo docker run musicplayer
```
## ⚒ <a name="configs"></a>Configs
- `API_ID`: Telegram app id from https://my.telegram.org/apps.
- `API_HASH`: Telegram app hash from https://my.telegram.org/apps.
- `SESSION`: Pyrogram string session. You can generate from [here](https://replit.com/@AsmSafone/genStr).
- `SUDOERS`: ID of sudo users (separate multiple ids with space).
- `BOT_TOKEN`: Telegram bot token from https://t.me/botfather. (optional)
- `QUALITY`: Custom stream quality (high/medium/low) for the userbot in vc. Default: `high`
- `PREFIX`: Bot commad prefixes (separate multiple prefix with space). Eg: `! /`
- `LANGUAGE`: An [available](#languages) bot language (can change it anytime). Default: `en`
- `STREAM_MODE`: An stream mode like audio or video (can change it anytime). Default: `audio`
- `ADMINS_ONLY`: Put `True` if you want to make /play commands only for admins. Default: `False`
- `SPOTIFY_CLIENT_ID`: Spotify client id get it from [here](https://developer.spotify.com/dashboard/applications). (optional)
- `SPOTIFY_CLIENT_SECRET`: Spotify client secret get it from [here](https://developer.spotify.com/dashboard/applications). (optional)
## 📄 <a name="commands"></a>Commands
Command | Description
:--- | :---
• !ping | Check if alive or not
• !start / !help | Show the help for commands
• !mode / !switch | Switch the stream mode (audio/video)
• !p / !play [song name or youtube link] | Play a song in vc, if already playing add to queue
• !radio / !stream [radio url or stream link] | Play a live stream in vc, if already playing add to queue
• !pl / !playlist [playlist link] | Play the whole youtube playlist at once
• !skip / !next | Skip to the next song
• !m / !mute | Mute the current stream
• !um / !unmute | Unmute the muted stream
• !ps / !pause | Pause the current stream
• !rs / !resume | Resume the paused stream
• !list / !queue | Show the songs in the queue
• !mix / !shuffle | Shuflle the queued playlist
• !loop / !repeat | Enable or disable the loop mode
• !lang / language [language code] | Set the bot language in group
• !ip / !import | Import queue from exported file
• !ep / !export | Export the queue for import in future
• !stop / !leave | Leave from vc and clear the queue
• !update / !restart | Update and restart your music player
## 🗣 <a name="languages"></a>Languages

```text
en    English
de    German
te    Telegu
```

## 💜 <a name="contribute"></a>Contribute
