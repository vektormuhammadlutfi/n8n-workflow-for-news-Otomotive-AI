# News AI Otomotif Workflow

Automated workflow for aggregating, filtering, summarizing, and distributing strategic news from multiple Indonesian RSS sources, with a focus on automotive topics. Integrates AI summarization and Telegram notifications.

![Workflow Diagram](https://raw.githubusercontent.com/vektormuhammadlutfi/n8n-workflow-for-news-Otomotive-AI/main/image.png)

## Features

- Aggregates news from up to 9 RSS feeds (CNN Indonesia, CNBC Indonesia, Kumparan, Tempo, Okezone, Republika, Antara News, Fajar Sulsel, Detik).
- Filters news by publication date (default: last 7 days, configurable).
- Sorts articles by date for relevance.
- Limits the number of news items (default: 10, configurable).
- Transforms and formats news data for AI processing.
- Uses AI (OpenAI or OpenRouter) to generate executive summaries in Indonesian, prioritizing automotive and strategic topics.
- Includes sentiment analysis and strategic filtering in summary.
- Distributes summaries via Telegram notifications.
- Highly customizable: add/remove RSS feeds, adjust filters, change output format, and switch notification channels.

## Setup

1. Configure RSS feed URLs in the respective nodes.
2. Connect your Telegram and AI provider credentials (OpenAI or OpenRouter).
3. Adjust the schedule trigger for desired execution time (default: daily at 8 AM).
4. Modify filter and limit nodes to set date range and number of articles.
5. Customize AI prompt templates for summary formatting and language.
6. Test workflow to ensure all integrations are working.

## Customization

- Add or remove RSS feeds by editing the Merge node and RSS nodes.
- Change the date filter in the 'Filter by date' node (e.g., last N days).
- Set the maximum number of news items in the 'Limit news to x' node.
- Update summary formatting and language in the AI prompt nodes.
- Switch notification channels (e.g., Telegram, Slack, Email) as needed.

## Usage

- Ideal for content managers, marketers, and executives needing daily strategic news updates.
- Automates news monitoring, filtering, and summarization for efficient decision-making.
- Delivers concise, actionable executive summaries with source links and sentiment analysis.

## Workflow Diagram

See n8n visual workflow for node connections and data flow.

## License

MIT

## Author

Muhammad Lutfi

## Notes

- Ensure all credentials are securely stored and managed.
- Review AI-generated summaries for accuracy and relevance.
- Monitor workflow execution logs for errors or missed feeds.
