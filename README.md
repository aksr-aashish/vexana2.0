<p align="center">
  <img src="https://telegra.ph/file/4a7d5037bcdd1e74a517a.jpg">
</p>

<h3 align="center"><b>✨ Vexana RoBot ✨</b></h9>

<h6 align="center">A Powerful, Smart And Simple Group Manager <br> ... Written with AioGram , Pyrogram and Telethon...</h4>
<p align='center'>
  <a href="https://www.python.org/" alt="made-with-python"> <img src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg?style=flat-square&logo=python&color=blue" /> </a>
  <a href="https://github.com/aksr-aashish/vexana2.0/tree/patch1.0/graphs/commit-activity" alt="Maintenance"> <img src="https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=flat-square" /> </a> 
</p>


### Click Below Image To Deploy On
### 💙 Heroku 💙
<p align="center"><a href="https://heroku.com/deploy?template=https://github.com/aksr-aashish/vexana1.0/tree/patch1.0.git"><img src="https://telegra.ph/file/4a7d5037bcdd1e74a517a.jpg" width="50"></a></p>
<p align="center">
<a href="https://app.codacy.com/manual/aksr-aashish/aksr-aashish/vexana1.0/dashboard"> <img src="https://img.shields.io/codacy/grade/4d58f2a402b54aed8a7d95f7add45a81?color=brightgreen&logo=codacy&logoColor=green&style=for-the-badge" alt="Codacy" /></a>
    <a href="https://github.com/aksr-aashish/vexana2.0"> <img src="https://img.shields.io/github/repo-size/aksr-aashish/vexana2.0?color=orange&logo=github&logoColor=green&style=for-the-badge" /></a>
    <a href="https://github.com/aksr-aashish/vexana2.0/commits/aksr-aashish"> <img src="https://img.shields.io/github/last-commit/aksr-aashish/vexana2.0?color=brown&logo=github&logoColor=green&style=for-the-badge" /></a>
    <a href="https://github.com/aksr-aashish/vexana2.0/issues"> <img src="https://img.shields.io/github/issues/aksr-aashish/vexana2.0?color=blueviolet&logo=github&logoColor=green&style=for-the-badge" /></a>
    <a href="https://github.com/aksr-aashish/vexana2.0/network/members"> <img src="https://img.shields.io/github/forks/aksr-aashish/vexana2.0?color=red&logo=github&logoColor=green&style=for-the-badge" /></a>  
    <a href="https://pypi.org/project/Telethon/"> <img src="https://img.shields.io/pypi/v/telethon?color=yellow&label=telethon&logo=python&logoColor=green&style=for-the-badge" /></a>
</p>



<h6 align="center"><b>⭐ If You like our repo and enjoyed the bot Plz Consider Giving Us A Star⭐ </b></h9>

## Available On Telegram As [Vexana_Robot](https://t.me/vexana_robot) 💜

## How to setup/deploy.



<details>
  <summary>Steps to deploy on Heroku !! </summary>

```
Fill in all the details, Deploy!
Now go to https://dashboard.heroku.com/apps/(app-name)/resources ( Replace (app-name) with your app name )
Turn on worker dyno (Don't worry It's free :D) & Webhook
Now send the bot /start, If it doesn't respond go to https://dashboard.heroku.com/apps/(app-name)/settings and remove webhook and port.
```

