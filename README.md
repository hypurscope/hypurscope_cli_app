# HypurScope

A simple python command-line interface (CLI) for querying Hyperliquid API endpoints. It provides access to user wallet data, token holders, Defi information, and spot USDC stats.

---

## Features
- Fetch user wallet data by ID and timeframe
- Get holders of a specific token
- View Defi information from hyperliquid
- check spot USDC info

---

## Installation


### 1. Clone the repo
```bash
git clone https://github.com/hypurscope/hypurscope_cli_app.git
cd hypurscope_cli_app
```

### 2. Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

### 3. Install dependencies
```bash
pip install -r requirements
```

### 4. Make the script executable
```bash
chmod +x hypur_scope.py
```

## Usage

### Get general help:
```bash
./hypur_scope.py --help
```

## Subcommands & Examples

### 1. Get user wallet data
- Fetch wallet data with a start time and optional end time.
```bash
./hypur_scope.py get_userdata <wallet_id> <start_time> [--end_time <end_time>]
```
- example
```bash
./hypur_scope.py get_userdata 0xfefefefefefefefefefefefefefefefefefefefe "2025-01-01 00:00" --end_time "2025-02-01 00:00"
```

### 2. Get token holders
- return holders of a token
```bash
./hypur_scope.py get_tokenholders <token_name>
```
- example
```bash
./hypur_scope.py get_tokenholders HYPE
```

### 3. Get Defi info
- retrieve Hyperliquid Defi information
```bash
./hypur_scope.py defi
```

### 4. Get spot USDC info
- retrieve hyperliquid spot USDC information
```bash
./hypur_scope.py spot
```
