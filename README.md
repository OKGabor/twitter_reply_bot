# Twitter Bot

## Description
This bot automatically replies to popular tweets about a certain topic without using the paid version of the X API.

## Features
- Scrapes tweets based on specific search terms
- Filters tweets by popularity (likes > 100)
- Avoids replying to the same tweet twice
- Stores replied tweet IDs in Google Drive

## Requirements
- Python 3.x
- tweepy
- ntscraper
- Google Colab (for Google Drive integration)

## Setup
1. Mount Google Drive in Colab
2. Set up a `replied_id.txt` file in your Google Drive
3. Replace the placeholder values in the `client` initialization with your X API credentials

## Usage
Run the script in a Google Colab notebook. The bot will:
1. Search for tweets about the selected topic
2. Reply to popular tweets that haven't been replied to before
3. Update the list of replied tweet IDs

## Configuration
- Modify `search_terms` to change the topics the bot looks for
- Adjust the `likes` threshold in the tweet filtering logic
- Customize the reply message in the `client.create_tweet()` function

## Caution
- Ensure compliance with Twitter's API terms of service
- Do not share your API credentials publicly
- Since ntscraper is not an official library of X, this bot is only for educational purposes

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Disclaimer
This bot is for educational purposes. Ensure you have the right to promote the mentioned website and that your use complies with all relevant terms of service and laws.
