## Plug dj bot writed in node.js with commands

### Commands

|Command Name |Arguments |Description |Minimum Rank |

|match      |`<@username>` | Love Calculator | User
|dare      |`<@username>` | Play truth & dare game with others | User
|truth      |`<@username>` | Play truth & dare game with others | User
|startroulette      |`null` | Manually start roulette. | Menager
|endroulette      |`null` | If roulette is started use this to end it manually. | Menager
|fortunecookie       |`null` | Open your fortunecookie.
|8ball       |`<any text>` | Asks the Magic 8 Ball a question.
|about       | | Displays bot's "about" message.
|afktime     |`[@username\|#userID]` | Returns the amount of time a user has been inactive. Gets your own info if no valid argument.
|anagram     |`<7-30 character string>` | Returns an anagram of the given word(s), retrieved from www.anagramgenius.com.
|blacklist   |`<blacklist name>` `<add//remove\|rem>` `<youtube\|yt\|1//soundcloud\|sc\|2>` `<video ID//track ID>` | Adds or removes songs to/from a given blacklist.|Manager
|blacklists  || Returns list of valid blacklist names to be used with the blacklist command.
|commands    || Lists active commands and amount of inactive commands.
|dc          || Places you back into the waitlist at your old position ONLY IF you were disconnected while waiting.Must be undefined since disconnecting.
|dclookup    |`[@username\|userID]` | Returns a user's last disconnect time and position. Use their ID if they are not present in the room.
|love       |`<@username>` | Show someone how much you love him/them.!
|cookie      |`<@username>` | Give someone a cookie!
|disable     |`<command name>` | Disable a command.|Manager
|enable      |`<command name>` | Enable a command.|Manager
|english     |`<@username>` | Notify a user in their language to speak English if it is required.|Bouncer
|kick        |`@username`| Bans a user from the room and unbans them 2.5 seconds later, simulating a kick.|Manager
|gif         |`<tags>`| Grabs a random image from Giphy with the given tags. 2s cooldown.
|help        |`<chat command name>`| Returns the description of a command.
|jointime    |`[@username\|#userID]` | Returns amount of time since the given user entered the room. Gets your own info if no valid argument.
|link        || Returns the link of the song currently playing.
|props       || Show some appreciation for the DJ!
|roll        |[`<1-10>\|<1-20d1-999999999>]` | Returns a random number with given amount of digits, or rolls dice. Default: 2 digits.
|seentime    |`[@username\|#userID]` | Returns the total amount of time a user has been seen in the room. Gets your own info if no valid argument.
|set         |`<option>` `<value>` | Sets a bot option to the given value. If no value is given, returns the current value of it. List of valid options: https://git.io/vM9aD|Manager
|shots, shot |`[@username]` | Buy a random shot for a user!
|skip        |`[reason]` | Skips current song with optional reason, if valid.|Bouncer
|skipreasons || Lists reasons that can be used with !skip.|Bouncer
|stats       |`[@username\|#userID]` | Returns the user's recorded amount of plays and votes received. Gets your own info if no valid argument.
|swap        |`@user1` `@user2` | Swaps positions of two users in the waitlist. At least one must be in the waitlist.|Manager
|trigger     || Returns current trigger of the bot. This can be called with any valid trigger character.
|uptime      || Returns uptime of this bot.




### set command option 
  
  |Command                   |Option   |Description|

|autoWoot                 |`true` \| `false`|If true, automatically woots when a new song is played.
|welcomeUsers             |`true` \| `false`|If true, welcomes users joining the room.
|chatDeleteTriggerMessages|`true` \| `false`|If true, deletes messages beginning with the bot\'s trigger.
|chatDeleteResponses      |`true` \| `false`|If true, deletes responses to !afkdisable and !joindisable.
|announcementInterval     |`Number` **(MILLISECONDS)**|Amount of time between announcements in MILLISECONDS, must be above 5000. Default is 1800000 (30 minutes). Will restart the timer when this is changed.
|announcementRandom       |`true` \| `false`|If true, selects random announcements to send. If false, sends them in the order they are listed.
|sendAnnouncements        |`true` \| `false`|If true, sends announcements.
|useMessageCommands       |`true` \| `false`|If true, allows message commands to be used (such as shuffle, fav, rules, theme, etc)
|doAFKCheck               |`true` \| `false`|If true, checks for AFK users on the waitlist and removes them.
|doRoulette               |`true` \| `false`|If true, begins a roulette every hour.
|doAutoDisable            |`true` \| `false`|If true, sends the "!afkdisable" and "!joindisable" messages every hour.
|autoStuckSkip            |`true` \| `false`|If true, checks to see if a song is playing 60 seconds past its actual length and skips it if it is.
|doSkipCheck              |`true` \| `false`|If true, checks to see if a song should be skipped based on history/blacklist/etc. Will **NOT** skip the song, but is required to be true for doAutoSkip to work.
|doAutoSkip               |`true` \| `false`|If true, autoskips songs if they are found in history/blacklists/etc. Requires doSkipCheck to be true.
|hostBypassAutoSkip       |`true` \| `false`|If true, the host of the room can bypass autoskip conditions unless the song is unavailable.
|sendMOTD                 |`true` \| `false`|If true, sends the MOTD.
|motdInterval             |`Number` **(MILLISECONDS)**|Amount of time between MOTD messages in MILLISECONDS, must be above 5000. Default is 1800000 (30 minutes). Restarts the timer if changed.
|motd                     |`string`         |The MOTD message.
