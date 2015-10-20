# dbiScripts
###A collection of MUSHClient [only, sorry] scripts I've developed for DBInfinity [a dragonball Z mud] for quality of life/usability.

###Foreword: Botting is illegal!!
######Anything which sends commands to the DBI server without your direct intervention is against the rules.
###That being said:
######This isn't a bot. If you are expecting it to play the game for you, you will be sad. The aggregator script doesn't send anything to the server, with the exception of the "setPrompt" and "setBattlePrompt" aliases, both of which are legal aliases.
###In the words of Rendo: don't be a dildo.
######Admins will catch you botting. If you modify my script for the purposes of botting [which is against MUD rules], not only are you breaking the rules, but you're making a legitimately helpful script look bad. I urge you not to do either.
###DO NOT UNDER ANY CIRCUMSTANCES MODIFY MY AGGREGATOR SCRIPT AS A BOT/AUTOMATION SCRIPT. 
######I will hate you, the admins will hate you, and basically everyone will hate you. Also you'll get banned. DON'T DO IT.

##Installation
#####To use any of these scripts, go to Program Files (x86)/MUSHClient/worlds/plugins and drop them in. From there, follow each set of instructions.

Here's how to install each of them, in guide form:

####1. Chat_Redirector 
  * Puts your chat messages in a separate window.
  * Install: create a NEW world with an IP of 0.0.0.0 (fake IP world, that makes it connect to nothing/local - your machine).
  * Important: Name it "DBI Chats" and save the world as "DBI Chats.mcl".
  * Connect to DBI (if you aren't already) and go to File -> Plugins -> Add -> Chat_Redirector.xml
  * The plugin should begin capturing chat-channel messages immediately!
  * Protip: un-maximize your DBI window and your DBI chat window and place them side by side, roughly half the screen each.
  * DBI output easily fits in half a screen, so you can split them into two windows - you won't miss anything that way!

####2. [totally optional] Chat_Input_Sender
  * Relays anything you type into your CHAT world to your actual world window, because otherwise typing there does nothing.
Install: before this will work, you need to modify LINE # 28 of this script. 
  * Change "DBI" to match whatever your DBI world is named. Mine is simply named "DBI" - yours might be "DB Infinity", etc.
  * Afterwards, click on your "DBI Chats" world to make it active, then go to File -> Plugins -> Add -> Chat_Input_Sender.xml
  * That's all! You should now be able to type in your chat world and still have it send to the real DBI world.

####3. [The good stuff] Aggregated_DBI
  * Scrapes all kinds of data to give you meaningful statistics, reduced spam and colorful output.
Install: Click your "DBI" world to make it active and go to File -> Plugins -> Add -> Aggregated_DBI.xml
  * Before this will work [mostly], you need to use my prompt and battle prompt. 
  * It's required for the regex to work properly on your prompts.
  * I've made this very simple: type "setPrompt" and "setBattlePrompt".
  * Two aliases I've created in the script will change your prompt for you!
  * You're done! Enjoy the [hopefully] improved DBI experience!

####Some disclaimer:
  * Alert messages will appear when important things happen:
    * While meditating, if you max out, it will alert you to Focus Ki. (Sorry if you're kicapped!)
    * While focusing, and below 20% of your max Ki, it alerts you to Meditate.
    * Anytime your Ki is below 20%, it turns RED.
    * If your armor falls below 80% durability, it turns your DR [damage reduction%] to RED, reminding you to repair.
    * Any time you receive the "You must stand to do that!" message, it alerts you to STAND UP.
    * Any time you try to use an ability and don't have enough Focus, your Focus will turn RED for a single prompt cycle.
  * Your focus % is based on the HIGHEST NUMBER THE SCRIPT HAS SEEN SINCE YOUR LAST LOGIN.
    * Ignore it until it hits max and then it will be accurate from that point on.

####Suggestions:
I won't go into detail, but there's a lot of redux output. Some of it you may like, some if it you might not. 
Feel free to make suggestions, but understand that this is generally tuned to my preferences.
If you disagree with my params and can't compel me to change it, feel free to modify it to your preference!

