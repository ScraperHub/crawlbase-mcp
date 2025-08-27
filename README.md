<!-- GitHub-Compatible Banner -->
<div align="center">
  <h2>🎉 Claim Your <ins>1,000 Free Credits</ins></h2>
  <p><strong>Start using our Crawling API today to extract data at scale — no setup, no maintenance.</strong></p>
  <table>
    <tr>
      <td align="center">✅ <strong>JS Rendering Included</strong></td>
      <td align="center">🛡️ <strong>CAPTCHA Handling</strong></td>
      <td align="center">💳 <strong>No Credit Card Required</strong></td>
    </tr>
  </table>
  <br>
  <a href="https://crawlbase.com/signup?utm_source=github&utm_medium=referral&utm_campaign=github_tracking
">
    <img src="https://img.shields.io/badge/Start%20for%20Free-Get%201000%20Credits-4CAF50?style=for-the-badge&logo=rocket&logoColor=white" alt="Start for Free">
  </a>
</div>


# What is Crawlbase MCP?

Crawlbase MCP is a Model Context Protocol (MCP) server that bridges AI agents and the live web. Instead of relying on outdated training data, your LLMs can now fetch fresh, structured, real-time content — powered by Crawlbase’s proven crawling infrastructure trusted by 70,000+ developers worldwide.

It handles the complexity of scraping for you:

- JavaScript rendering for modern web apps
- Proxy rotation & anti-bot evasion
- Structured outputs (HTML, Markdown, screenshots)

## How It Works

- Get Free Crawlbase Tokens → Sign up at [Crawlbase ↗️](https://crawlbase.com/signup?utm_source=github&utm_medium=readme&utm_campaign=mcp_launch&utm_content=signup_link), get free Normal, and JavaScript tokens.
- Set Up MCP Configuration → Configure the MCP server in your preferred client (Claude, Cursor, or Windsurf) by updating the MCP Servers settings.
- Start Crawling → Use commands like **crawl**, **crawl_markdown**, or **crawl_screenshot** to bring live web data into your AI agent.

## Setup & Integration

### Claude Desktop

1. Open Claude Desktop → File → Settings → Developer → Edit Config
2. Add to `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "crawlbase": {
      "type": "stdio",
      "command": "npx",
      "args": ["@crawlbase/mcp@latest"],
      "env": {
        "CRAWLBASE_TOKEN": "your_token_here",
        "CRAWLBASE_JS_TOKEN": "your_js_token_here"
      }
    }
  }
}
```

### Cursor IDE

1. Open Cursor IDE → File → Preferences → Cursor Settings → Tools and Integrations → Add Custom MCP
2. Add to `mcp.json`:

```json
{
  "mcpServers": {
    "crawlbase": {
      "type": "stdio",
      "command": "npx",
      "args": ["@crawlbase/mcp@latest"],
      "env": {
        "CRAWLBASE_TOKEN": "your_token_here",
        "CRAWLBASE_JS_TOKEN": "your_js_token_here"
      }
    }
  }
}
```

### Windsurf IDE

1. Open WindSurf IDE → File → Preferences → WindSurf Settings → General → MCP Servers → Manage MCPs → View raw config
2. Add to `mcp_config.json`:

```json
{
  "mcpServers": {
    "crawlbase": {
      "type": "stdio",
      "command": "npx",
      "args": ["@crawlbase/mcp@latest"],
      "env": {
        "CRAWLBASE_TOKEN": "your_token_here",
        "CRAWLBASE_JS_TOKEN": "your_js_token_here"
      }
    }
  }
}
```

🔑 Get your free tokens at [Crawlbase ↗️](https://crawlbase.com/signup?utm_source=github&utm_medium=readme&utm_campaign=mcp_launch&utm_content=signup_link).

## Usage

Once configured, use these commands inside Claude, Cursor, or Windsurf:

* crawl → Fetch raw HTML
* crawl_markdown → Extract clean Markdown
* crawl_screenshot → Capture screenshots

Example prompts:

- “Crawl Hacker News and return top stories in markdown.”
- “Take a screenshot of TechCrunch homepage.”
- “Fetch Tesla investor relations page as HTML.”

## Use Cases

- Market research → Pull live data from competitors, news, and reports
- E-commerce monitoring → Track products, reviews, and prices in real time
- News & finance feeds → Keep AI agents up-to-date with live events
- Autonomous AI agents → Give them vision to act on fresh web data

## Resources & Next Steps

Looking to supercharge your AI agents with live web data? Get started here:

- [✍️ Learn More – See how MCP powers AI agents with real-time web data ↗️](https://crawlbase.com/blog/introducing-crawlbase-mcp-feed-real-time-web-data-to-the-llms/?utm_source=github&utm_medium=readme&utm_campaign=mcp_launch&utm_content=learn_more)
- [🌐 Crawlbase Website – Get free tokens & start crawling today ↗️](https://crawlbase.com/?utm_source=github&utm_medium=readme&utm_campaign=mcp_launch&utm_content=website_link)

---

Copyright 2025 Crawlbase
