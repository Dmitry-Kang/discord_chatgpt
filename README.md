# Discord Chat Bot with ChatGPT

Welcome to the Discord Chat Bot powered by ChatGPT. This bot generates responses using the OpenAI ChatGPT model and provides various commands for customization. The bot is containerized using Docker Compose for easy deployment.

## Usage

1. Make sure you have Docker Compose installed on your system.

2. Clone the repository to your local machine:

```bash
git clone https://github.com/Dmitry-Kang/discord_chatgpt.git
cd discord_chatgpt
```

3. Before running the bot, make sure to edit the `config.json` file with your Discord and OpenAI credentials.

```json
{
    "discord_bot_token": "your_discord_bot_token",
    "discord_channel_id": "your_discord_channel_id",
    "openAI_key": "your_openai_api_key"
}
```

4. Build and run the Docker containers:

```bash
docker-compose up --build
```

## Bot Commands

- `/help`: Display a list of available commands.
- `/reset`: Clear the conversation history.
- `/chat your_message`: Send a message to the bot and receive a response.
- `/private`: Set the bot to respond privately to the user.
- `/public`: Set the bot to respond publicly for all users.

## Examples

- To send a message to the bot: `/chat Hello, bot!`
- To reset the conversation history: `/reset`
- To switch to private responses: `/private`
- To switch to public responses: `/public`

## Note

Make sure to handle your OpenAI API key securely and avoid sharing it publicly. Additionally, follow Discord's guidelines for bot permissions and privacy.

Feel free to customize and extend the bot to fit your specific needs. Happy chatting!
