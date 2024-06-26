

## Features

- Sends transactions from multiple wallets.
- Allows customization of the number of transactions and the time interval between them.
- Displays the transaction details and counts for each wallet.
- Uses a random amount and gas price for each transaction within specified ranges.

## Prerequisites

- [Go](https://golang.org/dl/) (version 1.21 or later)

## Install go:
```
sudo rm -rf /usr/local/go
curl -L https://go.dev/dl/go1.22.4.linux-amd64.tar.gz | sudo tar -xzf - -C /usr/local
echo 'export PATH=$PATH:/usr/local/go/bin:$HOME/go/bin' >> $HOME/.bash_profile
echo 'export PATH=$PATH:$(go env GOPATH)/bin' >> $HOME/.bash_profile
source .bash_profile
go version
```

## Getting Started

1. **Clone the repository:**
   ```sh
   git clone https://github.com/0xlimon/units-farm.git
   cd units-farm
   ```

2. **Set up Go modules:**
   ```sh
   go mod tidy
   ```

3. **Edit `privateKeys.json` file:**
   Add your private keys in the following format:
   ```json
   [
       "YOUR_PRIVATE_KEY_1",
       "YOUR_PRIVATE_KEY_2",
       "YOUR_PRIVATE_KEY_3",
       "YOUR_PRIVATE_KEY_4"
   ]
   ```

4. **Run the bot:**
   ```sh
   screen -S units
   go run main.go
   ```

5. **Follow the on-screen prompts:**
   - Enter the number of transactions per wallet.
   - Enter the time between transactions (in seconds).

Close screen with ctrl+A+D

## Common Issues

If you encounter errors similar to the ones below, don't worry, these are just network-related issues :))
```
Failed to get balance, retrying...
Failed to get nonce, retrying...
Failed to create transactor:
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Created by 0xLimon. Follow me on Twitter: [@zxLimon_](https://x.com/zxLimon_)
