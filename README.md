# TelegramConnector
Mudlet Package that integrates with Telegram

## Commands

| Command                                    | API | Comment      |
| -------                                    | --- | --------     |
| \#HELP                                     |     | Helpfile     |
| \#VERSION                                  |     | Version info |
| \#TELEGRAM                                 |     | Package Status |
| \#TELEGRAM STATUS                          | Telegram:showStatus()  | Package Status |
| \#TELEGRAM VERSION                         | Telegram:showVersion() | Version info |
| \#TELEGRAM HELP                            | Telegram:showHelp() | Helpfile     |
| \#TELEGRAM UPGRADE                         | Telegram:downloadLatestVersion() | Upgrade the package        |
| \#TELEGRAM TOKEN &lt;token&gt;                   | Telegram:SetToken(token)  | Set Telegram Token"             |
| \#TELEGRAM INTERVAL &lt;seconds&gt;              | Telegram:SetInterval(5)   | Set polling interval, default 10s             |
| \#TELEGRAM ENABLE                          |  | Enable the package   |
| \#TELEGRAM DISABLE                         |  | Disable the package    |
| \#TELEGRAM TELL &lt;username&gt; &lt;message&gt;       | Telegram:Tell("takilara","Someone is attacking me!!!") | Send a message to a telegram user    |
| \#TELEGRAM WHISPER &lt;username&gt; &lt;message&gt;    | Telegram:Tell("takilara","This message will get delivered without notification",true) | Send a message to a telegram user (no notification)    |
| \#TELEGRAM AUTH &lt;username&gt;                 |  | Authorize a Telegram user    |
| \#TELEGRAM UNAUTH &lt;username&gt;               |  | UnAuthorize a Telegram user    |

The #&lt;COMMAND&gt; commands are meant to be used from within the game. To use these mechanics in scripts or aliases, use the API commands

## Setup

1. Install the Package
1. Open telegram and open a chat with @botfather
1. Run the command /newbot in telegram, i recommend giving it a name that in part matches the character that you will be linking to (e.g. mymud_gandalf_bot)
1. Go to Mudlet, type #TELEGRAM TOKEN &lt;paste_the_token_here&gt;
1. Run the command /mybots, then click the bot, -> Bot Settings ->  Group Privacy -> Turn off
 (this is only required if you intend to add your bot to a chat group)
1. Open a chat with the bot, and run the command /start
1. Try a command like 'look', The bot will reply telling you: User '&lt;yourusername&gt;' not authorized
1. In Mudlet you should now see a message about unauthorized user, run the command #TELEGRAM AUTH &lt;yourusername&gt; 
1. Repeat the command 'look', it should now work
1. In Mudlet, also try '#TELEGRAM TELL &lt;yourusername&gt; some message' and it should show up in Telegram

## TODO
* Versioning
* Packaging
* Update from the script


