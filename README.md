# 🚂 GDG Hackathon: Gemma Local Setup

Welcome to the official offline AI setup repository for our train hackathon! 

Since internet connectivity on a moving train is often unstable, this repository provides everything you need to run Google's **Gemma** open models locally on your laptop. By following these guides, you will have a powerful, fully offline AI coding assistant integrated directly into your editor before we board.

## 📦 What's in this Repository?

We have prepared dedicated setup guides for all major operating systems. Choose the file that matches your machine:

*   **[Windows Setup](windows-setup.md)**: Setup instructions for Windows utilizing PowerShell or the official installer.
*   **[macOS Setup](macos-setup.md)**: Optimized instructions for Apple Silicon (M-series) using Homebrew.
*   **[Linux Setup](linux-setup.md)**: Terminal-based instructions tailored for Ubuntu/Debian users.

## 🤖 The Model Stack

We are exclusively using Google's open-weight models, scaled for different laptop hardware constraints:
*   **Gemma 4 (`e4b` & `12b`):** Google's latest highly efficient models for general logic, reasoning, and web development queries.
*   **Gemma 3 (`4b` & `12b`):** Excellent, stable all-rounder models for complex architectural questions.
*   **CodeGemma (`2b` & `7b`):** Lightning-fast models specifically trained and optimized for inline code completion.

## 🛠️ The Tooling

To make this seamless, participants will be using:
1.  **Ollama**: A lightweight runner that operates quietly in the background to serve the models locally.
2.  **Continue.dev**: A VS Code extension that connects directly to Ollama, providing an offline chat and autocomplete experience right in your IDE.

## ⚠️ Important Pre-Departure Checklist

Please ensure you complete the setup for your respective operating system **before arriving at the station**. Downloading the runner, the IDE extension, and pulling the actual model weights requires a stable Wi-Fi connection. Once downloaded, everything runs 100% offline.

Happy hacking!