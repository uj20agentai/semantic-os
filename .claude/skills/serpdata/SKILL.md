---
name: serpdata
description: Search Google SERP results via SerpData API. Use when the user wants to check Google search rankings, see top 10 organic results for a keyword, analyze SERP features (local pack, people also ask, related searches), or do competitive analysis for Polish market SEO.
argument-hint: [keyword] [optional: language] [optional: country]
allowed-tools: Bash(curl *)
---

# SerpData SERP Checker

Query Google search results via the SerpData API and return structured SERP data.

## API Details

- **Endpoint**: `https://api.serpdata.io/v1/search`
- **Method**: GET
- **Auth**: Bearer token in Authorization header

## Usage

When invoked, execute the following curl command with the user's keyword:

```bash
curl --silent --request GET \
  --url "https://api.serpdata.io/v1/search?keyword=$KEYWORD_ENCODED&hl=$HL&gl=$GL" \
  --header "Authorization: Bearer nodeshub_1cf9b3291f87e7a06e98bbb95902c3a0-TLltoqELg9I"
```

### Parameters

| Parameter | Default | Description |
|-----------|---------|-------------|
| keyword   | required | Search query (URL-encode spaces as `+`) |
| hl        | pl      | Language (pl, en, de, etc.) |
| gl        | pl      | Country (pl, us, de, etc.) |

If the user provides only a keyword, default to `hl=pl` and `gl=pl`. If the user specifies a language or country, use those values instead. Use `$ARGUMENTS[0]` as the keyword, `$ARGUMENTS[1]` as language (if provided), `$ARGUMENTS[2]` as country (if provided).

## Output Format

After receiving the API response, present the results as follows:

### 1. Top 10 Organic Results (always show)

Display as a numbered table:

| # | Position | Domain | Title | URL |
|---|----------|--------|-------|-----|
| 1 | {global_pos} | {domain} | {title} | {url} |

Extract these from `data.results.organic_results`. Use `global_pos` for the actual SERP position and `pos` for the organic-only rank.

### 2. SERP Features Found (show if present)

List which snippets were found from `data.results.snippets_found` (e.g., local_pack, people_also_ask, related_searches).

### 3. Local Pack (show if present)

If `local_pack` exists in snippets, list the businesses:
- Name, URL, rank

### 4. People Also Ask (show if present)

If `people_also_ask` exists, list the questions.

### 5. Related Searches (show if present)

If `related_searches` exists, list the queries.

## Error Handling

- If the API returns an error or `success: false`, report the error to the user.
- If no organic results are found, inform the user.
- If the request times out, suggest trying again.

## Example

User runs: `/serpdata pomoc drogowa Krakow`

Expected: curl call with `keyword=pomoc+drogowa+Krakow&hl=pl&gl=pl`, then a formatted table of top 10 organic results plus any SERP features found.