[![Deploy To Heroku](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?button-url=https%3A%2F%2Fgithub.com%2Faksr-aashish%2Fvexana&template=https%3A%2F%2Fgithub.com%2FAnuragSharma080%2Fvexana1.0)



</details>  
<details>
  <summary>Steps to self Host!! </summary>

  ## Setting up the bot (Read this before trying to use!):
Please make sure to use python3.6, as I cannot guarantee everything will work as expected on older Python versions!
This is because markdown parsing is done by iterating through a dict, which is ordered by default in 3.6.

  ### Configuration

There are two possible ways of configuring your bot: a config.py file, or ENV variables.

The preferred version is to use a `config.py` file, as it makes it easier to see all your settings grouped together.
This file should be placed in your `VexanaRoBot` folder, alongside the `__main__.py` file. 
This is where your bot token will be loaded from, as well as your database URI (if you're using a database), and most of 
your other settings.

It is recommended to import sample_config and extend the Config class, as this will ensure your config contains all 
defaults set in the sample_config, hence making it easier to upgrade.

An example `config.py` file could be:
```
from Vexana.sample_config import Config
  class Development(Config):
    OWNER_ID = 1332331113  # your telegram ID
    OWNER_USERNAME = "Pain_to_this_world"  # your telegram username
    API_KEY = "your bot api key"  # your api key, as provided by the @botfather
    SQLALCHEMY_DATABASE_URI = 'postgresql://username:password@localhost:5432/database'  # sample db credentials
    MESSAGE_DUMP = '-1234567890' # some group chat that your bot is a member of
    USE_MESSAGE_DUMP = True
    SUDO_USERS = [1332331113, 1656709282]  # List of id's for users which have sudo access to the bot.
    LOAD = []
    NO_LOAD = ['translation']
```

If you can't have a config.py file (EG on Heroku), it is also possible to use environment variables.
The following env variables are supported:
 - `ENV`: Setting this to ANYTHING will enable env variables

 - `TOKEN`: Your bot token, as a string.
 - `OWNER_ID`: An integer of consisting of your owner ID
 - `OWNER_USERNAME`: Your username

 - `DATABASE_URL`: Your database URL
 - `MESSAGE_DUMP`: optional: a chat where your replied saved messages are stored, to stop people deleting their old 
 - `LOAD`: Space-separated list of modules you would like to load
 - `NO_LOAD`: Space-separated list of modules you would like NOT to load
 - `WEBHOOK`: Setting this to ANYTHING will enable webhooks when in env mode
 messages
 - `URL`: The URL your webhook should connect to (only needed for webhook mode)
  - `SUDO_USERS`: A space-separated list of user_ids which should be considered sudo users
 - `SUPPORT_USERS`: A space-separated list of user_ids which should be considered support users (can gban/ungban,
 nothing else)
 - `WHITELIST_USERS`: A space-separated list of user_ids which should be considered whitelisted - they can't be banned.
 - `DONATION_LINK`: Optional: link where you would like to receive donations.
 - `CERT_PATH`: Path to your webhook certificate
 - `PORT`: Port to use for your webhooks
 - `DEL_CMDS`: Whether to delete commands from users which don't have rights to use that command
 - `STRICT_GBAN`: Enforce gbans across new groups as well as old groups. When a gbanned user talks, he will be banned.
 - `WORKERS`: Number of threads to use. 8 is the recommended (and default) amount, but your experience may vary.
 __Note__ that going crazy with more threads wont necessarily speed up your bot, given the large amount of sql data 
 accesses, and the way python asynchronous calls work.
 - `BAN_STICKER`: Which sticker to use when banning people.
 - `ALLOW_EXCL`: Whether to allow using exclamation marks ! for commands as well as /.

  ### Python dependencies

Install the necessary Python dependencies by moving to the project directory and running:

`pip3 install -r requirements.txt`.

This will install all the necessary python packages.
### Database

If you wish to use a database-dependent module (eg: locks, notes, userinfo, users, filters, welcomes),
you'll need to have a database installed on your system. I use Postgres, so I recommend using it for optimal compatibility.

In the case of Postgres, this is how you would set up a database on a Debian/ubuntu system. Other distributions may vary.

- install postgresql:

`sudo apt-get update && sudo apt-get install postgresql`

- change to the Postgres user:

`sudo su - postgres`

- create a new database user (change YOUR_USER appropriately):

`createuser -P -s -e YOUR_USER`

This will be followed by you need to input your password.

- create a new database table:

`createdb -O YOUR_USER YOUR_DB_NAME`

Change YOUR_USER and YOUR_DB_NAME appropriately.

- finally:

`psql YOUR_DB_NAME -h YOUR_HOST YOUR_USER`

This will allow you to connect to your database via your terminal.
By default, YOUR_HOST should be 0.0.0.0:5432.

You should now be able to build your database URI. This will be:

`sqldbtype://username:pw@hostname:port/db_name`

Replace sqldbtype with whichever DB you're using (eg Postgres, MySQL, SQLite, etc)
repeat for your username, password, hostname (localhost?), port (5432?), and DB name.

  ## Modules
   ### Setting load order.

The module load order can be changed via the `LOAD` and `NO_LOAD` configuration settings.
These should both represent lists.

If `LOAD` is an empty list, all modules in `modules/` will be selected for loading by default.

If `NO_LOAD` is not present or is an empty list, all modules selected for loading will be loaded.

If a module is in both `LOAD` and `NO_LOAD`, the module will not be loaded - `NO_LOAD` takes priority.

     ### Creating your own modules.

Creating a module has been simplified as much as possible - but do not hesitate to suggest further simplification.

All that is needed is that your .py file is in the modules folder.

To add commands, make sure to import the dispatcher via

`from MizuharaSmexyBot import dispatcher`.

You can then add commands using the usual

`dispatcher.add_handler()`.

Assigning the `__help__` variable to a string describing this modules' available
commands will allow the bot to load it and add the documentation for
your module to the `/help` command. Setting the `__mod_name__` variable will also allow you to use a nicer, user-friendly name for a module.

The `__migrate__()` function is used for migrating chats - when a chat is upgraded to a supergroup, the ID changes, so 
it is necessary to migrate it in the DB.

The `__stats__()` function is for retrieving module statistics, eg number of users, number of chats. This is accessed 
through the `/stats` command, which is only available to the bot owner.

## Starting the bot.

Once you've set up your database and your configuration is complete, simply run the bat file(if on windows) or run (Linux):

`python3 -m Vexana`

You can use [nssm](https://nssm.cc/usage) to install the bot as service on windows and set it to restart on /gitpull 
Make sure to edit the start and restart bats to your needs. 
Note: the restart bat requires that User account control be disabled.

For queries or any issues regarding the bot please open an issue ticket or visit us at [Support](https://t.m/PAIN_TO_THIS_WORLD)
## How to setup on Heroku 
For starters click on this button 
</details>  

## Support 💜

<a href="https://t.me/Vexana_updates"><img src="https://img.shields.io/badge/Join-Updates%20Channel-violet.svg?logo=Telegram"></a>

<a href="https://t.me/vexana_support"><img src="https://img.shields.io/badge/Join-Support%20Group-purple.svg?logo=telegram"></a>

### Inspired From

•[SaitamaRobot](https://github.com/animekaizoku/saitamarobot)

•[LaylaRobot](https://github.com/queenarzoo/LaylaRobot)

•[DaisyX](https://github.com/TeamDaisyX/DaisyX)

### Original Works Of
•[WilliamButcherBot](https://github.com/TheHamkerCat/WilliamButcherBot)

•[SaitamaRobot](https://github.com/animekaizoku/saitamarobot)

•[LaylaRobot](https://github.com/queenarzoo/LaylaRobot)

•[DaisyX](https://github.com/TeamDaisyX/DaisyX)

•[Trojhanz](https://github.com/TroJanzHEX/Image-Editor) For Image Editor

•[TgCalls](https://github.com/MarshalX/tgcalls) For VC Player

•[AsmSafone](https://github.com/AsmSafon) For Many Things

•[EveryThingSuckz](https://t.me/EveryThingSuckz) For NSFW Watch


### ALL DEVS AND Contributors ❤

#### • AXEL  (aksr-aashish)    »»  <a href="https://github.com/aksr-aashish" alt="aksr0aashish"> <img src="https://img.shields.io/badge/AXEL-90302f?logo=github" /></a> (OWNER)

#### • Anand »»  <a href="https://github.com/Stella-80" alt="Akeno"> <img src="https://img.shields.io/badge/Akeno-95B9C7?logo=github" /></a> (Dev)
#### • Aashish »»  <a href="https://github.com/aksr-aashish" alt="Aashish "> <img src="https://img.shields.io/badge/Aashish-95B9C7?logo=github" /></a> (Dev)
#### • Asmita »»  <a href="https://github.com/asmita" alt="asmita"> <img src="https://img.shields.io/badge/asmita-107D8D?logo=github" /></a> (DEV)
