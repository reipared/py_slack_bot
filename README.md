# Slack Bot README

This is a simple Slack bot implementation that connects to the Slack API using the SlackClient library and responds to commands.

## Prerequisites

- Python 3.x
- Slack API credentials (Slack Bot Token)

## Installation

1. Clone the repository or download the source code files.
2. Install the required dependencies by running the following command:
   ```
   pip install slackclient
   ```
3. Set up your Slack Bot Token as an environment variable named `SLACK_BOT_TOKEN`.
4. Run the script using the following command:
   ```
   python slack_bot.py
   ```

## Usage

Once the bot is running, it will listen for commands in the Slack workspace it's connected to.

To invoke the bot, mention the bot's username followed by a command. For example:

The available commands and their responses can be customized in the code.

## Customization

You can modify the bot's behavior by editing the code in the `slack_bot.py` file.

### Adding Commands

To add a new command, follow these steps:

1. Define a new string constant for the command, e.g., `NEW_COMMAND = "new"`.
2. In the `handle_command` function, add an `if` condition to check for the new command:
   ```python
   if command.startswith(NEW_COMMAND):
       response = "This is the response to the new command!"
   ```
3. Customize the response text as needed.

### Modifying Default Response

The default response is sent when the bot receives an unrecognized command. You can modify the default response message by changing the value of the `default_response` variable in the `handle_command` function.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- [SlackClient library](https://github.com/slackapi/python-slackclient) for interacting with the Slack API.
