THIS SCRIPT CAN PARSE TELEGRAM GROUPS (українська інструкція - у файлі README_ua.md)

1. Go to https://my.telegram.org and login
2. Press 'API development tools' and create a new application or go to step 3 if you already have one.
3. Copy your 'App api_id' and 'App api_hash' to the .env file (next to '=' sign, no spaces, just ctrl+v)
4. Run 'parse.exe'.
5. Follow the instructions in file you had open.
6. Phone number should be start with '+' and has international code (38 for UA). For example,
"+380123456789"
7. Enter the values in the app and get your result in .html file!
8. If you didn't get any result, check log.txt.
9. LIMIT - the bigger number you enter, more users you will get, but the script will run longer too.

Q: What each option means?

A: 1 - parse my channels - sending you list of the channels where you are member, 
then you select channel to parse
2 and 3 means equal to their description
4 - large parsing - this option allows you to get a large database by 1 parsing session
first you have to enter keyword, script will find some groups to parse
then you enter the limit (more limit=more users but more time for script to run)
then you get your data

Q: I get a .html file, it has header ('id', 'username' else) but it is empty

A: You've tried to parse a default channel. You can parse only channels with discussion/comments ON

Q: What is chat and what is channel?

A: Chat is a tg group where you communication with others. Channels is a tg group when you can't
reply to the messages in it. More: https://appsgeyser.com/blog/telegram-channel-vs-telegram-group/

Q: How can I know how many messages I should enter?

A: More messages means more time for channel to be parsed and more users you get.
If you want to parse from tg channel, there is only one method: to parse chat, where people
have replied to the message in channel. If you want to change the limit of 50 messages max,
go to .env file and change 'MAX_MESSAGES'. 

QUESTIONS, DEALS, EVERYTHING: raskolbrd@gmail.com
