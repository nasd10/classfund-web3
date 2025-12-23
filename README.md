# 🪙 Classfund v1.0
**A Decentralized Class Treasury Management System**

Classfund is a Web3 application designed to bring transparency, accountability, and automation to class treasury management. Built on the Ethereum blockchain (deployed on Sepolia Testnet), it eliminates the need for manual bookkeeping and ensures that every contribution is recorded immutably.

---

## 🌟 Features

- **Decentralized Payments**: Members can pay their dues directly via MetaMask using ETH.
- **Role-Based Access**: 
  - **Treasurer**: Can add/remove members, withdraw funds for class needs, and trigger new payment periods.
  - **Members**: Can view total balance, track their personal contributions, and see the active period.
- **Transparency Dashboard**: A real-time transaction history that "listens" to blockchain events to show who has paid and when.
- **Period Management**: Tracks contributions across different timeframes (e.g., weekly or monthly).

---

## 🛠 Tech Stack

- **Smart Contract**: Solidity (0.8.0)
- **Frontend**: Next.js 14+ (App Router)
- **Blockchain Library**: Ethers.js v6
- **Styling**: Tailwind CSS
- **Wallet Integration**: MetaMask (EIP-1193)

---

## 🚀 Smart Contract Overview

The contract consists of several key functions:
- `pay()`: Allows whitelisted members to contribute funds.
- `withdraw(uint amount)`: Restricted to the Treasurer for fund allocation.
- `addMembers(address[])`: Enables the Treasurer to whitelist new classmates.
- `nextPeriod()`: Increments the treasury cycle for organized reporting.

---

## 📦 Getting Started

### 1. Prerequisites
- [Node.js](https://nodejs.org/) installed.
- [MetaMask](https://metamask.io/) extension installed in your browser.
- Some **Sepolia Testnet ETH** (you can get this from a faucet).

### 2. Installation
Clone the repository and install dependencies:
```bash
git clone [https://github.com/your-username/classfund.git](https://github.com/nasd10/classfund.git)
cd classfund
npm install
```

### 3. Configuration
The smart contract is already deployed on the Sepolia testnet at address `0x43c9c8ced4655a2b7ee26d680935cb0d82bdf071`. The contract address is hardcoded in the application for simplicity.

### 4. Running the Application

Start the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### 5. Usage

1. **Connect Wallet**: Click the "Connect Wallet" button and approve the connection in MetaMask. Ensure you are on the Sepolia testnet.

2. **View Dashboard**: Once connected, you can see the treasury balance, current period, and your total contributions.

3. **Make a Payment**: Enter the amount in ETH and click "Pay Dues" to contribute to the treasury.

4. **Treasurer Functions** (if you are the treasurer):
   - Add new members by entering their addresses and clicking "Add Members".
   - Withdraw funds by entering the amount and clicking "Withdraw".
   - Advance to the next period by clicking "Next Period".

5. **View Transactions**: The transaction history updates in real-time as blockchain events are emitted.

---

## 📋 Smart Contract Details

- **Network**: Sepolia Testnet
- **Contract Address**: `0x43c9c8ced4655a2b7ee26d680935cb0d82bdf071`
- **Source Code**: Available in the class-fund repo `contracts/` directory (if applicable)

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📞 Contact

For questions or support, please open an issue on GitHub or contact the maintainers.

---

*Built for transparent class treasury management.*