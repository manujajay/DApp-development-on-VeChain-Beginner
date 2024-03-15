
# VeChain Smart Contract Deployment Guide

This guide provides comprehensive instructions for deploying a smart contract on VeChain using a project built with Vite and npm. The repository includes a smart contract called `Storage.sol` compiled on Remix, along with a custom frontend.

## Repository Structure

- `public/`: Contains static assets for the frontend.
- `LICENSE`: The license file for the project.
- `README.md`: The file you are currently reading, which provides instructions and documentation for the project.
- `index.html`: The entry point for the frontend of the DApp. It contains the HTML structure of the web application.
- `javascript.svg`: An SVG file, likely used as an icon or graphic in the frontend.
- `main.js`: The main JavaScript file that contains the logic for interacting with the smart contract.
- `package-lock.json`: Automatically generated file for any operations where npm modifies either the `node_modules` tree or `package.json`.
- `package.json`: Lists the packages that the project depends on and provides information to npm that allows it to identify the project and handle its dependencies.
- `storage.sol`: The Solidity smart contract that includes a simple storage mechanism and is deployed on the VeChain blockchain.
- `style.css`: The Cascading Style Sheets (CSS) file that contains the styles for the frontend of the DApp.

## Prerequisites

- Node.js and npm installed.
- Vite.js for frontend build and development.
- A VeChain wallet and access to VeChain nodes.

## Setting up the Project

1. Clone the repository to your local machine.
2. Navigate to the root directory of the project via the terminal.
3. Run `npm install` to install all dependencies listed in `package.json`.

## Smart Contract: `storage.sol`

The `Storage.sol` contract has the following functions:

- `store(int _a)`: Stores a number in the contract's state.
- `read()`: Returns the number stored in the contract.

## Frontend: `index.html`, `main.js`, and `style.css`

The frontend is a simple decentralized application (DApp) that interacts with the smart contract. It allows users to store and read a number from the blockchain.

- `index.html`: Contains the markup for the DApp, including buttons for login, storing, and reading data.
- `main.js`: Includes the Connex framework setup and the logic for user login, and functions to call the `store` and `read` methods of the contract.
- `style.css`: Provides the styling for the DApp.

## Usage

### Running the Development Server

- Run `npm run dev` to start the Vite development server.
- Open the displayed local server URL in your web browser to interact with the DApp.

### Building for Production

- Run `npm run build` to build the static files for production.
- The built files can be served using `npm run preview`.

## Interacting with the Smart Contract

Users can interact with the smart contract through the frontend. Here's how:

- **Login**: Users must first log in using their VeChain wallet.
- **Store a Number**: Users can store a number in the smart contract by entering it and clicking the 'store' button.
- **Read the Number**: Users can read the stored number from the smart contract by clicking the 'read' button.

The `main.js` script manages these interactions using Connex, the standard interface to connect VeChain apps with the blockchain and user wallets.

## Contact

For any further questions regarding this guide or the project, you can reach out.

---

Happy Coding!
