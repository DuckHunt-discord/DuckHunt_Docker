# DuckHunt docker install

Files used to run DuckHunt V4 in production. This should give you a head start if you want to selfhost the bot.
Remember to keep credit, and to only run private instances of the bot.

PRs (Pull Requests) are **welcome** on every repository under the Duckhunt org.
If you see something that could be improved, please take the time to contribute back to the project.

If you are willing to selfhost the bot, please give yourself the Selfhoster role and stay in the DuckHunt support server.

## Install

Create a file named .env

```dotenv
BOT_TOKEN="YOUR.BOT.TOKEN.FROM.DISCORD.HERE"
GLOBAL_API_KEY="AN.UUID4.YOU.GENERATED.SOMEHOW"
```

Edit the Caddyfile to set your domain for the api/webinterface.
You can have localhost if you don't want to use them, but at that point, why are you even using this ?

Then run

```shell
docker-compose up -d --build
```

To deploy the website