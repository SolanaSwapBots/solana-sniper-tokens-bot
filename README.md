**Solana Tokens Bot Pump.fun/Raydium** This advanced bot for the Solana network is designed to listen for and detect new liquidity pools on both Pump.Fun and Raydium, ensuring you’re among the first to take action. It automatically purchases tokens using a fixed amount in WSOL, often executing transactions before the tokens are publicly available for exchange on the user interface.

The bot's success relies on RPC node speed, enabling high-priority and efficient operations in a competitive environment. After two months of intensive development and optimization, this program is now ready to assist Solana enthusiasts and traders in seizing the best token acquisition opportunities.

Even for testing purposes, it is essential to keep additional SOL available to cover transaction fees, in addition to using WSOL as the trading token. A recommended configuration is:

"1 SOL / 0.1 WSOL / QUOTE_AMOUNT=0.01"

This setup can be adjusted according to your needs and circumstances. Make sure to always have enough SOL in your wallet to ensure smooth execution of operations.

- `New Tokens Snipe`
- `Burn/Lock Check`
- `Renounce Check`
- `Min Pool Liq`
- `Take Profit`
- `Stop Loss`
- `Auto-Sell`
- `Fast Buy`

## Setup
Steps to Run the Script:

1. Download and Extract the Repository Files:
        Use the command: git clone https://github.com/SolanaSwapBots/solana-sniper-tokens-bot
        Or click the green "Code" button on the repository page and select "Download ZIP".

2. Install Node.js:
    Ensure the Node.js runtime environment is installed on your computer. You can download it from: Node.js Official Site.

3. Set Up the Runtime Environment:
    Use a terminal or an IDE like VSCode to run the script. Detailed instructions are provided below; follow them carefully.

4. Prepare Your Wallet:
    Convert some SOL into WSOL for trading.
        Important: Even if you plan to test the bot for only an hour, ensure you have enough SOL in your wallet to cover transaction fees, as gas fees are paid in SOL.
        Example configuration: (10 SOL) : (1 WSOL) : (QUOTE_AMOUNT=0.1).

By following these steps, you'll be ready to deploy the bot effectively!

## How to Convert SOL to WSOL on Raydium
Step 1: Access Raydium

1. Open the official Raydium website: Raydium.io.
2. Connect your Solana wallet (such as Phantom, Solflare, or another supported wallet).

Step 2: Convert SOL to USDC

1. Navigate to the Swap tab in the main menu.
2. In the first dropdown menu, select SOL as the source token.
3. In the second dropdown menu, select USDC as the target token.
4. Enter the amount of SOL you want to convert.
5. Confirm the transaction and pay the network fees in SOL.

Step 3: Convert USDC to WSOL

1. Once the first step is completed, stay on the Swap tab.
2. Select USDC as the source token in the first dropdown menu.
3. In the second dropdown menu, select WSOL as the target token.
4. Enter the amount of USDC you want to convert.
5. Confirm the transaction and pay the network fees in SOL.

## Configuration Guide
Follow these steps to configure the script correctly:

1. Update the .env File:
    Customize the configuration settings by editing the .env file with the details below.

2. Required Parameters:
        PRIVATE_KEY: Your wallet's private key. Ensure it is stored securely.
        RPC_ENDPOINT: The HTTPS RPC endpoint for connecting to the Solana network.
        RPC_WEBSOCKET_ENDPOINT: The WebSocket RPC endpoint for real-time event monitoring.
        QUOTE_MINT: The token used for purchases. Default is WSOL.
        QUOTE_AMOUNT: The amount of WSOL used to buy each new token.
        COMMITMENT_LEVEL: Leave as default unless specific adjustments are needed.

3. Liquidity and Security Checks:
        CHECK_IF_IS_BURNED: Enable to verify if liquidity is burned.
        CHECK_IF_IS_LOCKED: Enable to verify if liquidity is locked.

4. Snipe List Settings:
        USE_SNIPE_LIST: Enable to purchase only tokens listed in snipe-list.txt.
        SNIPE_LIST_REFRESH_INTERVAL: Set the refresh interval for the snipe list in milliseconds.

5. Additional Checks:
        CHECK_IF_MINT_IS_RENOUNCED: The script will purchase tokens only if the mint authority is renounced.
        MIN_POOL_SIZE: Specify the minimum pool size required for a token to be considered.

6. Profit and Risk Management:
        TAKE_PROFIT: Set the take-profit percentage (default is 70%).
        STOP_LOSS: Set the stop-loss percentage (default is 20%).

7. BirdEye API:
        BIRDEYE_API_KEY: Used for features like take-profit/stop-loss and liquidity checks. You can use the default key provided in the .env file, or generate your own via BirdEye API Key Documentation.
  
## Installation
1. Install Dependencies:
    Run the following command in your terminal to install all required dependencies:
    `npm install`

2. Start the Script:
    Launch the script by executing:
    `npm run index`

## Donate

This program has undergone extensive testing and audits, showcasing its strong profitability.

Support the project: 
Solana Wallet Address: `J1Q418tYAPR2ymCEWraWTmvVuVYtwHxFidzvfWpu11WB` 

## Disclaimer

> [!IMPORTANT]
> Use this script at your own risk. Ensure you understand the functionality and associated risks before proceeding.
