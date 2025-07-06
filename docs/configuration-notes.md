# Configuration Notes

## Setup Instructions
1. **Install n8n**: Ensure n8n is installed and running (e.g., locally or via n8n Cloud).
2. **Add Credentials**:
   - **OpenAI**: Obtain an API key from [OpenAI](https://platform.openai.com/) and add it in n8n Credentials.
   - **Gmail**: Set up OAuth via Google Cloud Console and authorize in n8n Credentials.
3. **Import Workflow**: Import `rss-news-summarizer-workflow.json` in n8n (Workflow > Import).
4. **Configure Nodes**:
   - Update the RSS feed URL if using a different source.
   - Adjust polling times in RSS Feed Trigger if needed.
5. **Test**: Execute the workflow manually, then activate it.

## Troubleshooting
- **No Email**: Check Gmail credentials and n8n execution logs.
- **No Summary**: Verify OpenAI API key and AI Agent prompt.
- **Memory Issues**: Ensure the `link` field is passed correctly via the Set node.