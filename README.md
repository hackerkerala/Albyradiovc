# Albyradiovc
# Telegram Voice Chat Bot with Channel Support.

A Telegram Bot to Play Audio in Voice Chats With Youtube and Jio Saavn support.
Supports Playing Music files from a telegram channel.
Supports Live streaming from youtube.



## Deploy to Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/ALBINPRAVEEN/Albyradiovc)

NOTE: Make sure you have started a VoiceChat in your Group before deploying.
### Deploy to VPS

```sh
git clone https://github.com/ALBINPRAVEEN/Albyradiovc
cd Albyradiovc
pip3 install -r requirements.txt
# <Create Variables appropriately>
python3 main.py
```

# Vars:
1. `API_ID` : Get From my.telegram.org
2. `API_HASH` : Get from my.telegram.org
3. `BOT_TOKEN` : @Botfather
4. `SESSION_STRING` : Generate From here [![GenerateStringName](https://img.shields.io/badge/repl.it-generateStringName-yellowgreen)](https://replit.com/@ALBINPRAVEEN1/getStringName)
5. `CHAT` : ID of Channel/Group where the bot plays Music.
6. `LOG_GROUP` : Group to send Playlist, if CHAT is a Group
7. `ADMINS` : ID of users who can use admin commands.
8. `STREAM_URL` : Stream URL of radio station or a youtube live video to stream when the bot starts or with /radio command.You can also use a telegram channel as radio station. Just upload all you music files to a telegram channel and add the bot and user account in that channel and use chat_id of channel in STREAM_URL.You can also use any public telegram channels, in that case use the username of such channel in place of STREAM_URL (Bot being admin in public channel not required.)
9. `MAXIMUM_DURATION` : Maximum duration of song to play.(Optional)
10. `REPLY_MESSAGE` : A reply to those who message the USER account in PM. Leave it blank if you do not need this feature. 
11. `ADMIN_ONLY` : Pass `Y` If you want to make /play and /splay commands only for admins of `CHAT`. By default /play and /splay is available for all.

- Enable the worker after deploy the project to Heroku
- Bot will starts radio automatically in given `CHAT` with given `STREAM_URL` after deploy.(24*7 Music even if heroku restarts, radio stream restarts automatically.)  
- To play a song use /play as a reply to audio file or a youtube link.
- Use /play <song name> to play song from youtube and /splay <song name> to play from JioSaavn or /cplay <channel username or channel id> to play music from a telegram channel.
- Use /help to know about other commands.

**Features**

- Supports Play from Youtube Playlist.
- Change VoiceChat title to current playing song name.
- Supports Live streaming from youtube
- Supports both Jio Saavn and youtube to search songs.
- Play from telegram file supported.
- Play whole music files from a telegram channel.
- Starts Radio after if no songs in playlist.
- Automatically downloads audio for the first two tracks in the playlist to ensure smooth playing
- Automatic restart even if heroku restarts.

#### Support

Connect Me On [Telegram](https://telegram.dog/i_am_albin_praveen)
