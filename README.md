# Track My Money API

Application to control all my expenses

## Features

- Wallets 💰
    - Add all your bank accounts and digital wallets in one place
    - View your total balance and control your resources easily
- Credit Cards 💳
    - Register all your credit cards
    - Monitor your bills and avoid surprises at the end of the month
- Income 💵
    - Record all your income sources in an organized way
- Expenses 📉
    - Log and categorize your expenses for better financial control
- Loans 🔄
    - Manage borrowed money and keep track of who owes you and who has already paid
- Subscriptions 📅
    - Keep track of all your service subscriptions and avoid unexpected charges

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user
- `POST /api/auth/refresh-token` - Refresh authentication token
- `POST /api/auth/logout` - Logout user

### Wallets
- `GET /api/wallets` - Get all wallets
- `POST /api/wallets` - Create new wallet
- `GET /api/wallets/{id}` - Get wallet details
- `PUT /api/wallets/{id}` - Update wallet
- `DELETE /api/wallets/{id}` - Delete wallet
- `GET /api/wallets/{id}/transactions` - Get wallet transactions
- `POST /api/wallets/{id}/transactions` - Add transaction to wallet
- `POST /api/wallets/transfer` - Transfer between wallets

### Credit Cards
- `GET /api/credit-cards` - Get all credit cards
- `POST /api/credit-cards` - Add new credit card
- `GET /api/credit-cards/{id}` - Get credit card details
- `PUT /api/credit-cards/{id}` - Update credit card
- `DELETE /api/credit-cards/{id}` - Delete credit card
- `GET /api/credit-cards/{id}/bills` - Get all bills for a card
- `GET /api/credit-cards/{id}/bills/current` - Get current bill
- `GET /api/credit-cards/{id}/transactions` - Get card transactions
- `POST /api/credit-cards/{id}/transactions` - Add transaction to card

### Transactions
- `GET /api/transactions` - Get all transactions
- `POST /api/transactions` - Create transaction
- `GET /api/transactions/{id}` - Get transaction details
- `PUT /api/transactions/{id}` - Update transaction
- `DELETE /api/transactions/{id}` - Delete transaction
- `GET /api/transactions/summary` - Get transactions summary
- `GET /api/transactions/categories` - Get transactions by category

### Categories
- `GET /api/categories` - Get all categories
- `POST /api/categories` - Create new category
- `GET /api/categories/{id}` - Get category details
- `PUT /api/categories/{id}` - Update category
- `DELETE /api/categories/{id}` - Delete category
