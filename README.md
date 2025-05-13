# SMOLana
The official Github of the SMOLana Project on the SOLana blockchain powered by SMOL agents and python man

# The SMOLana Multi-Agent Automation System 🤖 🌐 ⚡

A Python-based system for running multiple browser automation agents that can interact with Solana blockchain interfaces and perform automated tasks.

## Overview

This system combines web browser automation with Solana blockchain interactions, allowing you to create and manage multiple autonomous agents through a user-friendly Gradio interface. Each agent can:

- Navigate web pages related to Solana
- Interact with elements (clicking, scrolling, searching)
- Handle popups and modals
- Extract information from websites
- Interact with the Solana blockchain (check balances, prices, NFTs)
- Run independently in parallel

## Features

- **Multi-Agent Management**: Create and manage multiple agents, each with their own browser instance
- **Task Queue**: Submit tasks to agents which are processed asynchronously
- **Solana Integration**: Built-in tools for Solana blockchain interactions
- **Screenshot Capture**: View the current state of each agent's browser session
- **Results History**: Track all completed tasks and their results
- **User-Friendly Interface**: Gradio-based UI for easy interaction

## Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/solana-multi-agent-system.git
cd solana-multi-agent-system
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Install Chrome browser and ChromeDriver if not already installed.

## Usage

1. Start the application:
```bash
python main.py
```

2. Open your browser and navigate to the URL displayed in the terminal (typically http://127.0.0.1:7860)

3. Use the Gradio interface to:
   - Create new agents
   - Submit tasks to agents
   - Monitor agent status and results
   - View agent screenshots

## Example Tasks

Here are some example tasks you can submit to your agents:

1. **Check token prices**:
```
Please navigate to https://coinmarketcap.com/currencies/solana/ and tell me the current Solana price.
```

2. **Monitor NFT marketplaces**:
```
Navigate to https://magiceden.io/ and find the floor price of the top 3 collections.
```

3. **Research token information**:
```
Go to https://solscan.io/ and look up information about the Raydium token.
```

4. **Track wallet activity**:
```
Check the balance and recent transactions of the wallet address 8YUVta4Hz7kYnGsxoJrKRYSLaYSSr9cGmhKR7mEz1n9z
```

## System Architecture

The system consists of several components:

1. **SolanaAgentManager**: Manages the lifecycle of agents, task queues, and results
2. **CodeAgent**: The browser automation agent from smolagents library
3. **Solana Tools**: Custom tools for interacting with the Solana blockchain
4. **Gradio Interface**: User interface for controlling the system

## Extending the System

You can extend the system by:

1. Adding new tools in the `solana_agent_tools.py` file
2. Modifying the Gradio interface in `main.py`
3. Implementing additional agent capabilities

## Troubleshooting

- **Chrome crashes**: Make sure you have the latest version of Chrome and ChromeDriver installed
- **Agent stuck**: Check the agent status and restart if necessary
- **Solana RPC errors**: Switch to a different RPC endpoint if you encounter rate limiting

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- Based on the browser automation system from SmolagentsLab
- Utilizes Helium and Selenium for browser automation
- Built with Gradio for the user interface
