# MCP Setup Guide

This guide will help you set up a Python environment for demonstrating the MCP (Model Context Protocol) POC demo. The steps are compatible with both Windows and macOS systems.

## Prerequisites

Make sure you have the following installed on your system:
- Python (version 3.8 or later)
- pip (Python package manager)
- Git (optional, for version control)

### 1. Clone the Project Repository

#### On Windows:
Open the command prompt and run:
```cmd
mkdir C:\MCP_POC
cd C:\MCP_POC
git clone https://github.com/Ayumilan/MCP.git
```

#### On macOS:
Open the terminal and run:
```bash
mkdir ~/MCP_POC
cd ~/MCP_POC
git clone https://github.com/Ayumilan/MCP.git
```

### 2. Navigate to the Project Directory

#### Windows:
```cmd
cd C:\MCP_POC\MCP
```

#### macOS:
```bash
cd ~/MCP_POC/MCP
```

### 3. Create a Virtual Environment

#### On Windows:
```cmd
python -m venv .venv
.venv\Scripts\activate
```

#### On macOS:
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 4. Install Dependencies

The `requirements.txt` file lists all necessary dependencies for running the MCP POC demo. Install them as follows:

#### On Windows:
```cmd
pip install -r requirements.txt
```

#### On macOS:
```bash
pip install -r requirements.txt
```

### 5. Set Up Environment Variables

Create a `.env` file in the project root. Add the following values:
```env
AZURE_OPENAI_ENDPOINT=****
AZURE_OPENAI_API_KEY=****
AZURE_OPENAI_API_VERSION=***
AZURE_OPENAI_DEPLOYMENT_NAME=***
```
> **Note:** Replace the above values with your own keys and endpoints if applicable.

### 6. Run the Demo
**Run Chatbot:**
Start the chatbot by running:
```cmd
python mcp_chatbot.py
```

### 7. Test Your Setup

Verify the setup by executing sample commands or interacting with the chatbot and tools.

## Troubleshooting

### Dependency Issues
If some packages fail to install, double-check your Python version and run `pip install --upgrade pip` to update your pip version.

### Virtual Environment Activation Issues
Refer to your operating system’s specific requirements for command line or terminal operations.

## Conclusion

This guide should help you quickly set up and demonstrate the MCP Proof of Concept. Feel free to explore the additional tools and functionality included in this repository.
