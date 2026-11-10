# Russia Import Export Data MCP

**Russia Customs Data: Importers, Suppliers & HS Codes.** Russia import export data for your AI assistant. Search Russia customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Russia trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/russia
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Russia: the server tells your AI to filter on `RU` unless you ask about another country

## Russia data coverage

- **Years:** 2013–2025
- **Records:** Import declarations: Russian importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `RU` (use `buyerCountry: "RU"` for imports into Russia)
- **Common products:** aluminium (HS 7601), industrial machinery (HS 8479), cars (HS 8703), phones (HS 8517)

> Party names are stored as declared, in Russian Cyrillic; search in Cyrillic.

## Notable traders in the data

Companies that appear most often in recent Russia records (by number of declaration lines, not value):

**Importers**

- Tatprof
- International Aluminium Company

## Example prompts

- *"Who are the top importers of aluminium (HS 7601) into Russia?"*
- *"What does Tatprof import, and from which countries?"*
- *"List Russian importers of industrial machinery (HS 8479) in 2024"*
- *"Which countries supply cars (HS 8703) to Russia, by year?"*
- *"Show recent import shipments of phones (HS 8517) into Russia"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Russia import data, Russia export data, Russia customs data, Russia shipment data, importers in Russia, Russia buyers and suppliers, HS code search, таможенные данные России, импорт России, импортеры России, ТН ВЭД
