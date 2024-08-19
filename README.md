# **Stellar Token Transfer MVP**

## **Overview**

This project is a simple Minimum Viable Product (MVP) that demonstrates the creation, issuance, and transfer of a custom token on the Stellar blockchain using a React front end. The application leverages Stellar’s fast and low-cost transactions, along with a Soroban smart contract to facilitate secure token transfers between accounts.

## **Features**

- **Token Issuance**: Create and issue a custom token (`MVPToken`) on the Stellar testnet.
- **Token Transfer**: Transfer tokens between accounts using a simple React interface.
- **Soroban Smart Contract**: A Soroban smart contract handles token transfers securely on the blockchain.
- **User-Friendly Interface**: A basic but functional React front end for interacting with the Stellar blockchain.

## **Technologies Used**

- **Stellar SDK**: For interacting with the Stellar blockchain.
- **Soroban**: For writing and deploying smart contracts on Stellar.
- **React**: For building the front end of the application.
- **JavaScript**: The primary programming language used.
- **HTML/CSS**: For structuring and styling the web interface.

## **Installation and Setup**

### **Prerequisites**

- **Node.js**: Make sure you have Node.js installed on your machine.
- **npm**: The Node package manager should be available (comes with Node.js).
- **Rust**: Required for Soroban smart contract development.

### **Clone the Repository**

```bash
git clone https://github.com/mederhoo-scrip/stellar-token-transfer.git
cd stellar-token-transfer-mvp
```

### **Install Dependencies**

```bash
npm install
```

### **Set Up Stellar Accounts**

1. Visit [Stellar Laboratory](https://laboratory.stellar.org/#account-creator?network=test) to create test accounts on the Stellar testnet.
2. Fund your issuing and distribution accounts using the Stellar testnet faucet.
3. Update the Stellar account details in the project’s environment variables or in the relevant configuration files.

### **Issue the Custom Token**

- Use the Stellar SDK to issue your custom token (`MVPToken`). You can run the script provided in the `src/services/stellarService.js` to handle the token issuance process.

### **Deploy the Soroban Smart Contract**

1. Write the Soroban smart contract in Rust.
2. Compile and deploy the contract to the Stellar testnet.
3. Note down the contract ID for use in the React application.

### **Running the Application**

To start the React application locally, run:

```bash
npm start
```

The app will be available at `http://localhost:3000`.

### **Test the Application**

1. Open the application in your browser.
2. Enter the recipient’s Stellar address and the amount of tokens to transfer.
3. Submit the form to initiate the token transfer.
4. Check the transaction result displayed on the interface.

## **Project Structure**

```plaintext
stellar-token-transfer-mvp/
│
├── public/
│   └── index.html            # The main HTML file
├── src/
│   ├── components/           # React components
│   ├── services/             # Stellar-related functions (e.g., token issuance, transfers)
│   ├── App.js                # Main React component
│   └── index.js              # Entry point for the React app
├── .gitignore                # Files and directories to ignore in Git
├── package.json              # Project dependencies and scripts
└── README.md                 # Project documentation
```

## **Deployment**

To deploy the application, follow these steps:

1. **Build the app**:
   ```bash
   npm run build
   ```
2. **Deploy**: Use a service like GitHub Pages, Vercel, or Netlify to host the built files.

## **Usage Instructions**

1. **Token Issuance**: Issue the `MVPToken` using the provided script in the `src/services/stellarService.js`.
2. **Token Transfer**: Use the web interface to transfer tokens by entering the recipient’s address and amount, then submitting the form.
3. **Transaction Verification**: Monitor the transaction status directly on the web interface.

## **Contributing**

Contributions are welcome! If you’d like to improve the project or add new features, feel free to fork the repository and submit a pull request.

## **License**

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## **Acknowledgments**

- [Stellar Development Foundation](https://www.stellar.org/) for providing the blockchain infrastructure.
- [Soroban](https://soroban.stellar.org/) for the smart contract platform.
- [Create React App](https://reactjs.org/docs/create-a-new-react-app.html) for the React project setup.
