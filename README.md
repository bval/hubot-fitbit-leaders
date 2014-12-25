# Hubot Fitbit Leaders [![npm version](https://badge.fury.io/js/hubot-fitbit-leaders.svg)](http://badge.fury.io/js/hubot-fitbit-leaders) [![Build Status](https://travis-ci.org/hubot-scripts/hubot-fitbit-leaders.png)](https://travis-ci.org/hubot-scripts/hubot-fitbit-leaders)

This script is designed to be used with a [Hubot](http://hubot.github.com) to compare the Fitbit activity of your friends.

## Suggested Setup

* Decide whether you want to use a user account or create a "robot" account to use with Fitbit
* Register a new Fitbit application with whichever you selected in the previous step, noting the `FITBIT_CLIENT_ID` and FITBIT_CLIENT_SECRET`.
* Using the supplied OAuth credentials from registration, obtain a `FITBIT_OAUTH_TOKEN` and `FITBIT_OAUTH_TOKEN_SECRET` by manually walking through the OAuth process (use a tool like [Runscope](https://www.runscope.com/) to make this a bit easier).
* Register the four values as environment variables when starting your bot (as usual with Hubot scripts).
 * `export FITBIT_CLIENT_ID=theclientid`
 * `export FITBIT_CLIENT_SECRET=theclientsecret`
 * `export FITBIT_OAUTH_TOKEN=theoauthtoken`
 * `export FITBIT_OAUTH_TOKEN_SECRET=theoauthtokensecret`

If you are using Heroku to host your bot, replace `export ...` with `heroku set:config ...`.

## Adding to Your Hubot

See full instructions [here](https://github.com/github/hubot/blob/master/docs/scripting.md#npm-packages).

1. `npm install hubot-fitbit-leaders --save` (updates your `package.json` file)
2. Open the `external-scripts.json` file in the root directory (you may need to create this file) and add an entry to the array (e.g. `[ 'hubot-fitbit-leaders' ]`).

## Commands

- `hubot fitbit leaders` - Show table of leaders
- `hubot fitbit register` - Show how to friend the bot
- `hubot fitbit approve` - Approve all pending requests
