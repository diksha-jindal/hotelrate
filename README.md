# 🏨 HotelRate MCP — AI-Powered Hotel Price Comparison

<p align="center">
  <strong>Compare hotel prices across multiple booking platforms using AI and automation.</strong>
</p>

![Python](https://img.shields.io/badge/Python-3.12+-blue?logo=python)
![MCP](https://img.shields.io/badge/MCP-Compatible-purple)
![Playwright](https://img.shields.io/badge/Playwright-Automation-green?logo=playwright)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Overview

HotelRate MCP is an MCP-based hotel price comparison system that helps AI agents retrieve and compare hotel offers across Trip.com, Booking.com, Agoda, and Google Hotels through a unified interface.

It supports demo mode for testing and live browser-based searches using Playwright.

## ✨ Features

- 🔎 Multi-platform hotel price comparison
- 🤖 AI-agent integration using Model Context Protocol (MCP)
- 🌐 Browser automation with Playwright
- ⚡ Batch queries for multiple hotels
- 📊 Structured hotel offers and pricing data
- 🧪 Environment health checks and diagnostics
- 🔌 Optional REST API using FastAPI

## 🛠️ Tech Stack

Python • MCP • Playwright • FastAPI • Pydantic • pytest

## 🏗️ Architecture

```text
AI Agent / MCP Client
        |
        v
    MCP Server
        |
        v
   Quote Service
        |
   +----+----+----+
   |    |    |    |
 Trip Booking Agoda Google
        |
        v
 Result Normalization
        |
        v
 Structured Hotel Offers
```

## ⚙️ Installation

```bash
git clone https://github.com/seanbabalala/hotelrate-crawl.git
cd hotelrate-crawl
pip install -e .
cp .env.example .env
hotelrate-mcp doctor
```

For live searches, configure your environment and run:

```bash
hotelrate-mcp setup
```

## 🔌 Available MCP Tools

| Tool | Description |
|---|---|
| `hotel_quote` | Retrieve offers for a hotel |
| `hotel_quote_batch` | Query multiple hotels |
| `list_platforms` | Check supported platforms |
| `health_check` | Check system readiness |

## 🧪 Testing with MCP Inspector

```bash
npx @modelcontextprotocol/inspector hotelrate-mcp
```

Open the URL printed in the terminal, navigate to **Tools → hotel_quote**, enter the hotel details, and run the tool to inspect the results.

## 🔮 Future Enhancements

- Historical hotel price tracking
- Price-drop notifications
- Improved room matching
- Interactive price comparison dashboard

## 🔒 Security

- Keep credentials and `.env` files private.
- Never commit browser sessions or authentication tokens.
- Respect website terms and access restrictions.

## 📄 License

MIT License. Retain the applicable license and original attribution when redistributing the code.

---

<p align="center">
  <strong>Making hotel price comparison simpler with AI and automation.</strong>
</p>