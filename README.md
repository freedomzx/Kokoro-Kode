# Kokoro-Kode
A discord bot featuring small usabilities such as checking the weather via zipcode, a word of the day, checking stock history, and a game of hangman using the discord py api.

# Commands

### !8ball

Ask the bot any question, then it'll give you a random response.

Order: Send "!8ball", wait for bot response, respond with question, receive answer.

### !addcommand

Adds a new custom command to be stored by the bot in a MySQL server.

Order: Send "!addcommand", wait for bot response, respond with command name, wait for bot response, respond with command content, command will be stored.

### !define

Asks the bot to connect to the PyDictionary API to define a given (english) word.

Order: Send "!define <word>", bot will respond.
  
### !hangman

Starts a game of hangman!  Bot will pick a random word from the RandomWord API, then will send an ASCII image of the hangman board once ready.

Order: Send "!hangman", repeatedly send "!guess <word>" until either the users win or lose.
  
### !help

Causes the bot to respond with a list of commands, not including custom ones from !addcommand.

Order: Send "!help", get response.

### !randomword

Causes the bot to fetch a random word from the RandomWord API.

Order: Send "!randomword", get response.

### !roll

Roll a number between 1 and a given number.

Order: Send "!roll", wait for bot response, send a number n for the roll range cap, receive a random number from 1 to n.

### !rtd

Rolls a random number between 1 to 6.

Order: Send "!rtd", receive a random number from 1 to 6.

### !stocks

Gets stock information for a certain company's ticker.

Order: Send "!stocks", wait for bot response, send the ticker of the company to analyze stock data for, receive either an error message (cannot be found) or the stock information of the company.

### !translate

Translates any given words or sentences into a different language using the Google Translate API.

Order: Send "!translate", wait for bot response, send the phrase to be translated, wait for bot response, send the language code for the phrase to be translated to.

### !weather

Gives the weather (temperature, pressure, humidity) in any place in the world using the OpenWeather API.

Order: Send "!weather", wait for bot response, send zip code, wait for bot response, send country's 2 letter ISO code (instructions given from bot), receive weather information.

### Other commands

Other commands may be stored from other users using the !addcommand function, so ask around and see what exists!  The bot will check every message starting with a ! in the MySQL Database if it doesn't match any other command.