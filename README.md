# Wormhole AI Agent

Wormhole AI Agent designed to simplify cross-chain operations on the Solana blockchain. Built with **LangChain**, **Solana Agent Kit**, and the **Wormhole Protocol**, this agent allows users to interact with blockchain bridges using natural language.

## 🚀 Features

*   **Natural Language Interface**: Chat with the agent to execute complex blockchain transactions.
*   **Cross-Chain Transfers**: Bridge tokens between supported chains (Ethereum, Solana, Arbitrum, Optimism, etc.) using Wormhole.
*   **CCTP Support**: Native USDC transfers across chains using Circle's Cross-Chain Transfer Protocol.
*   **Asset Management**: Create wrapped tokens and manage assets on Solana.
*   **Chain Discovery**: Query supported chains and network status instantly.
*   **Real-Time Logs**: View the agent's "thought process" and tool execution logs in a dedicated panel.

## 🛠 Tech Stack

*   **Frontend**: Next.js 15 (App Router), React 19, Tailwind CSS 4
*   **AI/LLM**: LangChain, LangGraph, OpenAI (GPT-4o-mini)
*   **Blockchain**: Solana Agent Kit, Wormhole SDK
*   **State**: Keyv (SQLite)

## 📋 Prerequisites

Before running the project, ensure you have:

*   Node.js 18+ installed.
*   A **Solana Wallet** (Private Key) with some SOL for transaction fees.
*   An **OpenAI API Key** (with credits available).
*   A Solana RPC URL (e.g., from Helius, QuickNode, or public endpoints).

## ⚡ Getting Started

1.  **Clone the repository**
    ```bash
    git clone <repository-url>
    cd wormhole-ai-agent
    ```

2.  **Install dependencies**
    ```bash
    npm install
    ```

3.  **Configure Environment Variables**
    Create a `.env` file in the root directory:
    ```bash
    cp .env.example .env
    ```
    
    Add your keys:
    ```env
    # Solana Configuration
    SOLANA_PRIVATE_KEY=your_base58_private_key
    RPC_URL=https://api.mainnet-beta.solana.com

    # OpenAI Configuration
    OPENAI_API_KEY=sk-...
    ```

4.  **Run the Development Server**
    ```bash
    npm run dev
    ```

    Open [http://localhost:3000](http://localhost:3000) in your browser.

## 💬 Usage Examples

Once the agent is running, try these prompts:

*   **Check Support**: "What chains are supported by Wormhole?"
*   **Bridge Funds**: "Transfer 0.1 SOL to Ethereum address 0x123..."
*   **USDC Transfer**: "Bridge 5 USDC to Arbitrum via CCTP."
*   **Wrap Tokens**: "Create a wrapped token for [Mint Address]."

## 📄 License

This project is licensed under the MIT License.
