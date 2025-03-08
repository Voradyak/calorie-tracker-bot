# Calorie Tracker Telegram Bot

A Telegram bot that helps users track their daily calorie intake through photo recognition and manual entry.

## Features

- Photo-based food recognition
- Manual calorie entry
- Daily calorie summaries
- Meal logging reminders
- Persistent data storage using Supabase

## Setup

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Create a `.env` file with the following variables:
   ```
   TELEGRAM_BOT_TOKEN=your_bot_token
   SUPABASE_URL=your_supabase_url
   SUPABASE_KEY=your_supabase_key
   FOOD_API_KEY=your_food_recognition_api_key
   ```
4. Run the bot:
   ```bash
   python src/main.py
   ```

## Usage

1. Start the bot by sending `/start`
2. Upload a food photo or use `/add` to manually log food
3. View your daily summary with `/summary`
4. Get help anytime with `/help`

## Commands

- `/start` - Initialize the bot
- `/help` - Show help message
- `/add` - Manually add food and calories
- `/summary` - Get daily calorie summary
- `/settings` - Configure reminder settings

## Deployment

The bot can be deployed on Render or Railway.app. Follow their respective documentation for Python application deployment.

## Data Storage

The bot uses Supabase for data persistence. Required tables:
- users
- meals
- daily_logs

## Contributing

Feel free to submit issues and pull requests.

## License

MIT License 