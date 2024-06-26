# Python ChatBot Project

This project is a Python-based chatbot that utilizes various libraries to provide functionalities like responding to user queries, checking server status, and more. It's structured to be modular, with separate components for different tasks.

## TODO

- Adding a system so that people don't spam queries (and getting that so that the system can adjust to meet spending limits). Something related to economy, but I'm not sure.

- Building an informed query section, that can search up good context.

- Creating a proompter section, which asks a question based on some news -> probably add some schedulability.

- Reaction role section -> don't know how that'll be done, but it'll be helpful.

## Features

- **[ChatBot Prompts](cogs/ChatBotPrompts.py)**: Handles dynamic conversation flows.
- **[Ping](cogs/Ping.py)**: Checks and reports server status.
- **[Status](cogs/Status.py)**: Provides the current status of the chatbot.

## Dependencies

The project relies on several third-party libraries, including:

- `urllib3` for HTTP requests.
- `websockets` for WebSocket communication.
- `aiohttp` for asynchronous HTTP requests.
- `distro` for Linux distribution information.
- `sniffio` for detecting the async library in use.
- `discord.py` for directly interfacing with Discord.
- `openai` for accessing OpenAI's APIs.

For a full list of dependencies, refer to the [requirements.txt](requirements.txt) file.

## Installation

1. Clone the [repository](https://github.com/Elias2660/Proompter):

   ```shell
   git clone git@github.com:Elias2660/Proompter.git
   ```

2. Create a virtual environment:

   ```shell
   python -m venv venv
   ```

3. Activate the virtual environment:

   - On Windows:

     ```powershell
     .\venv\Scripts\activate
     ```

   - On Unix or MacOS:

     ```sh
     source venv/bin/activate
     ```

4. Install the [dependencies](requirements.txt):

   ```sh
   pip install -r requirements.txt
   ```

5. Add an env file with the following information with the following structure. Read about creating your own [Discord](https://discord.com/) bot and application [here](https://www.geeksforgeeks.org/discord-bot-in-python/) and [here](https://realpython.com/how-to-make-a-discord-bot-python/), and learn about using gpt and creating your own API key [here](https://platform.openai.com/docs/overview).

   ```env
   export BOT_TOKEN="<Insert the token for your bot here>"
   export GPT_API_KEY="<>"
   ```

## Usage

Run the [main script](main.py) to start the chatbot:

```sh
python main.py
```

## Contributing

[Contributions](CONTRIBUTING.md) are welcome! Please feel free to submit pull requests or open issues to discuss potential improvements or features.

## Code of Conduct

Please don't be a bad person! Check out the [code of conduct](CODE_OF_CONDUCT.md) for more details.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
