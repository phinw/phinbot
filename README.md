# phinbot
a tiny little discord bot made with lua/discordia and JDK

## getting started

i reccomend just inviting the bot to your server but for self-hosting purposes, i have designed it so it's easy to selfhost. 

you need:
- linux (windows or a unix-based os might work, but this has been optimized for linux)
- git
- java (jdk/openjdk)
- lua 5.3 or above
- luvit
- discordia 2.0 or above

## tutorial 
this tutorial assumes you use debian or something based off debian like ubuntu, which is what i use. 

### config
this bot runs off a LUA and JDK folder, along with a shell script for running the bot. im planning on editing both files to run off 1 config folder but for now don't mind it. 

### LUA folder
once you open lua, create a file called settings.lua using your preferred text editor. copy and paste this file and replace "!" on "Prefix =" with your preferred prefix and "token" on "Token =" with your bot's token. save and go back into the main folder.

### JAVA folder
once you open java, create a file called config.txt using your preferred text editor. copy and paste this file in it.

this has some more config options for some more customization. you don't have to set everything, but i reccomend it. 

(TODO: make main config file so you don't have to paste the token and prefix twice)

REQUIRED OPTIONS
paste your bot token after token = 
paste your discord ID after owner = (this sets the bot owner)
paste your prefix in quotations after prefix = 

STATUS
paste your bots' status in quotations after game =
(NOTE: prefix it with "Playing", "Listening to", or "Watching". no prefix sets it to playing)
paste the status you want your bot in after status = 
(valid values are ONLINE, IDLE, DND, and INVISIBLE)
if you are running the bot in a single server, make songinstatus true if you want the bot to have the song playing now in the status. (will not work in multiple servers)


if you want the bot to have another prefix (like a universal prefix) change the quoted text. i highly reccommend just keeping it as "@MENTION"
the next 5 settings are emotes for notifying of music command successes, errors, etc, you can change these if you want 
setting npimages as true displays thumbnails for songs played, but if you don't want your bot to do so or you want it to be more compact

BANDWIDTH OPTIONS

if you care about bandwidth set stayinchannel as false. stayinchannel will have the bot stay in vc
if you want to place a limit on songlength change the number after maxtime = to something other than 0 in seconds. 0 means that there's no limit.



## credits
- me for making this bot
- sarah for being an amazing gf and helping me 
- jagrosh for providing the music bot's base (thank you for your service)
