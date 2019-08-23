# bytetorrent-plus

[bytetorrent-plus](https://github.com/bytetorrent-plus/bytetorrent-plus) is a new generation of bittorrent applications that are built on the [bytetrade blockchain](https://www.bytetrade.io/) and and [libtorrent](https://github.com/arvidn/libtorrent).
 It works on iOS, Android, OS X, Windows and Linux Server.

### Windows Version

Click to download the [Windows client](https://cdn2.bytetrade.io/bytetorrent/windows/bytetorrent-0.1.0-2019-8-24.zip), which provides download and seeding function. You can find the free torrent file of TED conferences on the ByteTorrent website, and start download to experience the product. Please visit the Help Center for [tutorials](https://bytetorrent.zendesk.com/hc/en-us/articles/360034522833-ByteTorrent-Plus-Windows-Tutorial).

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
