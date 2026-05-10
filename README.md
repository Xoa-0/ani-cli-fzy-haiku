As of now, there is no fzf port for Haiku, which means that some software, including ani-cli, cannot run. Well, ani-cli-fzy-haiku (or ani-cli-haiku) fixes that!... almost.

This fork doesn’t introduce major changes; just two lines of code have been modified so that the ani-cli script uses fzy (which is available on HaikuDepot) instead of fzf.

---
# Basic setup:
```sh
git clone "https://github.com/Xoa-0/ani-cli-fzy-haiku.git"
cd ~/ani-cli-fzy-haiku
```

# Dependencies:
- grep
- sed
- curl
- mpv *or* VLC - Video Player
- aria2c - Download manager (aria2 in HaikuDepot)
- yt-dlp - m3u8 Downloader
- ffmpeg - m3u8 Downloader (fallback. ffmpeg-tools in HaikuDepot)
- fzy - User Interface
- openssl

# Known issues:
mpv may be laggy and/or slow. Use VLC instead: `ani-cli -v` 

For some reason, certain media may cause the media player to crash.
