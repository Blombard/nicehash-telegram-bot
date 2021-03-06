# Starting out

1.  Step 1: Serverless framework

  ```bash
  npm install -g serverless
  ```

2.  Export credentials:

  ```bash
  export AWS_ACCESS_KEY_ID=<Access key ID>
  export AWS_SECRET_ACCESS_KEY=<Secret access key>
  export TELEGRAM_TOKEN=<Your Telegram Token>
  ```

3.  Install pip requirements:

  ```bash
  pip install -r requirements.txt -t vendored
  ```

4.  Deploy to AWS:

  ```bash
  serverless deploy
  ```

5. Set up webhook:

  ```bash
  curl --request POST --url https://api.telegram.org/bot<Your Telegram TOKEN>/setWebhook --header 'content-type: application/json' --data '{"url": <API endpoint>}'
  ```

6. Ask something to the bot:
  * /help to get help
  * /balance to get the total balance
  * /detailed_balance to get the distribution between wallets
  * /payments to get the latests payments
  * /euro to get the balance in EURO

Inspired by this repo : https://github.com/Andrii-D/serverless-telegram-bot
