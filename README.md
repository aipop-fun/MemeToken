# MemeToken Generator 🎨

![MemeToken, by codingsh](/public/src/public/screenshot.png)

An AI-powered platform for generating and deploying meme tokens on Base and baseSepolia networks. Create unique tokens with AI-generated names, symbols, and images through an intuitive interface.

## 🌟 Features

- AI-powered token name and symbol generation
- AI-generated token images
- Automatic smart contract deployment
- Multi-chain support (Base and baseSepolia)
- MetaMask integration
- Farcaster Frame SDK integration
- Automated liquidity pool creation

## 🛠 Technology Stack

### Frontend
- React.js with TypeScript
- TailwindCSS for styling
- wagmi for Ethereum interactions
- Farcaster Frame SDK for social integration
- shadcn/ui components

### Smart Contracts
- Solidity ^0.8.13
- OpenAI Oracle for AI integration
- OpenZeppelin contracts
- Custom Token Factory

## 🚀 Getting Started

### Prerequisites
- Node.js
- npm or yarn
- MetaMask wallet
- Some ETH on Base or Optimism network

### Installation

1. Clone the repository:
```bash
git clone https://github.com/aipop-fun/MemeToken
cd MemeToken
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Set up environment variables:
```env
NEXT_PUBLIC_WALLET_CONNECT_ID=your_wallet_connect_id
NEXT_PUBLIC_CONTRACT_ADDRESS=your_contract_address
```

4. Run the development server:
```bash
npm run dev
# or
yarn dev
```

## 💡 How It Works

1. **Connect Wallet**: Connect your MetaMask wallet to either Base or Optimism network
2. **Generate Token**: Enter a description for your meme token
3. **AI Processing**: 
   - Generates token name and symbol using LLaMA model
   - Creates token image using Stable Diffusion
4. **Smart Contract**: Automatically deploys your token with:
   - Fixed supply of 1 million tokens
   - Automatic liquidity pool creation
   - Custom token metadata

## 🔧 Smart Contract Details

### Main Components:

#### AIMemeTokenGenerator Contract
- Handles token generation requests
- Interacts with AI Oracle
- Manages token deployment
- Creates initial liquidity

Key functions:
```solidity
function createMemeToken(
    string calldata namePrompt,
    string calldata imagePrompt
) external payable nonReentrant
```

### Fees Structure:
- Name generation fee (AI Oracle)
- Image generation fee (AI Oracle)
- Deployment fee (0.0008 ETH)

## 🔐 Security

- NonReentrant protection
- Owner-only admin functions
- Gas limit controls
- Secure callback handling

## 📱 UI Components

### Key Features:
- Responsive design
- Dark/light mode support
- Interactive token preview
- Real-time network switching
- MetaMask integration

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📄 License

MIT License - see LICENSE.md

## 🙏 Acknowledgments
- Ora.io
- OpenAI for AI models
- Farcaster team for Frame SDK
- shadcn for UI components
- Base 
- Clanker Codebase 

## 📞 Support

For support, please open an issue in the repository or reach out to our community on Discord.

---

Built with ❤️ by [Codingsh](https://warpcast.com/codingsh) ❤️❤️❤️ [aipop](https://aipop.fun)