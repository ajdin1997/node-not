## Plug dj bot writed in node.js with commands

### Commands

|Command Name |Arguments |Description |Minimum Rank |

|match      |`<@username>` | Check are you compatible with others person | User
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
