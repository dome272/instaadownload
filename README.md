# instaadownload - An automated instagram downloading bot running in-platform


### What is "instaadownload"?:
    "instaadownload" is a bot running on a separate instagram account which people can send posts to and afterwards
    receive the posts as a downloadable version. The initial idea was to have an easy, in-platform way of
    downloading videos. Later this was further developed to download stories, profile pictures and images as well.
    Instaadownload started with a few subscribers and a small number of downloads a day. It quickly gained a lot of
    attraction and grew to 20.000 followers with more than 30.000 downloads a day. After enjoying so much attention,
    Instagram noticed it too and banned it as a result of violating the Tos. Further tries to build up news downloader
    for the community also resulted in these accounts being banned.
    We decided to make the code public so other people could make their own private or public downloader for their
    community. 

Requirements:
- [Python 3](https://www.python.org/downloads/)
- [FFMPEG](https://ffmpeg.org/download.html) (installed and added to the PATH variable)

Setup:
1. Clone the repo
2. Edit the InstagramDownloader.py file. At the bottom should be a username and a password variable
3. search for self.admins and put in the usernames you want to be admins
4. install the requirements (pip install -r requirements.txt) in the correct folder
5. run python InstagramDownloader.py and wait for 3 logins to happen


## Admincommands: (if youre in the self.admins)
### Priority
- !upgrade [user]
- !downgrade [user]

### Antispam:
- !remove [username] (removes queue items from given username)

### Other
- !delay - avg delay by priority level
- !reset - resets the delay log

- !most - user with most items in queue (used to find spammers)

- !day - downloads of the day (bugging and sometimes switches the current day and the next day)
