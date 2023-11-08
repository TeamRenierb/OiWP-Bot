# Open in WhatsApp

![LICENSE](https://img.shields.io/github/license/TeamRenierb/OiWP-Bot?style=flat&color=ff0000)
![GitHub issues](https://img.shields.io/github/issues/TeamRenierb/OiWP-Bot?color=fdf629)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/TeamRenierb/OiWP-Bot?color=c4fff9&label=Repo%20size)
![Lines of code](https://img.shields.io/tokei/lines/github/TeamRenierb/OiWP-Bot?color=e63977)
[![Hits-of-Code](https://hitsofcode.com/github/TeamRenierb/OiWP-Bot?branch=main)](https://hitsofcode.com/github/TeamRenierb/OiWP-Bot/view?branch=main)


<div align="center" width="100%">
<img width=200 src="OiWP-Logo.png">
</div>

> I was using a great [app](https://github.com/subhamtyagi/openinwa/) to open a whatsapp chat with a given number directly without saving that number in my contact list, but I felt it was overkill and uninstalled it, then searched telegram for a bot doint the same job but couldn't find so decided to make a new one.

## [See it in action](https://t.me/InWhatsAppBot)


# Deploy
> If you want to deploy to vercel, you'll find the relevant code in `vercel` branch, just select it from top left branches menu, or locally by running `git checkout vercel`.

> Heroku Deployment not added because Developers are too lazy to create an app.json, so do it yourself or deploy manually to Heroku.

## Using docker

### Requirements

- [docker-compose](https://github.com/docker/compose)

### Steps

- Add your bot token to `docker-compose.yml` file
- Run `docker-compose up -d`

## Development
**Make sure you have Python `3.12` and [poetry](https://python-poetry.org/) installed.**

- Clone this repo
  - `git clone https://github.com/TeamRenierb/OiWP-Bot`
  - `cd OiWP-Bot`
- Run
  - `poetry shell && poetry install`
  - `python main.py`
- Build
  - `docker buildx build --platform linux/amd64,linux/arm64 --load -t OiWP-Bot:latest .`
- Run a docker container from the built image
  - `docker run -d --name OiWP-Bot -e BOT_TOKEN=you_bot_token OiWP-Bot`


###### Logo was designed by [dtafalonso](https://iconarchive.com/artist/dtafalonso.html) - [deviantart](https://www.deviantart.com/dtafalonso)
