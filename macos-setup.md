# GDG Siliguri Hackathon: macOS Offline AI Setup

Welcome to the GDG Siliguri Hackathon! Since internet connectivity on the train will be spotty, we are leveraging Google's powerful open-weight **Gemma** models to run AI locally on your laptops.

Please complete this setup **before boarding the train** while you have stable Wi-Fi.

## Recommended Google Models by Hardware
*   **8GB RAM (Base M1/M2/M3):** 
    *   `gemma4:e4b` (Google's latest highly efficient 4B model)
    *   `gemma3:4b` (Great all-rounder)
    *   `codegemma:2b` (Lightning-fast, optimized for code completion)
*   **16GB+ RAM (Pro/Max Models):** 
    *   `gemma4:12b` (Highly capable and handles complex logic)
    *   `gemma3:12b` (Excellent reasoning capabilities)
    *   `codegemma:7b` (Heavy-duty coding assistant)

## Step 1: Install the Runner
The runner is highly optimized for Apple Silicon and natively utilizes Mac's unified memory and Metal GPU. If you have Homebrew installed, simply open your terminal and run:

```bash
brew install ollama
```
*(Alternatively, download the Mac installer from ollama.com/download, extract the zip, and drag the app to your Applications folder).*

## Step 2: Pull the Models
Open your terminal and download your preferred models:

```bash
# For 8GB Macs
ollama pull gemma4:e4b
ollama pull codegemma:2b

# For 16GB+ Macs
ollama pull gemma4:12b
ollama pull codegemma:7b
```

## Step 3: Run and Test Offline
Turn off your Wi-Fi completely, then run:

```bash
ollama run gemma4:e4b
```

When the `>>>` prompt appears, test its capabilities with a realistic scenario: *"How do I develop a frontend React app using Firebase Studio and connect that app with a Firebase backend?"*
*(Type `/bye` to exit).*

## 💡 Pro-Tip: VS Code Integration
1. Open **VS Code** and install the **Continue.dev** extension.
2. Click the Continue icon in the left sidebar.
3. Select **Ollama** as your provider and choose your Google model (e.g., `codegemma:2b` for autocomplete).
