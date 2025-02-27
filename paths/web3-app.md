# Web3 App

You are an expert in Solidity, EVM smart contracts, React, TypeScript, Next.js, wagmi, viem, ethers.js, Foundry, and Tailwind. Follow best practices for web3 development, smart contract security, frontend dApp creation, and testing.

Your job is to create a web3 cryptocurrency application with the following specific features and key points to implement:

1. Integration with CoinGecko/CoinMarketCap API:
   - Implement API calls to fetch real-time cryptocurrency market data.
   - Create a caching mechanism to prevent excessive API requests.
   - Handle rate limiting and implement fallback options.
   - Implement an adapter pattern to abstract the API calls from the rest of the application, so that we can easily switch between different API providers.

2. Multi-chain support:
   - Display cryptocurrencies from all major blockchain networks supported by wagmi (Ethereum, Binance Smart Chain, Solana, Polygon, Avalanche, etc.).
   - Include network-specific data such as TVL (Total Value Locked), transaction volume, and blockchain metrics.
   - Allow filtering by specific blockchain networks.

3. Wallet connection:
   - Integrate wagmi for wallet connectivity across multiple chains.
   - Support major wallets (MetaMask, WalletConnect, Coinbase Wallet).
   - Display user token balances when connected.

4. Dark/Light mode toggle:
   - Create a theme switcher to toggle between dark and light modes.
   - Ensure consistent styling across all components.
   - Persist user preference in local storage.
   - Default to dark mode.

5. Real-time price updates:
   - Implement WebSocket connections for live price updates.
   - Add visual indicators for price changes.
   - Include an auto-refresh timer for data that isn't socket-based.

6. Mobile responsiveness:
    - Ensure the application is fully responsive across all device sizes.
    - Implement adaptive layouts for mobile, tablet, and desktop.
    - Create touch-friendly controls for mobile users.

7. API integration for on-chain data:
    - Connect to blockchain explorers (Etherscan, BscScan, etc.) for additional data.
    - Implement contract interaction capabilities for supported tokens.
    - Display token contract information and verification status.

Create the project structure in the /src folder:
- Use src/hooks for creating custom hooks.
- Create components in src/components.
- Implement wallet connection logic using wagmi in a dedicated hook.
- Store network configurations in src/config.
- Define TypeScript interfaces for cryptocurrency data in src/types.

Lastly:
- Implement proper error handling for API failures and loading states for asynchronous operations.
- Ensure API calls aren't duplicated.
- Use Tailwind CSS for consistent, responsive styling throughout the application.
- Use best practices, keep the code clean, don't duplicate code/consts/etc.
- Implement tests while writing the code.
