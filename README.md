# csubscriptionbot

This repository contains a template for a Go-based Telegram bot designed to manage subscriptions.

## Introduction

The csubscriptionbot allows users to manage subscriptions for services via Telegram. It leverages the [gotgbot](https://github.com/PaulSonOfLars/gotgbot) library for interacting with the Telegram Bot API and Redis for managing subscription data.

## Installation

To set up the project, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/Teamhapp/csubscriptionbot-main.git
    cd csubscriptionbot-main
    ```

2. Install dependencies:
    ```sh
    go mod tidy
    ```

3. Set up environment variables:
    ```sh
    export TOKEN=<your-telegram-bot-token>
    export REDIS_URL=redis://<username>:<password>@<host>:<port>
    ```

4. Run the bot:
    ```sh
    go run main.go
    ```

## Usage

To use the bot, send the following commands via Telegram:

- `/start`: Start interaction with the bot.
- `/buy`: Buy a subscription for a service.
- `/status <chat_id>`: Check the status of your subscription.

## Features

- **Subscription Management**: Easily manage subscriptions for various services.
- **Manual Approval**: Admins can manually approve or reject subscription requests.
- **Automated Responses**: The bot provides automated responses for user commands.

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License

This project is licensed under the MIT License.
