<h3 align="center">
A cli to browse and watch anime (alone AND with friends). This tool scrapes the site <a href="https://allanime.to/">allanime.</a>
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
git clone "https://github.com/PhosCity/ani-cli.git" && cd ./ani-cli
sudo cp ./ani-cli /usr/local/bin
cd .. && rm -rf "./ani-cli"
```

_Also note that mpv installed through flatpak is not compatible_

## Uninstall

```sh
sudo rm "/usr/local/bin/ani-cli"
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

## Homies

* [animdl](https://github.com/justfoolingaround/animdl): Ridiculously efficient, fast and light-weight (supports most sources: allanime, zoro ... (Python)
* [jerry](https://github.com/justchokingaround/jerry): stream anime with anilist tracking and syncing, with discord presence (Shell)
* [anipy-cli](https://github.com/sdaqo/anipy-cli): ani-cli rewritten in python (Python)
* [Dantotsu](https://github.com/rebelonion/Dantotsu): Rebirth of Saikou, Best android app for anime/manga/LN with anilist integration (Kotlin)
* [mangal](https://github.com/metafates/mangal): Download & read manga from any source with anilist sync (Go)
* [lobster](https://github.com/justchokingaround/lobster): Watch movies and series from the terminal (Shell)
* [mov-cli](https://github.com/mov-cli/mov-cli): Watch movies/shows in the cli (Python/Shell)
* [dra-cla](https://github.com/CoolnsX/dra-cla): ani-cli equivalent for korean dramas (Shell)
* [redqu](https://github.com/port19x/redqu):  A media centric reddit client (Clojure)
