# [Penumbuk Api BOT](https://penumbukapi.net/)

This is bot modified by me based on open-source bot below  
[Sat's Splinterlands Bot](https://satelliting.github.io/Sats-Splinterlands-Bot/)

# Feature

* Play multi account with 1 bot.  
* Hardcode the team when DATABASE don't have team to submit.  
* Skip daily focus if not in selected splinter.  
* Selected splinter burn ECR to meet minimun 1 focus chest for that day focus. (Premium)  
* Counter opponent summoners based on last 5 battles. ( Premium )  
* 20% more priority for selected splinter to submit the team. ( Premium )  
* Battle history based on leaderboard player. ( Premium )  
* Will fill out empty slot with Fiend cards. ( Premium )
* Will fill out empty slot with Chaos Agent if have extra 1 mana. ( Premium )

# Config

### Ranked Config ###
# Play Modern or Wild 'MODERN' / 'WILD'
MODERN_WILD = 'MODERN'
# Time to wait for next battle (seconds)
BATTLE_INTERVAL = 5 # default is 600 (10 minutes)
# Min ECR % should be before battling
ECR_MIN = 75 # (do not add percentage)
# Max ECR % needs to be before battling
ECR_MAX = 98 # (do not add percentage)
# Prioritize Quest
PRIORITIZE_QUEST = True # True, False (case-insensitive)
# Min Daily Chest to obtain, work if PRIORITIZE_QUEST = True
CHEST_MIN = 1
# ECR % Limit to obtain CHEST_MIN, work if PRIORITIZE_QUEST = True
ECR_CHEST_MIN = 85
# Claim Daily Quest Reward
CLAIM_REWARD_QUEST = True # True, False (case-insensitive)
# Claim Season Reward
CLAIM_REWARD_SEASON = True # True, False (case-insensitive)
# Advance League
ADVANCE_LEAGUE = False # True, False (case-insensitive)
# Max League to advance, work if ADVANCE_LEAGUE = True
MAX_LEAGUE = 'BRONZE'
# Prioritize Rating
RATING_MODE = True # True, False (case-insensitive)
# Rating should be before stop
RATING = 700 # default is 1000 ( Silver III )
# this splinter will prioritize for normal battle if able
# ['Fire', 'Water', 'Earth', 'Life', 'Death', 'Dragon']
PRIORITIZE_SPLINTER_NORMAL = ['Death']
# Burn erc if Daily focus splinter is in PRIORITIZE_SPLINTER_NORMAL
ERC_BURN_MODE = False # True, False (case-insensitive)
# Burn ERC until % before stop, work if ERC_BURN_MODE = True
ECR_BURN_MIN = 50 # (do not add percentage)
# Renting individual cards list up in cardlist_XXX.txt, card level based on XXX value
# will renting if Daily focus splinter is in PRIORITIZE_SPLINTER_NORMAL
RENTING_MODE = False # True, False (case-insensitive)
# Renting if ECR % over this, work if RENTING_MODE = True
ECR_RENTING_MIN = 85 # (do not add percentage)
# Ban selected summoners
SUMMONER_BAN_MODE = False # True, False (case-insensitive)
# Summoner Id to ban, work if SUMMONER_BAN_MODE = True
SUMMONER_BAN_ID = []

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
