# SolanaNSB - A Solana NFT Sales Bot

SolanaNSB is a bot that track your NFT sales on Secondery Marketplaces

## About
This bot created by [NoamPeretz](https://github.com/byfunkz) . The Bot created for my project - [@koalasnft_](https://twitter.com/koalasnft_). If this will help you please support me by follow me on Twitter 🐦

<img src="https://i.postimg.cc/T31b2BZs/l-OGO-V2-1080x1080-Rounded.png" width=200>

## Ok So Let's Start Build the Bot! 🤖

### Requirement
- [x] [Node v16.6](https://nodejs.org/download/release/v16.16.0/) (Download the node-v16.16.0-x64.msi/node-v16.16.0-x84.msi *Depends on your computer*  )
- [x] [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/#windows-stable) (Follow the instructions)

**Clone this repository:**

```
git clone https://github.com/funkzzz/SolanaNSB.git
```
**cd into the folder**
```
cd SolanaNSB
```

### Updating .env with your Secrets 
Inside SolanaSNB you can find the env file. Inside it you will find the configurations:

```
DISCORD_BOT_TOKEN=
SOLANA_RPC=
SUBSCRIPTION_DISCORD_CHANNEL_ID=
SUBSCRIPTION_MINT_ADDRESS=
```

### DISCORD BOT TOKEN
Go to [Discord Developer Portal]() , login with your Discord account and then you will reach the main page -> 
<img src="https://i.postimg.cc/v8rJzZ0W/Screenshot-2022-10-14-102354.png" width=800>
Click on the "New Application" Button -> Name your Bot -> Create a Bot User by navigating to the “Bot” tab and clicking “Add Bot” -> Scroll down and make sure the bot has the following permission:
Give him the permission "Administrator". If you are afraid to bring him this approach, you can only mark the following approaches:

- [x] Send messages
- [x] Send messages in Threads
- [x] Embed links
- [x] Embed files
- [x] Manage Messages
- [x] Read Message History 
- [x] View Channels

Invite the bot by navigating to the “OAuth2” tab -> Tick the “bot” checkbox under “scopes”. -> Check the permissions required for your bot to run under "Bot Permissions" -> Now the resulting URL can be used to add your bot to a server. Copy and paste the URL into your browser, choose a server to invite the bot to, and click “Authorize”.

After you done that go back to the discord developer portal site and navigate to the bot tab and click on "Reset Token".(Keep the token you create in a safe place, if you forget it you need to create a new one and update it with the code)

<img src="https://i.postimg.cc/XYrLJshs/Screenshot-2022-10-14-104114.png" width=800>

### SOLANA RPC
If you want to create your own solana node rpc you can go to google and check how to do that. but if you dont want to create your own rpc and use a public one you can use: https://api.mainnet-beta.solana.com

### SUBSCRIPTION DISCORD CHANNEL ID
Go to User Settings -> Advanced -> and make sure the Developer mode is turned on
Afterwards go to your Discord server and select any channel you want the bot to send every time there is a sale and just right click on the channel and then click "copy ID".
If it was not clear, you can go through the instructions through the following link: [Where can I find my User/Server/Message ID?](https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-)

### SUBSCRIPTION MINT ADDRESS
The address that you want the bot will track:
Go to Solscan -> Search your collection -> Click on any NFT you choose (it doesn't matter which one) -> Then choose one of the creators (avoid personal messages because it can identify unwanted sales)

<img src="https://i.postimg.cc/CxKvThSn/Screenshot-2022-10-14-105737.png" width=450>

### Preferences 🎨

**Discord Bot Embeded Color:**
if you want to you can change the bot embeded message color by going to src/lib/discord/notifyDiscordSale.ts in [line 49]([link](https://github.com/funkzzz/SolanaNSB/blob/main/src/lib/discord/notifyDiscordSale.ts#L49)).
Go to https://redketchup.io/color-picker , pick the color that you want and then copy the hex code (#?????). in line 49 delete the 0xffffff and type 0x{pase your hex without the #}

**Custom status:**
you can change the bot status by going to src/lib/discord/index.ts in [line 22]([link](https://github.com/funkzzz/SolanaNSB/blob/main/src/lib/discord/index.ts#L22)).
```client.user?.setActivity(`type here whatever you want` , { type: "Activity Type"})```

Activity Type:
Type of activity: for type of activity you can choose from the following options:
- [x] WATCHING
- [x] PLAYING
- [x] LISTENING
- [x] STREAMING
- [x] COMPETING


## Install dependencies
```
npm install
```

## Run the Bot
Simply run:
```yarn dev```
And your bot should be online!

## Error
if you got any error with the port just go to src/server.ts on line 27 Change the port to number between 4000-8080

### Hosting your Bot
I haven't found a free hosting service that easy to use at the moment (if anyone here does, I'd love for you to let me know). But here is an option you can try:

- [x] https://www.ibm.com/cloud/code-engine 

*Please don't ask questions about how to host this bot through IBM because I don't know either!*

# Show me support
If this will help you please support me by follow me on Twitter 🐦[@byfunkz](https://twitter.com/byfunkz)
