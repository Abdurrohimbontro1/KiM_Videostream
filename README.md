# Telegram Kim Video Stream Bot (KIM VIDEO BOT)

![GitHub Repo stars](https://img.shields.io/github/stars/abdurrohimbontro/kimvideostream?color=blue&style=flat)

Telegram Bot  [KIM VIDEO BOT](https://t.me/kimvideo_bot) bot yang di gunakan untuk memutar video di obrolan video grup anda

## Fitur spesial

- Daftar putar, antrean, streaming langsung 24x7
- Mendukung streaming langsung dari youtube
- Mulai streaming langsung jika tidak ada lagu di daftar putar
- Pemutaran otomatis bahkan jika heroku dimulai ulang
- Tampilkan posisi pemutaran audio saat ini
- Ubah judul obrolan Suara menjadi nama lagu yang sedang diputar
- Secara otomatis mengunduh audio untuk dua trek pertama dalam daftar putar untuk memastikan pemutaran yang lancar

## Deploy Bot 

### Heroku (The Easiest Way)
<p><a href="https://heroku.com/deploy?template=https://github.com/abdurrohimbontro/kimvideostream/tree/master"><img src="https://img.shields.io/badge/Deploy%20KIM%20VIDEO BOT-blueviolet?style=for-the-badge&logo=heroku" width="200""/></a></p>

### Railway (At Your Own Risk)
<p><a href="https://railway.app/new/template?template=https%3A%2F%2Fgithub.com%2Fabdurrohimbontro%2Fkimvideostream%2Ftree%2Fmaster&envs=API_ID%2CAPI_HASH%2CBOT_TOKEN%2CSESSION_STRING%2CCHAT_ID%2CLOG_GROUP%2CAUTH_USERS%2CADMIN_ONLY%2CSTARTUP_STREAM%2CREPLY_MESSAGE&optionalEnvs=LOG_GROUP%2CADMIN_ONLY%2CREPLY_MESSAGE&API_IDDesc=Your+Telegram+API_ID+get+it+from+my.telegram.org%2Fapps&API_HASHDesc=Your+Telegram+API_HASH+get+it+from+my.telegram.org%2Fapps&BOT_TOKENDesc=Bot+token+of+your+bot%2C+get+from+%40Botfather&SESSION_STRINGDesc=Session+string%2C+use+%40https://replit.com/@ZauteKm/GenerateStringSession+to+generate+pyrogram+session+string&CHAT_IDDesc=ID+of+Channel+or+Group+where+the+Bot+plays+Live%2FMusic%2FYouTube+Lives&LOG_GROUPDesc=ID+of+the+group+to+send+playlist+if+CHAT+is+a+Group%2C+if+channel+then+leave+blank&AUTH_USERSDesc=ID+of+Users+who+can+use+Admin+commands+%28for+multiple+users+seperated+by+space%29&ADMIN_ONLYDesc=Change+it+to+%27True%27+If+you+want+to+make+%2Fplay+commands+only+for+admins+of+CHAT.+By+default+%2Fplay+is+available+for+all&STARTUP_STREAMDesc=URL+of+Live+Stream+or+Youtube+Live+video+link+to+stream+with+bootup&REPLY_MESSAGEDesc=A+reply+message+to+those+who+message+the+USER+account+in+PM.+Make+it+blank+if+you+do+not+need+this+feature.&ADMIN_ONLYDefault=False&STREAM_URLDefault=https://youtu.be/36YnV9STBqc&REPLY_MESSAGEDefault=Hello Sir, I'm a bot to stream videos on telegram voice chat, not having time to chat with you 😂!"> <img src="https://img.shields.io/badge/Deploy%20to%20Railway-blueviolet?style=for-the-badge&logo=railway" width="200""/></a></p>


## Konfigurasi Vars
1. `API_ID` : Akun Pengguna Telegram API_ID, dapatkan dari https://my.telegram.org
2. `API_HASH` : Akun Pengguna Telegram API_HASH, dapatkan dari https://my.telegram.org
3. `BOT_TOKEN` : Token Bot Telegram Anda, dapatkan dari [@Botfather](https://t.me/botfather) XD
4. `SESSION_STRING` : Pyrogram Session String Akun Pengguna, dapatkan dari [![GenerateStringSession](https://img.shields.io/badge/repl.it-GenerateStringSession-yellowgreen)](https://replit.com/@abdurrohimbontr/kim-1?v=1)
5. `CHAT_ID` : ID Saluran atau Grup tempat bot akan melakukan streaming video.
6. `LOG_GROUP` : Grup untuk mengirim Daftar Putar, jika CHAT_ID adalah Grup.
7. `AUTH_USERS` : ID Pengguna yang dapat menggunakan perintah Admin (untuk beberapa pengguna yang dipisahkan oleh spasi).
8. `REPLY_MESSAGE` : Balasan kepada mereka yang mengirim pesan ke akun USER di PM. Biarkan kosong jika Anda tidak membutuhkan fitur ini.
9. `ADMIN_ONLY` : Pass 'True' Jika Anda ingin membuat perintah /play hanya untuk admin. Secara default /play tersedia untuk semua.
10. `STARTUP_STREAM` : URL streaming stasiun langsung atau video langsung youtube untuk streaming saat bot dimulai.
11. `HEROKU_API_KEY`: Kunci api Heroku Anda. Dapatkan dari [di sini](https://dashboard.heroku.com/account)
12. `HEROKU_APP_NAME`: Nama aplikasi Heroku Anda jika di-deploy ke heroku.
13. `IS_NONSTOP_STREAM`: Ubah ke 'False' Jika Anda ingin menonaktifkan fitur streaming langsung 24x7 nonstop. Secara default diaktifkan.

## Requirements
- Python 3.6 or Higher.
- Latest [FFmpeg](https://www.ffmpeg.org/).
- [Telegram API Key](https://docs.pyrogram.org/intro/quickstart#enjoy-the-api).
- Pyrogram [String Session](https://replit.com/@abdurrohimbontr/kim-1?v=1) Of The Account.
- The User Account Needs To Be An Admin In The Group / Channel.

## Self Host
```sh
$ git clone -b master https://github.com/ZauteKm/VideoStreamBot
$ cd VideoStreamBot
$ sudo apt install git curl python3-pip ffmpeg -y
$ pip3 install -U pip
$ curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -
$ sudo apt install -y nodejs
$ sudo apt install build-essential
$ sudo npm install pm2@latest -g
$ pip3 install -U -r requirements.txt
# <create .env variables appropriately>
$ python3 main.py
```

##
