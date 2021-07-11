<h1 align="center"> xkcd bot. </h1>

<p align="center">
  <img src="./src/assets/xkcd.png" width="350" alt="The xkcd logo.">
</p>

<p align="center">
  A straightforward Discord bot that retrieves and sends xkcd comics straight from the API to your Discord channel.
</p>

<p align="center">
  <a href="https://github.com/weiyi-m/xkcd-bot/blob/main/package.json"><img src="https://img.shields.io/github/package-json/v/weiyi-m/xkcd-bot"></a>
  <a href="https://github.com/weiyi-m/xkcd-bot/tree/main/src"><img src="https://img.shields.io/tokei/lines/github/weiyi-m/xkcd-bot"></a>
  <a href="https://github.com/weiyi-m/xkcd-bot/blob/main/LICENSE"><img src="https://img.shields.io/github/license/weiyi-m/xkcd-bot"></a>
  <a href="https://github.com/weiyi-m/xkcd-bot/blob/main/package.json"><img src="https://img.shields.io/github/package-json/dependency-version/weiyi-m/xkcd-bot/discord.js"></a>
</p>

<p align="center">
  Invite the bot <a href="https://discord.com/api/oauth2/authorize?client_id=863300460034392084&permissions=117760&scope=bot">here!</a>
</p>

<hr>

<details open="open">
  <summary>Table of Contents</summary>
  <br>
  <ol>
    <li>
      <a href="#about">About The Project</a>
      <ul>
        <li><a href="#inspiration">Inspiration</a></li>
        <li><a href="#functionality">Features and Functions</a></li>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#future-plans">Future Plans</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li>
      <a href="#license">License</a>
    </li>
    <li>
      <a href="#contact-and-more-information">Contact & More Information</a>
    </li>
    <li>
      <a href="#special-thanks">Special Thanks</a>
    </li>
  </ol>
</details>
<hr>
<br>

## About
<br>
<p align="center">
  <img src="https://i.imgur.com/NiMeT1D.png" alt="A demonstrative picture of what the bot does." width="700">
</p>

### Disclaimer
This project (or at least, Version 1.0.0) was built in 48 hours for Major League Hacking's [Hacktoon](https://hacktoon.devpost.com/) event.
<br>
<hr>

### Inspiration
[xkcd comics.](https://xkcd.com/)

They are humorous, comedic, witty, and somehow, Randall Munroe (former NASA programmer and author of 3 amazing books) wraps up this wonderful package of science, technology, and mathematics with relatable stick figures that seem to be more than simple lines and circles. 

Statistics have shown that 98% of MLHers have Discord installed (this is not factual, this is made up to exaggerate the usefulness of my hack but pretty please pretend that it's real), and most of them spend their time chatting around with others or pulling their hair whilst staring at their favourite IDE. While I can't integrate the geniosity of xkcd comics into VS Code or Atom or Sublime Text or [butterflies](https://xkcd.com/378/), I can always pull up a couple of Javascript files and work my way around Discord bots.
<br>
<hr>

### Functionality
Introducing xkcd! xkcd, the bot, not to be confused with xkcd, the webcomic, is a xkcd-themed Discord bot whose sole purpose is to retrieve and send xkcd comics of your choosing. 

Just kidding, xkcd (the bot) features plenty of other commands, such as help, invite, statistics, what, eval, reload, flip, and ping commands. What's more, other than just typing in a number to view a xkcd comic of your choice, you can let the bot do the work for you by letting it choose a random comic, or by letting it show you the latest xkcd comic.
<br>
<hr>

### Built With
xkcd (again, the bot) was built using:
- [Discord.js](https://discord.js.org)
- [xkcd API](https://xkcd.com/json.html/)
- [Chalk](https://github.com/chalk/chalk#readme)

xkcd is hosted 24/7 using:
- [Linode](https://www.linode.com/)

With a couple of creaks and tweaks here and there, accompanied by my unhealthy obsession for the simplicity yet complexity of Discord bots, you've got the xkcd bot.
<br>
<hr>

### Future Plans
There's quite a bit of things that I was planning to do for this Discord bot, but sadly, I wasn't able to implement them properly.

Possible future features include:
- Per-server settings, such as custom prefixes using [Firebase](https://firebase.google.com/) or [MongoDB](https://www.mongodb.com/)
- Per-user settings, as there are people who can get annoyed with the bot's line replies
- A custom website for the bot

<hr>


## Getting Started

Below are some simple instructions on how to clone, download and create your own xkcd Discord bot.
To get a local copy of this project up and running, feel free to take a gander at the prerequisites and the installation guide.


### Prerequisites

Before continuing, make sure you have the following software:
- [Node.js](https://nodejs.org/en/download/)
- npm
  ```sh
  npm install npm@latest -g
  ```
<hr>
  
### Installation

1. Head over to [https://discord.com/developers/applications](https://discord.com/developers/applications) and create a new application.
2. Give it a name, a profile picture, and then click on the "Bot" section and add the application as a bot user. Make sure to copy the token.
3. Clone the repo and cd into it
   ```sh 
   git clone https://github.com/weiyi-m/xkcd-bot.git
   cd xkcd-bot
   ```
4. Install the required NPM packages
   ```sh
   npm install
   ```
5. Rename [`example.json`](https://github.com/weiyi-m/xkcd-bot/blob/main/src/example.json) to `config.json` and replace the placeholder text with necessary details.
   ```json
   "token": "Your Discord bot token in step 2.",
   "owner": "Your Discord user ID. You can find by following https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-",
   "invite": "Your OAuth2 bot invite link. You can find by following https://discordjs.guide/preparations/adding-your-bot-to-servers.html#bot-invite-links"
   ```
6. cd into src and run the xkcd.js file.
   ```sh
   cd src
   node xkcd.js
   ```
7. Your bot should be online now. Congratulations!
8. This is all optional, but if you want to host your bot 24/7, you can use [Linode](https://linode.com). Feel free to follow [this video tutorial](https://www.youtube.com/watch?v=Cl2Od4mR9Ds) on how to deploy a Discord bot to Linode.

<hr>

## License
The code in this repository is licensed under the MIT License. See [`LICENSE`](https://github.com/weiyi-m/xkcd-bot/blob/main/LICENSE) for more information. <br>
All xkcd comics belong to Randall Munroe, and they are licensed under the CC BY-NC 2.5 License. Click [here](https://creativecommons.org/licenses/by-nc/2.5/) for more information.

## Contact and More Information
This bot was made by me. <br>
You can find me on [Twitter](https://twitter.com/thermopmeter), [Polywork](https://poly.work/foop), or [Discord](https://discord.com/users/698216301675544667). <br>
The Devpost project submission can be viewed [here](https://devpost.com/software/xkcd-zv3fxp).

## Special Thanks

- [Shields](https://shields.io)
- [Choose a License](https://choosealicense.com)
- [Discord.js](https://discord.js.org)
- [Discord Reply](https://www.npmjs.com/package/discord-reply)
- [xkcd](https://xkcd.com)
- [Linode](https://linode.com)
- [Chalk](https://github.com/chalk/chalk#readme)
