# How to Configure Environment Variables for Paystack

Use this guide to keep your Paystack API/Secret Keys  safely in a node.js app, so it will not appear in your code

## Before you begin

- A Paystack account 
- Your test secret key (Settings > API keys & Webhooks
- Node.js and npm installed 
- An existing Node.js project
  ## Steps

### 1. Install the dotenv package

In your project folder, Install the package that reads ` .env` files:

  ```bash
  npm install dotenv
  ```
### 2. Create the .env file

In the root of your project (the same folder as `package.json`), create a file named `.env` and add your key. Don't put spaces `=` or quotes around the key.

```
PAYSTACK_SECRET_KEY=your_test_secret_key_here
```
 
### 3. Keep the .env file off GitHub

Open (or create) `.gitignore` in your project root and add this line so Git never uploads your key:

```
.env
```

### 4. Load the key in your code

At the top of your main file (for example `index.js`), load `dotenv` first, then read the variable:

```javascript
require('dotenv').config();

const secretKey = process.env.PAYSTACK_SECRET_KEY;
```

### 5. Check that the key loaded

Add this line below the code from step 4 and run `node index.js`:

```javascript
console.log(secretKey ? 'Key loaded' : 'Key missing');
```

You should see `Key loaded`. Never print the key itself.
