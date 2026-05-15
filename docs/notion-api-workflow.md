# Notion API Workflow

Hermes can help operate Notion-backed workflows when the task is bounded and credentials remain local. This is a public-safe pattern, not a credentialed setup dump.

## Useful operations

- search pages and databases
- read a page by id
- create a page in a database
- query a database/data source
- update page properties
- append blocks to a page

## Example command shape

```bash
export NOTION_KEY="<your integration token>"
curl -X POST "https://api.notion.com/v1/search" \
  -H "Authorization: Bearer $NOTION_KEY" \
  -H "Notion-Version: 2025-09-03" \
  -H "Content-Type: application/json" \
  -d '{"query":"page title"}'
```

## Safety boundary

- Store the token outside the repo.
- Share the target Notion page/database with the integration explicitly.
- Review before creating pages, sending external updates, or overwriting content.
