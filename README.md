AgenticAI Framework - Intelligent Test Automation
🚀 Overview
The AgenticAI Framework is an advanced test automation system that automatically generates complete test suites from recorded user interactions. It uses AI-powered agents to create Feature files, Page Object Models (POMs), and Step Definitions with perfect alignment and intelligent deduplication.

📦 VS Code Extension - Quick Start
🎯 The Fastest Way to Get Started
The AgenticAI Framework Extension for VS Code allows you to create complete test automation projects in seconds!

Features
✨ One-Click Project Creation - Generate complete test automation projects instantly
🔐 Encrypted AI Agents - 19 pre-encrypted Python agents (1.02 MB) for secure deployment
🎭 Playwright Integration 
🥒 Cucumber BDD - Full Cucumber 10.0.0 support with TypeScript
📦 Bundled Dependencies - All npm packages included (no internet required for setup)
🔧 Auto-Configuration - Pre-configured AI-global-settings.json and cucumber.js
🐍 Python Ready - Automatic pip install for pycryptodome 3.23.0, playwright, pytesseract
🤖 LLM Integration - Azure OpenAI support for AI-enhanced scenario generation
📚 Documentation - README.md and QUICK_START.md included in every project

Installation
Open VS Code
Go to Extensions (Ctrl+Shift+X)
Search for "AgenticAI Framework"
Click Install
Or install from VSIX:

Download agenticai-framework-1.2.9.vsix
Extensions → ⋯ menu → Install from VSIX
Reload VS Code
Getting Started
Prerequisites
Visual Studio Code 1.80.0 or later
Node.js 18.x or later
Python 3.8 or later
pip (Python package manager)
Creating Your First Project
Open Command Palette (Ctrl+Shift+P)
Type "Create AgenticAI Project"
Enter your project name
Choose a folder location
Wait for project creation and automatic dependency installation
Open the project when prompted
The extension will:

✅ Create the complete project structure
✅ Copy all node_modules (12.56 MB)
✅ Generate configuration files (AI-global-settings.json, cucumber.js)
✅ Copy README.md and QUICK_START.md for reference
✅ Run npm install (verifies packages)
✅ Run pip install -r requirements.txt (installs Python packages)
What Gets Created
your-project/
├── AgenticAI/
│   ├── src/
│   │   ├── agents/agents/          # 19 encrypted agent files (.enc)
│   │   │   ├── autogen.py          # Wrapper with CLI interface
│   │   │   ├── pega_test_config.py # User configuration
│   │   │   └── test_llm_connection.py # LLM connectivity test
│   │   ├── core/                   # 6 encrypted core modules
│   │   │   ├── llm_client.enc      # Azure OpenAI integration
│   │   │   └── framework.enc       # Core framework
│   │   └── _encrypted_runtime.py   # Decryption loader
│   └── pega_test_artifacts/        # Generated test artifacts
│       ├── features/               # Cucumber feature files
│       └── step_definitions/       # TypeScript step definitions
├── support/
│   ├── hooks.ts                    # Cucumber hooks with PegaSUT
│   └── world.ts                    # Custom World interface
├── logs/                           # Test execution logs
├── screenshots/                    # Test screenshots
├── reports/json/                   # Cucumber JSON reports
├── node_modules/                   # All dependencies (2715 files)
├── README.md                       # Project documentation
├── QUICK_START.md                  # Quick start guide
├── AI-global-settings.json         # Pega test configuration
├── cucumber.js                     # Cucumber configuration
├── package.json                    # NPM configuration
├── tsconfig.json                   # TypeScript configuration
├── requirements.txt                # Python dependencies
├── .npmrc                          # Pega registry config
└── README.md                       # Project documentation

Running Your Tests
# Record user interactions
cd AgenticAI/src/agents/agents
python autogen.py --url https://your-app.com --headful

Extension Benefits
🚀 Zero Setup Time - Complete project in <2 minutes
🔐 Encrypted Agents - 12 AI agents (825.63 KB) pre-encrypted
📦 Bundled Dependencies - No internet required after install
🎭 Playwright Ready
🥒 Cucumber Ready - Full Cucumber 10.0.0 + TypeScript support
✅ Cross-Platform - Works on Windows, macOS, Linux
🎯 Key Features
✨ Features-First BDD Approach
Behavior-Driven Development: Define business scenarios before implementation
Living Documentation: Features serve as executable requirements
Test-Driven: Implementation follows specified behavior
🧠 Ultimate Priority-Based Locator Technology
Self-Healing: 110 → 88 → 78 → 60 priority level fallback system
Intelligent Element Detection: PascalCase method naming (e.g., UserIdentifierFill())
Robust Selectors: Multi-tier locator strategies for maximum reliability
🔄 AI-Powered Generation Pipeline
Features → Define what the application should do
POMs → Implement how to interact with pages
Step Definitions → Connect features to POMs seamlessly
🎭 Smart Deduplication System
Zero Duplicates: Prevents "Multiple step definitions match" errors
Signature Tracking: Uses Set[str] to track generated step signatures
Action-Aware: Handles fill, select, and click actions intelligently
📋 Architecture
Generation Order
recorded_test_data.json
        ↓
    🎯 Features Generated (BDD scenarios)
        ↓  
    📄 POMs Generated (Priority-based locators)
        ↓
    🔗 Step Definitions Generated (Bridge features ↔ POMs)
        ↓
    ✅ Complete Test Suite Ready

Directory Structure
AgenticAI/
├── src/agents/agents/
│   ├── autogen.py                      # Main orchestrator
│   ├── ai_to_complete_system.py   # Core generation engine
│   └── Test_artifacts/
│       ├── features/                   # Cucumber feature files
│       ├── step_definitions/           # TypeScript step definitions  
│       └── page_objects/              # Priority-based POMs
├── recorded_test_data.json            # User interaction recordings
└── README.md                         # This file

📄 License
This project is proprietary software. All rights reserved.

🙏 Acknowledgments
Playwright - For reliable browser automation
Cucumber - For BDD framework excellence
TypeScript - For type-safe test development
Built with ❤️ by the VA 

Record once, test forever: agents that never sleep, never complain, and always deliver — an innoVAtion in automation
