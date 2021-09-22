[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/eritislami/evobot)

![logo](https://1.bp.blogspot.com/-9tIeR9DYKTo/YUsQlV56V3I/AAAAAAAACe8/7-2D_kNgfTMKOKDQpnGa8owT0XbDRSkWgCLcBGAsYHQ/s1366/Logo%2BJ0TAC%2Bvermelha%2Be%2Bbranca%2Bcom%2Bletra%2Bvermelha.jpg)

# 🤖 J0TAC Master (Discord Music Bot)
> J0TAC Master is a Discord Music Bot built with discord.js & uses Command Handler from [discordjs.guide](https://discordjs.guide)

## Requirements

1. Discord Bot Token **[Guide](https://discordjs.guide/preparations/setting-up-a-bot-application.html#creating-your-bot)**
2. YouTube Data API v3 Key **[Guide](https://developers.google.com/youtube/v3/getting-started)**  
2.1 **(Optional)** Soundcloud Client ID **[Guide](https://github.com/zackradisic/node-soundcloud-downloader#client-id)**
3. Node.js v14.0.0 or newer

## 🚀 Getting Started

If deploying to Heroku make sure to create config variables

```
git clone https://github.com/eritislami/bot.git
cd 
bot
npm install
```

After installation finishes you can use `node index.js` to start the bot.

## ⚙️ Configuration

Copy or Rename `config.json.example` to `config.json` and fill out the values:

⚠️ **Note: Never commit or share your token or api keys publicly** ⚠️

```json
{
  "TOKEN": "",
  "YOUTUBE_API_KEY": "",
  "SOUNDCLOUD_CLIENT_ID": "",
  "MAX_PLAYLIST_SIZE": 10,
  "PREFIX": "/",
  "PRUNING": false,
  "LOCALE": "en",
  "DEFAULT_VOLUME": 100,
  "STAY_TIME": 30
}
```

Currently available locales are:
- English (en)
- Arabic (ar)
- Brazilian Portuguese (pt_br)
- Dutch (nl)
- French (fr)
- German (de)
- Italian (it)
- Korean (ko)
- Polish (pl)
- Russian (ru)
- Simplified Chinese (zh_cn)
- Spanish (es)
- Swedish (sv)
- Traditional Chinese (zh_tw)
- Turkish (tr)
- Check [Contributing](#-contributing) if you wish to help add more languages!

## 📝 Features & Commands

> Note: The default prefix is '/'

* 🎶 Play music from YouTube via url

`/play https://www.youtube.com/watch?v=GLvohMXgcBo`

* 🔎 Play music from YouTube via search query

`/play under the bridge red hot chili peppers`

* 🎶 Play music from Soundcloud via url

`/play https://soundcloud.com/blackhorsebrigade/pearl-jam-alive`

* 🔎 Search and select music to play

`/search Pearl Jam`

Reply with song number or numbers seperated by comma that you wish to play

Examples: `1` or `1,2,3`

* 📃 Play youtube playlists via url

`/playlist https://www.youtube.com/watch?v=YlUKcNNmywk&list=PL5RNCwK3GIO13SR_o57bGJCEmqFAwq82c`

* 🔎 Play youtube playlists via search query

`/playlist linkin park meteora`
* Now Playing (/np)
* Queue system (/queue, /q)
* Loop / Repeat (/loop)
* Shuffle (/shuffle)
* Volume control (/volume, /v)
* Lyrics (/lyrics, /ly)
* Pause (/pause)
* Resume (/resume, /r)
* Skip (/skip, /s)
* Skip to song # in queue (/skipto, /st)
* Move a song in the queue (/move, /mv)
* Remove song # from queue (/remove, /rm)
* Play an mp3 clip (/clip song.mp3) (put the file in sounds folder)
* List all clips (/clips)
* Show api ping (/ping)
* Show bot uptime (/uptime)
* Toggle pruning of bot messages (/pruning)
* Localization in 6 languages
* Help (/help, /h)
* Command Handler from [discordjs.guide](https://discordjs.guide/)
* Media Controls via Reactions

