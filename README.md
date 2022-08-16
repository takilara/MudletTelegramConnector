# TelegramConnector
Mudlet Package that integrates with Telegram

## Commands

| Command                                    | Comment      |
| -------                                    | --------     |
| \#HELP                                     | Helpfile     |
| \#VERSION                                  | Version info |
| \#TELEGRAM                                 | Package Status |
| \#TELEGRAM STATUS                          | Package Status |
| \#TELEGRAM VERSION                         | Version info |
| \#TELEGRAM HELP                            | Helpfile     |
| \#TELEGRAM UPGRADE                         | Upgrade the package        |
| \#TELEGRAM TOKEN <token>                   |              |
| \#TELEGRAM INTERVAL <seconds>              |              |
| \#TELEGRAM ENABLE                          |     |
| \#TELEGRAM DISABLE                         |     |
| \#TELEGRAM TELL <username> <message> |     |
| \#TELEGRAM WHISPER <username> <message> |     |
| \#TELEGRAM AUTH <username> |     |
| \#TELEGRAM UNAUTH <username> |     |

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


