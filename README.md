# bytetorrent-plus

[bytetorrent-plus](https://github.com/bytetorrent-plus/bytetorrent-plus) is a new generation of bittorrent applications that are built on the [bytetrade blockchain](https://www.bytetrade.io/) and and [libtorrent](https://github.com/arvidn/libtorrent).
 It works on iOS, Android, OS X, Windows and Linux Server.


### Linux Version

You need to go to the bytetrade website to create an account and enter the command:
```
sudo docker run -itd --net=host -v /tmp/s1/run:/opt/run -e
BTP_USERNAME=$userid -e BTP_PRIVATE=$priv_key -e BTP_CLIENT_PORT=7655
libtorrent/bytetorrent
```

You can check the status of the server through the client.
```
ID=$(sudo docker run -itd --net=host libtorrent/bytetorrent-client 127.0.0.1 7655)
sudo docker attach $ID
```
To detach from a running container, use ^P^Q (hold the Ctrl, press P, press Q, release Ctrl).

### Where to get help
* [Explorer](https://explorer.bytetrade.com/)
* [Telegram](https://t.me/bytetorrentplus)
* [Issues Tracker](https://github.com/bytetorrent-plus/bytetorrent-plus/issues)
