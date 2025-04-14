# CryptoQuest: Blockchain Scavenger Hunt

A decentralized scavenger hunt platform built on the Stacks blockchain, where players solve progressive puzzles to earn crypto rewards.

## 📖 Overview

CryptoQuest is a blockchain-based scavenger hunt game where participants solve a series of puzzles to progress through stages and earn cryptocurrency rewards. The entire game mechanics are secured by smart contracts, ensuring transparency, fairness, and immutable record-keeping of achievements.

### Key Features

- **Progressive Puzzle System**: Multi-stage hunt with increasing difficulty and rewards
- **Time-Locked Challenges**: Stages unlock at predetermined times
- **Verifiable Solutions**: Solutions are verified on-chain using cryptographic hashes
- **Transparent Reward Distribution**: Automatic prize distribution upon correct solutions
- **Player Tracking**: Comprehensive tracking of player progress and achievements
- **Leaderboards**: Real-time rankings of fastest puzzle solvers

## 🔧 Technical Architecture

CryptoQuest is built using the following technologies:

- **Smart Contract**: Written in Clarity for the Stacks blockchain
- **Blockchain**: Deployed on Stacks, which provides Bitcoin's security with smart contract functionality
- **Frontend**: React-based web application for player interaction
- **Backend**: Node.js server for off-chain functionality and time synchronization

### Smart Contract Structure

The core game logic is implemented in a Clarity smart contract with the following components:

- **Hunt Management**: Functions to initialize, configure, and manage the scavenger hunt
- **Stage Management**: System to create and manage puzzle stages with clues and solutions
- **Player Registration**: Mechanism for players to register and pay entry fees
- **Solution Verification**: On-chain verification of submitted solutions
- **Prize Distribution**: Automatic distribution of rewards for correct solutions
- **Progress Tracking**: Comprehensive tracking of player achievements and stage completion

## 🚀 Getting Started

### Prerequisites

- Stacks wallet (Hiro Wallet recommended)
- STX tokens for transaction fees and entry fee
- Basic understanding of blockchain transactions

### Player Guide

1. **Register**: Connect your Stacks wallet and pay the entry fee to register
2. **Access Clues**: View the current available clue for your stage
3. **Solve Puzzles**: Work out the solution to the current puzzle
4. **Submit Solutions**: Submit your solution through the dApp interface
5. **Earn Rewards**: Receive STX tokens automatically upon correct solution
6. **Progress**: Advance to the next stage and repeat

### Hunt Creator Guide

1. **Deploy Contract**: Deploy the CryptoQuest contract to the Stacks blockchain
2. **Initialize Hunt**: Call the initialize-hunt function to activate the hunt
3. **Configure Stages**: Add stages with clues, solution hashes, unlock times, and prizes
4. **Fund Prizes**: Ensure the contract is funded with sufficient STX for prizes
5. **Monitor Progress**: Track player progress and stage completions

## 💻 Development

### Local Setup

1. Clone the repository:
   \`\`\`
   git clone https://github.com/yourusername/cryptoquest.git
   cd cryptoquest
   \`\`\`

2. Install dependencies:
   \`\`\`
   npm install
   \`\`\`

3. Start the local Stacks blockchain:
   \`\`\`
   npm run start-mocknet
   \`\`\`

4. Deploy the contract:
   \`\`\`
   npm run deploy-contract
   \`\`\`

5. Start the development server:
   \`\`\`
   npm run dev
   \`\`\`

### Testing

Run the test suite:
\`\`\`
npm test
\`\`\`

## 📝 Smart Contract API

### Administrative Functions

- **initialize-hunt**: Activate the hunt and reset state
- **add-stage**: Add a new puzzle stage with clue, solution hash, unlock time, and prize
- **update-timestamp**: Update the current timestamp (for time-based unlocks)

### Player Functions

- **register-player**: Register for the hunt by paying the entry fee
- **submit-solution**: Submit a solution for the current stage
- **get-current-clue**: Retrieve the clue for a specific stage
- **get-player-status**: Check a player's current progress
- **get-stage-winners**: View the winners for a specific stage
- **get-hunt-stats**: Get overall statistics about the hunt

## 🔐 Security Considerations

- Solution hashes are stored on-chain, not the solutions themselves
- Time-locked stages prevent premature access to puzzles
- Entry fees help prevent spam and fund the prize pool
- Administrative functions are protected by principal authorization

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (\`git checkout -b feature/amazing-feature\`)
3. Commit your changes (\`git commit -m 'Add some amazing feature'\`)
4. Push to the branch (\`git push origin feature/amazing-feature\`)
5. Open a Pull Request

---

Built with ❤️ by the CryptoQuest Team
