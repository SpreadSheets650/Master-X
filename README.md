
<h2 align="center">My Music Bot</h2>
<h4 align="center">High Quality Music Bot with a DJ System, Music Channel Setup, 24/7 in VC, Stage Channels, Slash Commands Support and more for FREE!</h4>
<p align="center">

## 🎭 Features

- ✅ Setup System
- ✅ Music
- ✅ 24/7
- ✅ Dj
- ✅ Custom Playlist (global)
- ✅ SlashCommand
- ✅ Custom prefix
- ✅ Filters
- ✅ Easy to use
- ✅ And much more!


For more information how to fill all the varialabes go to this page.
You do not need to edit anything like the PORT, ADDRESS, PASSWORD, HOST, SECURE and USERNAME. Unless you know what your doing.

After saving your changes you can open a terminal and go to the same location as the docker-compose file. Then type the following:

```bash
docker-compose up -d
```

The above command will start all your services and your bot should be up and running!

To update, you only have to type the following:

```bash
docker-compose up --force-recreate --build -d
image prune -f
```

You can automate this by using [Watchtower](https://github.com/containrrr/watchtower). The following should be sufficient:

```bash
docker run --detach \
    --name watchtower \
    --volume /var/run/docker.sock:/var/run/docker.sock \
    --restart on-failure \
    containrrr/watchtower --cleanup
```

Do note that the bot will restart itself to update to the latest!

## 🚀 Installation from source

```bash
git clone https://github.com/brblacky/lavamusic.git
```

After cloning, run

```bash
npm install
```

- Start the bot with `node src/sharder.js`

to snag all of the dependencies. Of course, you need [node](https://nodejs.org/en/) installed. I also strongly recommend [nodemon](https://www.npmjs.com/package/nodemon) as it makes testing _much_ easier.

## Intents

<p align="center">
  <a href="https://github.com/brblacky/lavamusic">
    <img src="https://media.discordapp.net/attachments/848492641585725450/894114853382410260/unknown.png">

  </a>
</p>
When you are running the Code you must have gotten this Error. To fix this head over to your Bot's Discord Application and go to the Bot Settings and find this:

<p align="center">
  <a href="https://github.com/brblacky/lavamusic">
    <img src="https://media.discordapp.net/attachments/848492641585725450/894115221701001216/unknown.png">

  </a>
</p>
Then turn on both of those Settings and click "Save Changes". Then you are done and it should be fixed!
<!-- CONFIGURATION -->

## ⚙️ Configurations

- edit in `src/config.js` and you can do in `.env`

```js
    token: process.env.TOKEN || "",  // your bot token
    prefix: process.env.PREFIX || "!", // bot prefix
    ownerID: process.env.OWNERID || "491577179495333903", //your discord id
    mongourl: process.env.MONGO_URI || "", // MongoDb URL
    embedColor: process.env.COlOR || "#303236", // embed colour
    logs: process.env.LOGS || "", // channel id for guild create and delete logs
```

## 🌋 Lavalink

```js
      "host": "localhost",
      "port": 2333,
      "password": "coders",
      "retryDelay": 3000,
      "secure": false
```

## ⚙️ SHARDS

- edit in `sharder.js`

```js
  respawn: true,
  autoSpawn: true,
  token: token,
  totalShards: 1,
  shardList: "auto",
```

- Create an application.yml file in your working directory and copy the [example](https://github.com/freyacodes/Lavalink/blob/master/LavalinkServer/application.yml.example) into the created file and edit it with your configuration.
- Run the jar file by running `java -jar Lavalink.jar` in a Terminal window.

<!-- ABOUT THE PROJECT -->

## 🌀 About

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=brblacky&repo=lavamusic&theme=tokyonight)](https://github.com/brblacky/lavamusic)

Lavamusic is a lavalink music bot base in [erela.js](https://github.com/MenuDocs/erela.js)
If you liked this repository, feel free to leave a star ⭐ to help promote !

## 💌 Support Server

[![DiscordBanner](https://invidget.switchblade.xyz/ns8CTk9J3e)](https://discord.gg/ns8CTk9J3e)<br />
[Support Server](https://discord.gg/ns8CTk9J3e) - lavamusic's Support Server Invite

# Donate

By donating, you will help me to maintain this Project!

- [PayPal](https://www.paypal.me/sdip521)

## 🤝 Contributing

1. [Fork the repository](https://github.com/brblacky/lavamusic/fork)
2. Clone your fork: `git clone https://github.com/your-username/lavamusic.git`
3. Create your feature branch: `git checkout -b my-new-feature`
4. Stage changes `git add .`
5. Commit your changes: `cz` OR `npm run commit` do not use `git commit`
6. Push to the branch: `git push origin my-new-feature`
7. Submit a pull request

<!-- LICENSE -->

## 🔐 License

Distributed under the Apache-2.0 license License. See [`LICENSE`](https://github.com/brblacky/lavamusic/blob/master/LICENSE) for more information.

[version-shield]: https://img.shields.io/github/package-json/v/brblacky/lavamusic?style=for-the-badge
[version-url]: https://github.com/brblacky/lavamusic
[contributors-shield]: https://img.shields.io/github/contributors/brblacky/lavamusic.svg?style=for-the-badge
[contributors-url]: https://github.com/brblacky/lavamusic/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/brblacky/lavamusic.svg?style=for-the-badge
[forks-url]: https://github.com/brblacky/lavamusic/network/members
[stars-shield]: https://img.shields.io/github/stars/brblacky/lavamusic.svg?style=for-the-badge
[stars-url]: https://github.com/brblacky/lavamusic/stargazers
[issues-shield]: https://img.shields.io/github/issues/brblacky/lavamusic.svg?style=for-the-badge
[issues-url]: https://github.com/brblacky/lavamusic/issues
[license-shield]: https://img.shields.io/github/license/brblacky/lavamusic.svg?style=for-the-badge
[license-url]: https://github.com/brblacky/lavamusic/blob/master/LICENSE
[spon-img]: https://media.discordapp.net/attachments/979364157541462066/982734017671606322/Vultr_Logo_Download_Vector.png
