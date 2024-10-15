# X (Twitter) to Discord Webhook

This project sets up a webhook that listens for new posts from specified X (formerly Twitter) accounts and forwards them to a Discord channel.

## Prerequisites

- Python 3.7 or higher
- X (Twitter) Developer Account and API credentials
- Discord server with webhook setup

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/x-discord-webhook.git
   cd x-discord-webhook
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Copy the `.env.example` file to `.env` and fill in your credentials:
   ```
   cp .env.example .env
   ```

## Configuration

Edit the `.env` file and replace the placeholder values with your actual credentials:

- `CONSUMER_KEY`: Your X (Twitter) API consumer key
- `CONSUMER_SECRET`: Your X (Twitter) API consumer secret
- `ACCESS_TOKEN`: Your X (Twitter) API access token
- `ACCESS_TOKEN_SECRET`: Your X (Twitter) API access token secret
- `DISCORD_WEBHOOK_URL`: Your Discord webhook URL
- `X_USER_ID_TO_FOLLOW`: The X (Twitter) user ID you want to follow

## Usage

Run the script with:

```
python webhook.py
```

The script will start listening for new posts from the specified X account and send them to your Discord channel.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
