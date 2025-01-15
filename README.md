# Solana Trade Bot

An advanced, automated trading bot designed for Solana tokens, leveraging the Solana Tracker API.

This bot supports various platforms, including Raydium (V4/CPMM), Pumpfun, Moonshot, Orca, and Jupiter, offering versatile trading opportunities.

It comes with two examples: one demonstrating HTTP request usage and another showcasing the speed and efficiency of Solana Tracker's Data Streams via Websockets.

![Screenshot of the Trading Bot](https://i.gyazo.com/afb12f6c358385f133fa4b95dba3c095.png)

## Features

- Enables automated trading of Solana tokens.
- Supports multiple tokens seamlessly.
- Offers customizable trading parameters, including liquidity, market cap, and risk score.
- Provides real-time monitoring and management of trading positions.
- Executes buy and sell operations concurrently for enhanced efficiency.
- Features detailed, timestamped logs with color-coded action highlights.
- Ensures persistent storage for tracking positions and transaction history.

## Prerequisites

- Node.js (v14 or later recommended)
- npm (comes with Node.js)
- A Solana wallet with SOL
- API Key (Billing Token) from [Solana Tracker Data API](https://docs.solanatracker.io)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/axioris/SolanaTradingBot.git
cd SolanaTradingBot
```

2. Install dependencies:

```bash
npm install
```

3. Rename the .env.example and configure the bot.

## Usage

Run the bot with:

```bash
node index.js 
```

Or

```bash
node websocket.js
```

## Configuration

To tailor the bot's functionality, update the .env file with the following settings:

- AMOUNT: Specify the SOL amount to swap per transaction.
- DELAY: Define the delay between buying cycles (in milliseconds).
- MONITOR_INTERVAL: Set the frequency for position monitoring (in milliseconds).
- SLIPPAGE: Determine the maximum acceptable slippage percentage.
- PRIORITY_FEE: Adjust the priority fee for transactions.
- JITO: Toggle "true" to enable Jito for transaction optimization.
- RPC_URL: Provide your Solana RPC endpoint URL.
- API_KEY: Input your Solana Tracker Data API Key.
- PRIVATE_KEY: Enter your wallet's private key securely.
- MIN_LIQUIDITY / MAX_LIQUIDITY: Define the liquidity range for token selection.
- MIN_MARKET_CAP / MAX_MARKET_CAP: Specify the market cap range for eligible tokens.
- MIN_RISK_SCORE / MAX_RISK_SCORE: Set the acceptable risk score range for tokens.
- REQUIRE_SOCIAL_DATA: Use "true" to limit trading to tokens with social data availability.
- MAX_NEGATIVE_PNL / MAX_POSITIVE_PNL: Establish PnL thresholds for triggering sales.
- MARKETS: List the targeted markets as a comma-separated value (e.g., Raydium, Orca, Jupiter).

## API Usage and Fees

This bot uses the Solana Tracker API. Please refer to [Solana Tracker's documentation](https://docs.solanatracker.io) for information about API usage and associated fees.

## Disclaimer

This bot is intended strictly for educational purposes. Use it at your own risk, and ensure you fully understand the code you are running as well as the financial implications of engaging in automated trading.

The primary objective of this project is to demonstrate the potential applications of the Solana Tracker API in creating automated trading solutions.

## License

[MIT License](LICENSE)

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/axioris/SolanaTradingBot/issues).

## Support

If you find this project helpful, please consider giving it a ⭐️ on GitHub!
If you have any further questions or need assistance, feel free to reach out to me anytime!
<p align="left">
  <a href="mailto:dane.foster.collins@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/dane-foster-11a177341/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://x.com/danefoster0"><img src="https://img.shields.io/badge/X-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="X" /></a>
  <a href="https://t.me/danefoster"><img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram" /></a>
  <a href="https://discord.com/users/354781324558467073"><img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
</p>
