<h3 align="center">
A cli to browse and watch anime. This tool scrapes the site <a href="https://animixplay.to/">animixplay.</a>
</h3>
	
<h1 align="center">
	Showcase
</h1>

https://user-images.githubusercontent.com/44473782/160729779-41fe207c-b5aa-4fed-87db-313c83caf6bb.mp4

## Table of Contents

- [New in this fork](#New-in-this-fork)
- [Install](#Installing-from-source)
- [Uninstall](#Uninstall)
- [Dependencies](#Dependencies)
- [Homies](#Homies)
- [Contribution Guidelines](./CONTRIBUTING.md)
- [Disclaimer](./disclaimer.md)

## New in this fork

- Update history file only after you watch the episode not as soon as you select play it.
- ~~Option to use dmenu as a launcher for all sort of selection. I create a hotkey to open the script and use dmenu to select anime without ever opening terminal.~~ Added to upstream as of v4
- Option to update anilist or myanimelist as you update the history file using trackma. Auto selects anime to update if it's present in your watching or plan to watch list otherwise prompts you to add an anime if to your anilist or mal.
- Only tested in Linux with mpv player. Any other OS or players, I've tried not to mess it for them, but it may or may not work.

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
- wget
- mpv - Video Player
- iina - mpv replacement for MacOS
- aria2c - Download manager
- ffmpeg - m3u8 Downloader
- fzf - User interface
- trackma (Optional)

## Homies

- [animdl](https://github.com/justfoolingaround/animdl): Ridiculously efficient, fast and light-weight (supports most sources: allanime, zoro ... (Python)
- [jerry](https://github.com/justchokingaround/jerry): stream anime with anilist tracking and syncing, with discord presence (Shell)
- [anime-helper-shell](https://github.com/Atreyagaurav/anime-helper-shell): A python shell for searching, watching, and downloading anime (Python)
- [anipy-cli](https://github.com/sdaqo/anipy-cli): ani-cli rewritten in python (Python)
- [dra-cla](https://github.com/CoolnsX/dra-cla): ani-cli equivalent for korean dramas (Shell)
- [kaa.si-cli](https://github.com/Soviena/kaa.si-cli): Stream anime from kaa.si and sync with anilist (Python)
- [lobster](https://github.com/justchokingaround/lobster): Life action movies and series fom the terminal (Shell)
- [manga-cli](https://github.com/7USTIN/manga-cli): Read manga in the cli (Shell)
- [mangal](https://github.com/metafates/mangal): Download & read manga from any source with anilist sync (Go)
- [mov-cli](https://github.com/mov-cli/mov-cli): Watch movies/shows in the cli (Python/Shell)
- [saikou](https://github.com/saikou-app/saikou): Best android app for anime/manga with anilist integration (Kotlin)
- [tv-cli](https://github.com/Spaxly/tv-cli): Watch live TV in the cli (Shell)
