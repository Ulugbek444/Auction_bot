# Auction_bot
# Car Auction Bot
This Telegram bot allows users to create and participate in car auctions. Users can describe the load, set a price, choose a currency, and specify the auction duration. The bot includes features such as bidding, auction end notifications, and sharing auction details.
## Prerequisites
Before running the bot, make sure you have the following:

### 1. Python: The bot is written in Python, so you need to have Python installed on your machine. You can download Python from python.org.

### 2. Telegram Bot Token: You need to create a Telegram bot and obtain the bot token. Follow the instructions (https://helpdesk.bitrix24.ru/open/17538378/) to create a new bot and get the token.

### 3. ImgBB Token: The bot uses ImgBB to store images. You need to sign up on ImgBB and obtain the API token.
# Installation
## The bot was created in the 3.12 version of python
1. You should download the (telebotAPI)library, other imports are built-in libraries.
   For this you need to open your terminal and enter the following commands:
   1. pip install pyTelegramBotAPI
2. Open the auction_bot.py file in a text editor.
   Replace 'YOUR_TELEGRAM_BOT_TOKEN' with the token you obtained from the BotFather:
   ### bot = telebot.TeleBot('YOUR_TELEGRAM_BOT_TOKEN')
6. Replace 'YOUR_IMGBB_TOKEN' with the ImgBB API token:
   ### imgbb_token = 'YOUR_IMGBB_TOKEN'
## Commands
•	/help: Displays instructions for using the bot.
•	/start or /restart: Starts the bot and provides a brief introduction.
## How to Use
1.	Start the bot using the command /start.
2.	Select the "Create an auction" button to initiate a new auction.
3.	Follow the prompts to describe the load, set the price, choose a currency, and select the auction duration.
4.	Send a photo of the load.
5.	Participants can bid on the auction using predefined bid buttons (+100, +1000, +2000, +3000, +5000).
6.	The auction ends automatically after the specified duration.
7.	The winner is notified, and participants can share the auction details.
## Inline Queries
Users can share auction details by using the "Share" button, which generates a shareable link with the current price and load description.
## Functions
### is_admin(chat_id, user_id): Check if a user is an admin.
### has_time_passed(chat_id): Check if the auction timer has expired.
### process_description(message): Process the auction description.
### choose_currency(call): Choose the currency for the auction.
### handle_callback_query(call): Handle callback queries for various actions.
### get_photo(message): Process the photo sent by the user for the auction.
### delete_photos_after_delay(photo_directory, delay_seconds): Delete photos older than a specified duration.
### auction_end_callback(chat_id): Handle actions when the auction ends.
### choose_time(message): Choose the duration of the auction.
### update_share_button_price(chat_id, new_price): Update the share button with the new price.
### buttons_auction(message): Display buttons for auction actions.
### get_end_time_for_user(chat_id): Get the end time of the auction for a user.
### save_to_context(chat_id, key, value): Save data to the context.
## Important Notes
•	Admin privileges are required for certain commands and operations.
•	The bot handles errors and provides relevant messages to users.
•	Auctions automatically end after the specified duration.
### Note: Replace the placeholder logic in the is_admin function with your own admin privilege verification.
Feel free to customize the bot further based on your requirements. For any assistance or issues, contact the bot administrator.
## The bot was created in the 3.12 version of python
1. You should download the (telebotAPI) and (threading) libraries, other imports are built-in libraries.
   For this you need to open your terminal and enter the following commands:
   1. pip install pyTelegramBotAPI
   2. pip install threading


