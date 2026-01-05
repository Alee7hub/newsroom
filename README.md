# Newsroom - AI-Powered News Aggregator

An n8n workflow that transforms RSS feeds into intelligent, summarized news digests delivered straight to your Discord channel.

## 🎯 What It Does

This workflow automatically:
- 📰 Pulls news from multiple RSS sources
- 🔍 Filters articles by date and relevance
- 🤖 Summarizes content using AI (LLM)
- 📬 Sends consolidated updates to Discord in a single message

Instead of managing multiple RSS feeds and notification systems, get everything you care about in one clean, AI-summarized message.

## 🚀 Getting Started

### Prerequisites
- [n8n](https://n8n.io/) (self-hosted or cloud)
- OpenWeatherMap API credentials (optional, for weather updates)
- Discord webhook URL
- LLM API access (e.g., OpenAI, Anthropic)

### Installation

1. Clone this repository:
```bash
git clone <your-repo-url>
cd newsroom
```

2. Import the workflow into n8n:
   - Open your n8n instance
   - Go to **Workflows** → **Import from File**
   - Select `news-assistant.json`

3. Configure your credentials:
   - OpenWeatherMap API (if using weather updates)
   - Discord Webhook URL
   - LLM provider credentials

4. Customize your news sources:
   - Edit the RSS Read node
   - Add your preferred RSS feed URLs
   - Adjust the filter criteria (date range, keywords, etc.)

## ⚙️ Workflow Overview

The workflow includes:
- **RSS Feed Reader** - Pulls articles from configured sources
- **Date Filter** - Shows only recent news (last 3 hours by default)
- **AI Summarizer** - Condenses articles into 2-3 sentence summaries
- **Discord Integration** - Sends formatted messages to your channel
- **Weather Update** - Optional weather information

## 🎥 YouTube Tutorial

Check out my YouTube channel for a detailed walkthrough of this workflow!

## 🛠️ Customization

- **News Sources**: Modify RSS feed URLs in the RSS Read node
- **Time Range**: Adjust the Filter node to change how recent articles should be
- **Summary Length**: Edit the AI prompt to change summary style/length
- **Discord Format**: Customize the message template in the Discord node
