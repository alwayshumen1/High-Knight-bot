# lichess-bot

Engine communication code taken from https://github.com/ShailChoksi/lichess-bot by [ShailChoksi](https://github.com/ShailChoksi)

###CHESS ENGINES 

Stockfish 14+(dev) POPCNT + SSE41
Multi-Variants Stcofkih14+dev

### Polyglot Opening Books

- .bin for Standard Chess

### How to Use

- [Fork](https://github.com/The-bot-makers/Lichess-bot/fork) this repository.
- Create a [new heroku app](https://dashboard.heroku.com/new-app).
- Go to the `Deploy` tab and click `Connect to GitHub`.
- Click on `search` and then select your fork of this repository.
- Then `Enable Automatic Deploys` and then select the `main` branch (which is already done by default usually) and Click `Deploy`.
- Once it has been deployed, go to `Resources` tab on heroku and enable `worker (bash startbot.sh)` dynos. (Do note that if you don't see any dynos in the `Resources` tab, then you must wait for about 5 minutes and then refresh your heroku page.)
- Finally go to your `Settings` tab and then under `Config Vars` click on `Reveal Config Vars` and then in the place of `key` type in `LICHESS_BOT_TOKEN` and in the place of `value` add your Lichess Bot Token.
- You're now connected to lichess and awaiting challenges! Your bot is up and ready!
