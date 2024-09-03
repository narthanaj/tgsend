# Telegram Message Send Action

This GitHub Action sends a message to a Telegram chat using a Telegram bot. It supports optional Markdown formatting for the message.

## Features

- Send messages to Telegram chats
- Optional Markdown support
- Easy to integrate into any workflow

## Inputs

### `bot_token`

**Required** The token for your Telegram bot.

### `chat_id`

**Required** The ID of the chat where you want to send the message.

### `message`

**Required** The message you want to send.

### `markdown`

**Optional** Enable Markdown parsing for the message. Default is 'false'.

## Usage

### Basic Usage

```yaml
- name: Send Telegram Notification
  uses: DiyRex/tgsend@v1.1
  with:
    bot_token: ${{ secrets.TELEGRAM_BOT_TOKEN }}
    chat_id: ${{ secrets.TELEGRAM_CHAT_ID }}
    message: 'Hello from GitHub Actions!'
    markdown: boolean