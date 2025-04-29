# Arbitrum Stylus Cache Manager GUI

## Project Overview

The Arbitrum Stylus Cache Manager GUI is a web application designed to interact with the Arbitrum Stylus Cache Manager smart contract. This tool provides a user-friendly interface for managing cache entries, placing bids, and monitoring the cache status on the Arbitrum One network.

Key features include:
- View active cache entries
- Place bids for cache space
- Monitor cache size and decay rate
- Interact with the Arbitrum Stylus Cache Manager contract

## Getting Started

### Prerequisites
- Node.js (v18+)
- npm or yarn
- Web3-compatible wallet (MetaMask recommended)

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/arb-stylus-cache-manager-gui.git
cd arb-stylus-cache-manager-gui
```

2. Install dependencies
```bash
npm install
# or
yarn install
```

3. Create a `.env` file in the project root and configure:
```
VITE_WALLET_CONNECT_PROJECT_ID=your_wallet_connect_project_id
VITE_ARBITRUM_RPC_URL=https://arb1.arbitrum.io/rpc
```

4. Start the development server
```bash
npm run dev
# or
yarn dev
```

## Deployment

### Production Build
```bash
npm run build
# or
yarn build
```

### Deployment Options
- **Vercel**: Connect your GitHub repository and deploy automatically
- **Netlify**: Use the `build` command and publish the `dist` directory
- **Docker**: A `Dockerfile` can be created for containerized deployment

## Project Structure
```
├── src/
│   ├── components/        # React components
│   ├── hooks/             # Custom React hooks
│   ├── utils/             # Utility functions
│   └── App.tsx            # Main application component
├── public/                # Static assets
└── cacheManagerComponent.tsx  # Core cache manager logic
```

## Technologies Used
- React
- TypeScript
- Vite
- Tailwind CSS
- wagmi (Web3 hooks)
- Arbitrum Stylus SDK

## Feature Highlights
- Real-time cache entry tracking
- Bid placement for cache space
- Contract interaction hooks
- Responsive design
- Network status monitoring

## Configuration

### Environment Variables
- `VITE_WALLET_CONNECT_PROJECT_ID`: WalletConnect project ID
- `VITE_ARBITRUM_RPC_URL`: Arbitrum network RPC endpoint

### Supported Networks
- Arbitrum One (Chain ID: 42161)

## Security and Permissions

The application interacts with the CacheManager contract at address: 
`0x51dEDBD2f190E0696AFbEE5E60bFdE96d86464ec`

Always verify contract addresses and transactions before confirming.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Resources
- [Arbitrum Stylus Documentation](https://docs.arbitrum.io/stylus/)
- [Cache Manager Concept](https://docs.arbitrum.io/stylus/concepts/stylus-cache-manager)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.