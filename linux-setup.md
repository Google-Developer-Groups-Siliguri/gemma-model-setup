# GDG Siliguri Hackathon: Linux (Ubuntu) Offline AI Setup

Welcome to the GDG Siliguri Hackathon! Since internet connectivity on the train will be spotty, we are leveraging Google's powerful open-weight **Gemma** models to run AI locally on your laptops.

Please complete this setup **before boarding the train** while you have stable Wi-Fi.

## Recommended Google Models by Hardware
*   **8GB RAM (Standard Laptops):** 
    *   `gemma4:e4b` (Google's latest highly efficient 4B model)
    *   `gemma3:4b` (Great all-rounder)
    *   `codegemma:2b` (Lightning-fast, optimized for code completion)
*   **16GB+ RAM (Pro Laptops):** 
    *   `gemma4:12b` (Highly capable and handles complex logic)
    *   `gemma3:12b` (Excellent reasoning capabilities)
    *   `codegemma:7b` (Heavy-duty coding assistant)

## Step 1: Install the Runner
Linux natively supports Ollama and will automatically detect your NVIDIA GPU if the proprietary drivers are installed. Open your terminal and run the official installation script:

```bash
curl -fsSL https://ollama.com/install.sh | sh
```

## Step 2: Pull the Models
Download your preferred models:

```bash
# For standard 8GB RAM laptops
ollama pull gemma4:e4b
ollama pull codegemma:2b

# For 16GB+ RAM laptops
ollama pull gemma4:12b
ollama pull codegemma:7b
```

## Step 3: Run and Test Offline
Turn off your Wi-Fi completely, then run:

```bash
ollama run gemma4:e4b
```

When the `>>>` prompt appears, test it with a web development prompt. For example, you can ask it: *"Write a Next.js App Router component that handles routing for a dashboard."*
*(Type `/bye` to exit).*

## 💡 Pro-Tip: VS Code Integration
1. Open **VS Code** and install the **Continue.dev** extension.
2. Click the Continue icon in the left sidebar.
3. Select **Ollama** as your provider and choose your Google model (e.g., `codegemma:2b` for autocomplete).
