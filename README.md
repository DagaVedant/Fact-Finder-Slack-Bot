# Almanac Bot
![logo](images/logo.png)

A Slack bot I made that drops a daily batch of info into your channel. Each message has the word of the day, a fun fact, something that happened on this day in history, and a quote.

![Project Screenshot](images/screenshot.png)

[TRY IT HERE](http://app.slack.com/client/E09V59WQY1E/C0BBD17T3QB)

## Quick Start
Install the Slack app with the link above and run:

`/almanac-today`

That's it.

## Features
* **Daily Digest** - Everything in one command with `/almanac-today`
* **Word of the Day** - A new word (definition, part of speech, and sentence)
* **Fact of the Day** - A random fact every day
* **On This Day** - Historical events that happened today
* **Quote of the Day** - A quote

## Running Locally
### Prerequisites
* Node.js (v18+)
* npm

### 1. Clone the Repository
```bash
git clone https://github.com/DagaVedant/Almanac-Slack-Bot.git
cd Almanac-Slack-Bot
npm install
```

### 2. Configure Environment Variables
Create a `.env` file in the project folder and add your Slack credentials:
```env
SLACK_BOT_TOKEN=xoxb-your-bot-token
SLACK_APP_TOKEN=xapp-your-app-token
```

### 3. Start the Bot
```bash
node index.js
```

## How It Works
Almanac Bot is built with Node.js and Slack Bolt in Socket Mode.

The biggest challenge while building it was getting the bot to respond quickly and reliably. The first version that I made was using like 4 different APIs or something, and that just caused errors, timeouts, and delays, and like was a pain to deal with. So I just removed some of the features, and made each API run by itself, so if one fails, the others still work and it can still reply to the message.

## Tech Stack
* Node.js
* Slack Bolt for JavaScript
* Axios

## APIs Used
* Free Dictionary API
* Useless Facts API
* Wikipedia REST API
* ZenQuotes API

## What I Learned
I learned how to work with many APIs, handle different errors, and make Slack apps. I also learned how to use differnt sources and make it into one message.
