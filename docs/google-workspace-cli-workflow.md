# Google Workspace CLI Workflow

A CLI-backed Google Workspace lane is useful for email search, calendar review, Drive lookup, Sheets automation, and Docs export/cat operations.

## Setup pattern

```bash
gog auth credentials /path/to/client_secret.json
gog auth add you@example.com --services gmail,calendar,drive,contacts,sheets,docs
gog auth list
```

## Common operations

```bash
gog gmail search 'newer_than:7d' --max 10
gog calendar events <calendarId> --from <iso> --to <iso>
gog drive search "query" --max 10
gog sheets get <sheetId> "Tab!A1:D10" --json
gog docs cat <docId>
gog docs export <docId> --format txt --out /tmp/doc.txt
```

## Approval boundary

Reading/searching can be low-risk. Sending mail, creating events, changing Sheets, or overwriting Docs should require a clear user request and final review.
