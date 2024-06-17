# ExclusiveDropNotifierBot (**OUTDATED** &amp;&amp;  **DEFUNCT**)

![DiscordSnkRaPP](https://github.com/joelb429078/ExclusiveDropNotifierBot/assets/160978621/b4c18483-5f0e-4a9d-b9dc-21b563c8c7b4)


This project is a bot designed to purchase high-end releases from popular sites such as Nike's SNKRS, Solebox, FootLocker, and Supreme. The bot uses various libraries and techniques to efficiently monitor and secure purchases.

## Features

- **Site Scraping**: Scrapes product information from various e-commerce websites.
- **Proxy Rotation**: Uses rotating proxies to avoid IP bans and improve scraping efficiency.
- **User-Agent Rotation**: Randomly rotates user-agent strings to simulate different devices and browsers.
- **Discord Notifications**: Sends notifications via Discord webhooks for product availability and bot actions.
- **Keyword Matching**: Filters products based on specified keywords.
- **Duplicate Removal**: Removes duplicate entries to ensure accurate monitoring.
- **Logging**: Logs all bot actions and errors for monitoring and debugging.

## Technologies Used

- **Python**: Programming language for the bot.
- **requests**: Library for making HTTP requests.
- **youtube-dl**: Library for downloading YouTube videos (if used for Supreme or other media content).
- **pafy**: Library for handling YouTube content.
- **discord.py**: Library for Discord bot integration.
- **dotenv**: Library for managing environment variables.
- **random-user-agent**: Library for rotating user-agent strings.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/high-end-purchasing-bot.git
   ```
   
2. Navigate to the project directory:

   ```sh
   cd high-end-purchasing-bot
   ```

3. Install the required libraries:

   ```sh
   pip install -r requirements.txt
   ```


###Set up your environment variables in a .env file:

**env**

    USERNAME=your_discord_username
    AVATAR_URL=your_avatar_url
    COLOUR=your_embed_colour
    WEBHOOK=your_discord_webhook_url
    LOC=location_code
    LAN=language_code
    PROXY=your_proxy_list
    KEYWORDS=your_keywords
    DELAY=monitoring_delay

### Usage

    Ensure you have the latest versions of Python and the required libraries installed.
    Run then run whichever bot you want depending upon which website you want to Bot.

### Commands

    scrape_site: Scrapes the site and adds items to the inventory array.
    checker: Determines whether the product status has changed.
    test_webhook: Sends a test Discord webhook notification.
    discord_webhook: Sends a Discord webhook notification to the specified webhook URL.
    remove_duplicates: Removes duplicate values from a list.
    comparitor: Compares product availability and sends notifications if necessary.
    monitor: Initiates the monitoring process.

### Configuration

    Environment Variables: Configure your bot using the .env file for sensitive data such as Discord webhooks, proxies, and user-agent settings.
    Proxies: Use a list of proxies to avoid IP bans and enhance scraping efficiency.
    Keywords: Set keywords to filter specific products you are interested in.

### Example .env File

USERNAME=your_discord_username
AVATAR_URL=your_avatar_url
COLOUR=your_embed_colour
WEBHOOK=your_discord_webhook_url
LOC=location_code
LAN=language_code
PROXY=proxy1%proxy2%proxy3
KEYWORDS=sneaker%release
DELAY=5.0

### License
This project is licensed under the MIT License
