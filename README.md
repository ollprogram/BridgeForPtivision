# TwitchDiscordBridge For the Ptivision
A copy of the [TwitchDiscordBridge](https://github.com/ollprogram/TwitchDiscordBridge) bot made for the Ptivision with new features.
</br> Links the [Discord](https://discord.com) chat and the [Twitch](https://www.twitch.tv) chat together. 
# What is Ptivision :
Ptivision is a Discord server made for events that look like the Eurovision. For more information join the discord server [here](https://discord.gg/Y66rvm9YE7)
# Author and Licence :
Hi I'm ollprogram and I am the author of this project. Thanks for using it. </br>Please don't be afraid to report bugs or mistakes to me. I'll try to fix them. By the way, english isn't my main language, so I'm sorry for english mistakes but I'm open if you find some. </br>
Find information about the licence used for this project [here](https://github.com/ollprogram/TwitchDiscordBridge/blob/main/LICENSE).
You need to know the licence before using my project. It gives information about how you can use it.
# Description :
With this application you will be able to link your Twitch chat with a Discord text channel in a guild.
</br>When someone will send something on a specified channel on Discord, the same message will be send to a specified Twitch chat, and reversly.
</br>In this project i'm using a lot the word "Bridge". What does a "Bridge" represent in this project? 
</br>A "Bridge" is an object which transfers messages between two destinations. In our case destinations are Discord and Twitch.
# Dependencies :
For this project I'm using three APIs :
- [JDA (Java Discord API)](https://github.com/DV8FromTheWorld/JDA)
- [Twitch4J (Java Twitch API)](https://github.com/twitch4j/twitch4j)
- [Emoji-Java (API to manipulate emojis codes)](https://github.com/vdurmont/emoji-java)
</br>You can see the Maven pom.xml [here](https://github.com/ollprogram/TwitchDiscordBridge/blob/main/pom.xml).
# Download :
You can download the runnable jar file [here](https://github.com/ollprogram/TwitchDiscordBridge/releases).
# Setup :
There are some procedures before launching the program :
<ol>
  <li> You need a <a href="https://discord.com">Discord</a> account and a Discord server (guild). </li>
  <li>Register a new bot on the <a href="https://discord.com/developers/docs/intro">Discord Developer Portal</a> (I recommand you to watch a tutorial on youtube). </br> You should also turn it to private mode.</li>
  <li> Add your bot on Discord with the <a href="https://discordapi.com/permissions.html">Discord Permissions Calculator</a> using your bot client ID. The Discord bot will need some permissions on your server. See the permissions needed in the screenshot below :
<img src="https://user-images.githubusercontent.com/39884051/148686617-3ca8d816-2a52-4724-a2d9-98dd1c962cb9.png" width="600"></img>
<p>If you want to activate other permissions, you will have to think about consequences. For exemple, if you decide to activate mentions to all roles for the bot, then every people from twitch will be able to mention all roles on discord.</p></li>
  <li> Create a new <a href="https://www.twitch.tv">Twitch</a> account for your Twitch bot. Recommanded to use OAuth2 and to make your bot moderator on the twitch channel where you stream.</li>
</ol>
</br></br>
When you launch the program for the first time, you need :
<ol>
  <li> Your Discord bot token (grab it on the <a href="https://discord.com/developers/docs/intro">Discord Dev Portal</a>).</li>
  <li>Your Twitch bot token (grab it <a href="https://twitchtokengenerator.com">Here</a>).</li>
  <li>A Twitch channel name (The channel where you stream).</li>
  <li> A discord channel ID. You need to activate first dev mode on discord <code>advanced -> developer_mode -> on</code>. Right click on the channel where you want your bot to listen to it, and copy the ID.</li>
</ol>

# Usage :
<h3> To launch the program with the console interface : </h3>
<code>java -jar TwitchDiscordBridge-1.0-shaded.jar</code> (cmd or terminal)

<h3> To list all commands : </h3>
Type <code>help</code> or <code>&ltcommand&gt help</code> in the console. Or type <code>!help</code> on Discord.

<h3>All commands on discord : </h3>
<ul>
  <li><code>!test</code> to see if the bot works.</li>
  <li><code>!code</code> to get the source code.</li>
  <li><code>!bridge &ltargument&gt</code> <ul>Arguments : 
      <li><code>target</code> this Discord channel is now linked to the Twitch chat.</li>
      <li><code>open</code> open the bridge.</li>
      <li><code>close</code> close the bridge.</li>
      <li><code>info</code> get information about the bridge.</li>
    </ul>
    </li>
  <li><code>!prefix &ltnew prefix&gt</code> to set a new prefix (also changes the nickname of your bot).</li>
  <li><code>!prefix reset</code> to reset the prefix (reset also the nickname).</li>
</ul>

<h3>All commands in the console :</h3>
<ul>
  <li><code>shutdown</code> shutdown the app without exceptions.</li>
  <li><code>shutdown now</code> shutdown the app with exceptions.</li>
  <li><code>say &ltyour message&gt</code> send a message on both platforms.</li>
  <li><code> bridge &ltargument&gt</code> <ul>Arguments :
    <li><code>twitchTarget &ltchannel name&gt</code> link the bridge to an other twitch chat.</li>
    <li><code>info</code> get information about the bridge.</li>
    <li><code>open</code> open the bridge.</li>
    <li><code>close</code> close the bridge.</li>
    </ul>
  </li>
</ul>

# JavaDocs :

# Next Upates :
- Allow to lock the bridge on one side. (comming very soon)
