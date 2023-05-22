# LimeBot CLI

LimeBot CLI is a command-line interface chatbot powered by POE . It allows you to have interactive conversations with two different bots: Sage and ChatGPT.

check the web version here : https://github.com/TheLime1/gptCensorFree

## Features

- Choose between two bots: Sage or ChatGPT.
- Input messages for the chatbot via command-line arguments or interactively.
- Export the conversation to a .txt file for future reference.

## Prerequisites

- Python 3.7 or higher installed on your system.

## Getting Started

1. Clone or download the LimeBot CLI repository to your local machine.

2. Open a command-line interface (e.g., Command Prompt, Terminal) and navigate to the directory where you have saved the LimeBot CLI files.

3. Install the required dependencies by running the following command:
```
pip install -r requirements.txt
```

4. Run the LimeBot CLI app:
```
python limebot_cli.py
```

## Usage

The LimeBot CLI supports the following command-line arguments:

- `-b` or `--bot`: Choose the bot for the conversation. Valid options are `sage` and `chatgpt`.
Example: `python limebot_cli.py -b sage`

- `-m` or `--message`: Input a message for the chatbot.
Example: `python limebot_cli.py -b chatgpt -m "Hello, how are you?"`

- for more info you can use `-h` or `--help` to see the help message.

If you don't provide any command-line arguments, the app will prompt you to choose a bot and enter a message interactively.

Once the conversation starts, you can continue the interaction by typing your messages or selecting options from the menu. The menu options include changing the bot or exporting the conversation to a .txt file.

To change the bot during the conversation, select option `1` from the menu and choose the desired bot.

To insert the clipboard contents as a message, select option `2` from the menu. The current contents of the clipboard will be used as the input message for the chatbot.

To export the conversation to a .txt file, select option `3` from the menu. Enter the desired filename when prompted, and the conversation will be saved in the `conv` directory as a .txt file.

To exit the LimeBot CLI app, select option `0` from the menu.

## Notes

- If the app cannot find the `token.txt` file or the file is empty, it will automatically generate a new token using the `token_gen.py` script provided.

- The conversation history is stored within the app and is not persistent between sessions.

Feel free to customize and enhance the LimeBot CLI app according to your needs. Happy ~~chatting~~ cheating!