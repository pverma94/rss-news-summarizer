# RSS News Summarizer

An automated workflow using n8n to summarize RSS news articles and send them via email.

## Overview
This project fetches articles from an RSS feed (e.g., BBC News), summarizes their content using an AI model (OpenAI), and emails the summaries with memory context to retain article-specific insights. The workflow runs hourly and is built for personal news monitoring.

## Features
- Polls an RSS feed every hour (configurable).
- Fetches full article content via HTTP Request.
- Summarizes content using OpenAI with Simple Memory for context.
- Sends summaries to a specified email address.

## Prerequisites
- [n8n](https://n8n.io/) installed (local or cloud).
- OpenAI API key.
- Gmail account with OAuth credentials.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/rss-news-summarizer.git
   cd rss-news-summarizer

2. Import the workflow:
    - Open n8n, go to Workflow > Import, and select workflow/rss-news-summarizer-workflow.json.

3. Configure Credentials
    - Add OpenAI API key in n8n Credentials.
    - Set up Gmail OAuth and authorize.

4. Adjust settings:
    - Update the RSS feed URL in the RSS Feed Trigger node if needed.
    - Modify the recipient email in the Gmail node.

5. Activate the workflow.
    - After all configurations are complete, **toggle the workflow to "Active"** in n8n.

Your summarized news emails will now be delivered on schedule!

## Tech Stack
    - [n8n](https://n8n.io) – Workflow automation
    - [OpenAI](https://openai.com) – Article summarization
    - [Gmail](https://gmail.com) – Email delivery

## License
This project is licensed under the MIT License.

## Support
Feel free to raise an issue or contribute to improvements. For general n8n setup help, visit the [n8n documentation](https://docs.n8n.io).