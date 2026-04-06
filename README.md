<h3 align="center">
A cli to browse and watch anime (alone AND with friends). This tool scrapes the site <a href="https://allmanga.to/">allmanga.</a>
</h3>
	
<h1 align="center">
	Showcase
</h1>

[ani-cli-demo.webm](https://user-images.githubusercontent.com/44473782/224679247-0856e652-f187-4865-bbcf-5a8e5cf830da.webm)

## Table of Contents

- [Fixing errors](#fixing-errors)
- [New in this fork](#New-in-this-fork)
- [Installing from source](#installing-from-source)
- [Uninstall](#uninstall)
- [Dependencies](#dependencies)
- [Homies](#homies)

## Fixing errors

If you encounter `No results found` (and are sure the prompt was correct) or any breaking issue, then make sure you are on **latest version** by typing
`sudo ani-cli -U` to update on Linux, Mac and Android. On Windows, run windows terminal preview and there type `ani-cli -U`.
If after this the issue persists then open an issue.

## Install

## New in this fork

- Update history file only after you watch the episode not as soon as you select play it.
- ~~Option to use dmenu as a launcher for all sort of selection. I create a hotkey to open the script and use dmenu to select anime without ever opening terminal.~~ Added to upstream as of v4
- Option to update anilist or myanimelist as you update the history file using trackma. Auto selects anime to update if it's present in your watching or plan to watch list otherwise prompts you to add an anime if to your anilist or mal.
- Only tested in Linux with mpv player. Any other OS or players, I've tried not to mess it for them, but it may or may not work.
- A script that uses ani-cli's history file but streams using animdl instead. Useful when ani-cli goes down.

## Installing from source

Install dependencies [(See below)](#Dependencies)

Uninstall any other forks of ani-cli if you already have them installed.

```sh
git clone "https://github.com/PhosCity/ani-cli.git"
sudo cp ani-cli/ani-cli /usr/local/bin
rm -rf ani-cli
```

## Uninstall

```sh
sudo rm "/usr/local/bin/ani-cli"
```

## Completion

### bash

To add tab completions using bash run the following command inside the ani-cli directory

```
cp _ani-cli-bash /path/to/your/completions
echo "source /path/to/your/completions/_ani-cli-bash" >> ~/.bashrc
```

### zsh

To add tab completions using zsh run the following command inside the ani-cli directory

```
cp _ani-cli-zsh /path/to/your/completions
echo "source /path/to/your/completions/_ani-cli-zsh" >> ~/.zshrc
```

## Dependencies

- grep
- sed
- curl
- mpv - Video Player
- iina - mpv replacement for MacOS
- aria2c - Download manager
- yt-dlp - m3u8 Downloader
- ffmpeg - m3u8 Downloader (fallback)
- fzf - User interface
- trackma (Optional)
- rofi (Optional)
- ani-skip (optional)

## FAQ

<details>
	
* Can I change subtitle language or turn them off? - No, the subtitles are baked into the video.
* Can I watch dub? - Yes, use `--dub`.
* Can I change dub language? - No.
* Can I change media source? - No (unless you can scrape that source yourself).
* Can I use vlc? - Yes, use `--vlc` or `export ANI_CLI_PLAYER=vlc`.
* Can I adjust resolution? - Yes, use `-q resolution`, for example `ani-cli -q 1080`.
* How can I download? - Use `-d`, it will download into your working directory.
* Can i change download folder? - Yes, set the `ANI_CLI_DOWNLOAD_DIR` to your desired location.
* How can I bulk download? - `Use -d -e firstepisode-lastepisode`, for example `ani-cli onepiece -d -e 1-1000`.

**Note:** All features are documented in `ani-cli --help`.

</details>

## Homies

- [animdl](https://github.com/justfoolingaround/animdl): Ridiculously efficient, fast and light-weight (supports most sources: allmanga, zoro ... (Python)
- [jerry](https://github.com/justchokingaround/jerry): stream anime with anilist tracking and syncing, with discord presence (Shell)
- [anipy-cli](https://github.com/sdaqo/anipy-cli): ani-cli rewritten in python (Python)
- [Dantotsu](https://github.com/rebelonion/Dantotsu): Rebirth of Saikou, Best android app for anime/manga/LN with anilist integration (Kotlin)
- [mangal](https://github.com/metafates/mangal): Download & read manga from any source with anilist sync (Go)
- [lobster](https://github.com/justchokingaround/lobster): Watch movies and series from the terminal (Shell)
- [mov-cli](https://github.com/mov-cli/mov-cli): Watch everything from your terminal. (Python)
- [dra-cla](https://github.com/CoolnsX/dra-cla): ani-cli equivalent for korean dramas (Shell)
- [redqu](https://github.com/port19x/redqu): A media centric reddit client (Clojure)
- [doccli](https://github.com/TowarzyszFatCat/doccli): A cli to watch anime with POLISH subtitles (Python)
- [GoAnime](https://github.com/alvarorichard/GoAnime): A CLI tool to browse, play, and download anime in Portuguese(Go)
- [Curd](https://github.com/Wraient/curd): A CLI tool to watch anime with Anilist, Discord RPC, Skip Intro/Outro/Filler/Recap (Go)

* [FastAnime](https://github.com/Benex254/FastAnime): browser anime experience from the terminal (Python)
