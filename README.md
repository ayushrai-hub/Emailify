# Email Cleaner Script

This Python script helps you clean your email inbox by automatically identifying and moving potential spam and promotional emails to the Trash folder. It uses IMAP to connect to your email account and processes emails based on a comprehensive list of spam keywords.

## Features

- Connects to any email account that supports IMAP
- Processes a user-defined number of emails (default: 800)
- Identifies potential spam and promotional emails based on subject, sender, and content
- Moves identified emails to the Trash folder
- Provides progress updates during execution

## Prerequisites

- Python 3.6 or higher
- `imaplib` and `email` libraries (included in Python standard library)

## Setup

1. Clone this repository or download the `email_cleaner.py` script.
2. Ensure you have Python installed on your system.
3. If you're using Gmail:
   - Enable IMAP in your Gmail settings
   - Create an App Password for this script (required if you have 2-Step Verification enabled)

## Usage

1. Open a terminal or command prompt.
2. Navigate to the directory containing the script.
3. Run the script:
   ```
   python email_cleaner.py
   ```
4. Follow the prompts to enter your:
   - Email address
   - Password (use App Password for Gmail)
   - IMAP server address (e.g., imap.gmail.com for Gmail)
   - Number of emails to process (default is 800)

5. The script will start processing emails and provide updates every 10 emails.
6. Once completed, the script will display a summary of the emails processed and moved to Trash.

## Customization

You can modify the `spam_keywords` list in the `is_spam_or_promo` function to add or remove keywords based on your needs.

## Caution

- This script moves emails to the Trash folder, not permanent deletion. However, use it cautiously.
- Always check your Trash folder for any important emails that might have been moved accidentally.
- It's recommended to run the script on a small batch of emails first to ensure it's working as expected.

## Contributing

Feel free to fork this repository and submit pull requests with any enhancements.

## License

This project is open source and available under the [MIT License](LICENSE).
