# [Penumbuk Api BOT](https://penumbukapi.net/)

This is bot modified by me based on open-source bot below  
[Sat's Splinterlands Bot](https://satelliting.github.io/Sats-Splinterlands-Bot/)

# Feature

* Play multi account with 1 bot.  
* Hardcode the team when API don't have team to submit.  
* Skip daily focus if not in selected splinter.  
* Selected splinter burn ECR to meet minimun 1 focus chest for that day focus.  
* Counter opponent summoners based on last 5 battles. ( Premium )  
* 20% more priority for selected splinter to submit the team ( Premium )  
* Battle history based on leaderboard player ( Premium )  
* Will fill out empty slot with Fiend cards ( Premium )

# DATABASE

* To optimized the Bot performance, you need to maintain the database in your system.  
* Please follow below step to setup your mariaDB.  

1. Download [MariaDB Community Server](https://mariadb.com/downloads/community/community-server/)
    1. Follow instruction [here](https://mariadb.com/kb/en/installing-mariadb-msi-packages-on-windows/)

2. Install it and setup as below when prompt. 
    1. username = "root"
    2. password = "mariadb123"

3. Add mariaDB to PATH in Windows environment variables
    1. ```C:\Program Files\MariaDB 10.8\bin```
    2. Follow instruction [here](https://sebhastian.com/mysql-not-recognized-fix/)

4. Download [Cygwin](https://stackoverflow.com/questions/36733176/how-do-i-add-a-gzip-command-to-windows-cmd)

5. Follow instruction in page above to enable gzip command in Windows.

6. Run ```import_db.bat``` to export the BATTLEBASE.sql.gz

7. Daily updated BATTLEBASE.sql.gz available [here](https://drive.google.com/drive/folders/18lNewKqWz6AkJ3eWyXqHNsBxpdGE4uO4?usp=sharing)

# Installation

1. Download [Penumbuk Api Bot](https://drive.google.com/drive/folders/18lNewKqWz6AkJ3eWyXqHNsBxpdGE4uO4?usp=sharing)
    1. File size too big to put in Github.
    
2. Copy all files in config folder to parent directory.

3. Replace the setting in those files with your information.

4. Run the exe file.

# Premium

* 250 DEC per account per month
* Visit [Penumbuk Api Website](https://penumbukapi.net/) for payment details.

# Security

1. Posting key
    1. It will use to login into the game.

2. Active key
    1. It will use for guild contribution.
    2. You can leave it blank if not using for guild contribution.

3. Disclaimer
    1. The BOT will not sent over the posting/active key to me.
    2. Its will be use for above function only.
