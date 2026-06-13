[Dealroom Scraper](https://apify.com/fatihtahta/dealroom-scraper?fpr=data)

# Dealroom Scraper

**Slug:** fatihtahta/dealroom-scraper

## Overview

Dealroom Scraper collects structured company intelligence from Dealroom, including core identity details, market positioning, growth signals, funding context, investor relationships, location data, and web presence attributes. It supports both broad directory-style collection and focused extraction from specific company pages so teams can build clean, comparable datasets at scale. [Dealroom](https://app.dealroom.co) is widely used for startup and innovation ecosystem discovery, making it a strong source for market mapping, benchmarking, and enrichment workflows. The actor standardizes output into analysis-ready JSON records that are easier to use across BI, CRM, and internal data workflows. By automating repetitive collection, it reduces manual research effort and improves consistency across recurring runs.

## Why Use This Actor

- **Market research & analytics teams:** Build comparable company datasets for sector sizing, trend tracking, and ecosystem benchmarking across geographies and themes.
- **Product & content teams:** Identify relevant companies, categories, and signals to support editorial planning, partner discovery, and product opportunity research.
- **Developers & data engineers:** Feed structured company records into ETL jobs, warehouses, and downstream APIs with minimal transformation overhead.
- **Lead generation & enrichment teams:** Expand account lists with firmographic and contextual attributes for segmentation, scoring, and outreach preparation.
- **Competitive monitoring teams:** Re-run targeted collections on a schedule to track changes in funding, growth, positioning, and market presence over time.

## Input Parameters

Provide any combination of URLs, queries, and filters to control what the actor collects.

| Parameter | Type | Description | Default |
| --- | --- | --- | --- |
| `startUrls` | `array[string]` | One or more Dealroom URLs to collect from directly. You can include company profile pages, filtered company directory pages, and public list pages in the same run. | – |
| `limit` | `integer` | Maximum number of listings to save per query/input path. Use lower values for quick validation runs and higher values for broader coverage. Minimum: `1`. | `50000` |
| `proxyConfiguration` | `object` | Optional connection settings for reliability on larger runs. Default setup uses Apify Proxy. Default values: `useApifyProxy: true`, `apifyProxyGroups: ["RESIDENTIAL"]`. | `{"useApifyProxy": true, "apifyProxyGroups": ["RESIDENTIAL"]}` |

## Example Input

```
{
  "startUrls": [
    "https://app.dealroom.co/companies/dazetechnology",
    "https://app.dealroom.co/companies/f/client_focus/consumer",
    "https://app.dealroom.co/lists/17482/list/f/landscapes/anyof_1834"
  ],
  "limit": 1500,
  "proxyConfiguration": {
    "useApifyProxy": true,
    "apifyProxyGroups": ["RESIDENTIAL"]
  }
}
```

## Output

### 6.1 Output destination

The actor writes results to an Apify dataset as JSON records. And the dataset is designed for direct consumption by analytics tools, ETL pipelines, and downstream APIs without post-processing.

### 6.2 Record envelope (all items)

Every dataset record includes the following stable envelope fields:

- **type** *(string, required)*
- **id** *(number, required)*
- **url** *(string, required)*

**Recommended idempotency key:** `type + ":" + id`

Use this key to deduplicate repeated entities across runs and to perform deterministic upserts in downstream storage.

### 6.3 Examples

Example: company (`type = "company"`)

```
{
  "type": "company",
  "id": 1587191,
  "url": "https://app.dealroom.co/companies/dazetechnology",
  "record_id": "12079561-e911-4a8a-bf31-140f35dca628",
  "company_name": "Daze",
  "company_website": "http://daze.eu/",
  "scrape_metadata": {
    "source_page_url": "https://app.dealroom.co/lists/17482",
    "seed_identifier": "15687805e879",
    "seed_input_type": "url",
    "seed_input_value": "https://app.dealroom.co/lists/17482",
    "results_page_index": 1,
    "extraction_method": "embedded_json",
    "scraped_time": 1773204080
  },
  "company_identity": {
    "about": "Daze develops smart EV charging solutions for residential and commercial use.",
    "about_ai_generated": true,
    "can_edit": false,
    "uuid": "12079561-e911-4a8a-bf31-140f35dca628",
    "images": { "100x100": "https://storage.googleapis.com/.../company-logo.png" },
    "is_ai_data": false,
    "is_editorial": false,
    "name": "Daze",
    "path": "dazetechnology",
    "tagline": "Italian EV charging technology company",
    "type": "company",
    "website_url": "http://daze.eu/",
    "listing_page": "https://app.dealroom.co/companies/dazetechnology"
  },
  "market_and_product_profile": {
    "client_focus": [{ "name": "consumer", "count": 1111916 }],
    "corporate_industries": [],
    "country_experience": [],
    "delivery_method": "direct_sales",
    "entity_sub_types": [],
    "industries": [{ "id": 100023, "name": "energy", "slug": "energy", "count": 100895 }],
    "industry_experience": [],
    "innovations_count": 0,
    "lists_ids": [16522, 21270],
    "lists": {
      "items": [{ "id": 16522, "title": "EIC Winners", "type": 1, "is_public": true, "created": "2020-08-04T13:56:10+01:00" }],
      "total": 21
    },
    "sdgs": [{ "id": 33, "name": "affordable and clean energy (#7)", "slug": "affordable_and_clean_energy_7_" }],
    "service_industries": [],
    "sub_industries": [{ "id": 19, "name": "energy efficiency", "slug": "energy_efficiency", "count": 5300 }],
    "tags": [{ "id": 20269, "name": "ev charging", "slug": "ev_charging", "is_verified": false, "count": 1203 }],
    "tech_stack": [
      {
        "id": 669,
        "name": "bootstrap",
        "company": {
          "uuid": "ca4f05c0-a588-4d57-9e4d-1120926b7e8e",
          "name": "Bootstrap",
          "entity_type": "organization",
          "labels": ["company", "investor"],
          "path": "bootstrap",
          "type": "corporate",
          "images": { "32x32": "https://storage.googleapis.com/.../32.png", "74x74": "https://storage.googleapis.com/.../74.png", "100x100": "https://storage.googleapis.com/.../100.png" }
        },
        "categories": [{ "id": 432, "name": "ui frameworks" }]
      }
    ],
    "technologies": [{ "id": 20, "name": "iot internetofthings", "slug": "iot_internetofthings", "count": 15801 }]
  },
  "growth_and_traction": {
    "employees_chart": [{ "date": "2025-12-09", "value": 8.5 }],
    "employees_latest": 9.1,
    "employee_12_months_growth_percentile": "top half",
    "employee_12_months_growth_unique": 56433,
    "similarweb_12_months_growth_percentile": "top half",
    "similarweb_12_months_growth_unique": 294525,
    "employees": "51-200",
    "job_offers_total": 0,
    "similarweb_chart": [{ "date": "2026-02-01", "value": 41000 }],
    "similarweb_hidden": false,
    "team_total": 7,
    "traffic": { "visitors": "41000", "sources": [], "top_countries": [] }
  },
  "funding_and_financials": {
    "current_and_prev_year_fundings_num": 1,
    "exits_higher_800m": 0,
    "fundings_investor": [],
    "income_streams": [{ "id": 4, "name": "selling own inventory", "slug": "selling_own_inventory", "count": 316297 }],
    "investments_higher_800m": 0,
    "investments_num": 0,
    "investments": [],
    "investor_exits_funding_enhanced": 0,
    "investor_exits_num": 0,
    "investor_total_rank": 9999,
    "investor_total": 0,
    "kpi_summary": {
      "id": 1587191,
      "last_update_date": "2025-08-19T15:08:46+01:00",
      "currency": "EUR",
      "share_price_chart": [],
      "share_price_currency": "EUR",
      "latest_share_price_enhanced": { "price": 12.34, "currency": "EUR", "date": "2025-08-19" },
      "values": [{ "year": 2024, "valuation": 35000000, "valuation_source": "kpi", "revenue": 7033302, "revenue_growth": 35, "revenue_source": 2, "ebitda": null, "ebitda_margin": null, "ebitda_source": null, "profit": -1913856, "profit_margin": -27, "profit_source": 2, "rnd": null, "rnd_margin": null, "rnd_source": null, "ev_revenue": null, "ev_ebitda": null }],
      "values_enhanced": {
        "values": [{ "year": 2024, "valuation": 38500000, "valuation_source": "kpi", "revenue": 7736632, "revenue_growth": 35, "revenue_source": 2, "ebitda": null, "ebitda_margin": null, "ebitda_source": null, "profit": -2105242, "profit_margin": -27, "profit_source": 2, "rnd": null, "rnd_margin": null, "rnd_source": null, "ev_revenue": null, "ev_ebitda": null }],
        "currency": "USD"
      },
      "valuations": [{ "id": 18274503, "year": 2024, "month": 2, "day": 15, "source": "funding", "source_round": "SERIES A", "valuation": 75000000, "valuation_min": 60000000, "valuation_max": 90000000, "valuation_currency": "EUR", "market_cap": null, "market_cap_currency": "EUR", "net_debt": null, "net_debt_currency": null }],
      "revenues_hidden": false,
      "ebitda_hidden": false,
      "rnd_hidden": false,
      "market_cap_hidden": false,
      "valuation_hidden": false,
      "profit_hidden": false,
      "values_sources": ["official_filing"]
    },
    "latest_valuation_enhanced": { "id": 18274503, "year": 2024, "month": 2, "day": 15, "source": "funding", "source_round": "SERIES A", "valuation": 82500000, "valuation_min": 66000000, "valuation_max": 99000000, "valuation_currency": "USD", "market_cap": null, "market_cap_currency": "USD", "net_debt": null, "net_debt_currency": null },
    "revenues": [{ "id": 831, "name": "manufacturing", "slug": "manufacturing", "count": 451042 }],
    "share_ticker_symbol": "DAZE.MI",
    "total_funding_enhanced": { "amount": 22330000, "currency": "USD" }
  },
  "investors_and_ownership": {
    "affiliated_funds": [],
    "investors": {
      "items": [{ "uuid": "77d5bbb7-6852-422a-b31b-709be66a33a7", "name": "A11 Venture", "images": { "32x32": "https://storage.googleapis.com/.../32.png", "74x74": "https://storage.googleapis.com/.../74.png", "100x100": "https://storage.googleapis.com/.../100.png" }, "exited": false, "path": "a11_venture" }],
      "total": 14
    },
    "legal_entities": [{ "id": 536485, "registered_name": "DAZETECHNOLOGY S.R.L.", "trade_register_number": "BG441090", "trade_register_url": "https://www.registroimprese.it/", "registry_name": "Registro delle Imprese", "is_primary": true, "country": { "id": 11, "name": "Italy" } }],
    "lp_investments": [],
    "lp_investors": [],
    "ownerships": [{ "id": 1140, "name": "Venture Capital" }],
    "patents_count": 0,
    "rounds_experience": []
  },
  "locations_and_operations": {
    "closing_month": 12,
    "closing_year": 2099,
    "company_status": "operational",
    "growth_stage": "breakout stage",
    "growth_stage_manual": "breakout stage",
    "hq_locations": [{ "id": 5063717, "address": "Via Aldo Moro, Almenno San Bartolomeo, Bergamo, Lombardy, 24030, Italy", "street": "Via Aldo Moro", "street_number": "12A", "zip": "24030", "lat": 45.7365806, "lon": 9.581759, "country": { "id": 11, "name": "Italy", "slug": "italy", "lat": 41.87194, "lon": 12.56738 }, "city": { "id": 28268, "name": "Almenno San Bartolomeo", "slug": "almenno_san_bartolomeo", "lat": 45.738, "lon": 9.582251 }, "continent": { "id": 3, "name": "Europe", "slug": "europe" }, "is_headquarters": true, "is_founding_location": false, "state": { "id": 13096, "name": "Lombardy", "slug": "lombardy", "lat": 45.65, "lon": 9.773252 } }],
    "is_government": false,
    "is_non_profit": false,
    "is_from_traderegister": false,
    "launch_month": 8,
    "launch_year": 2016
  },
  "web_and_social_presence": {
    "appstore_app_id": "id1234567890",
    "career_page_url": "https://daze.eu/careers",
    "facebook_url": "https://www.facebook.com/dazetechnology",
    "linkedin_url": "https://www.linkedin.com/company/daze-eu/",
    "playmarket_app_id": "eu.daze.app",
    "twitter_url": "https://x.com/dazetech",
    "instagram_handle": "@dazetech_official"
  }
}
```

## Field reference

### Company fields (`type = "company"`)

- **record_id** *(string, optional)*: Record UUID.
- **company_name** *(string, optional)*: Company display name.
- **company_website** *(string, optional)*: Company website URL.
- **scrape_metadata.source_page_url** *(string, optional)*: Page used as source for the record.
- **scrape_metadata.seed_identifier** *(string, optional)*: Input seed identifier.
- **scrape_metadata.seed_input_type** *(string, optional)*: Seed category (for example, URL-based input).
- **scrape_metadata.seed_input_value** *(string, optional)*: Original seed value provided in input.
- **scrape_metadata.results_page_index** *(number, optional)*: Source page index in result navigation.
- **scrape_metadata.extraction_method** *(string, optional)*: Extraction mode label.
- **scrape_metadata.scraped_time** *(number, optional)*: Unix timestamp of record capture.
- **company_identity.about** *(string, optional)*: Long-form company description.
- **company_identity.about_ai_generated** *(boolean, optional)*: Indicates whether description text is AI-generated.
- **company_identity.can_edit** *(boolean, optional)*: Editability flag.
- **company_identity.uuid** *(string, optional)*: Company UUID.
- **company_identity.images.100x100** *(string, optional)*: Logo/image URL.
- **company_identity.is_ai_data** *(boolean, optional)*: AI-data indicator.
- **company_identity.is_editorial** *(boolean, optional)*: Editorial-data indicator.
- **company_identity.name** *(string, optional)*: Company name.
- **company_identity.path** *(string, optional)*: Company path slug.
- **company_identity.tagline** *(string, optional)*: Short company tagline.
- **company_identity.type** *(string, optional)*: Entity type label.
- **company_identity.website_url** *(string, optional)*: Website URL.
- **company_identity.listing_page** *(string, optional)*: Listing page URL.
- **market_and_product_profile.client_focus** *(array, optional)*: Client-focus categories.
- **market_and_product_profile.industries** *(array, optional)*: Industry classifications.
- **market_and_product_profile.sub_industries** *(array, optional)*: Sub-industry classifications.
- **market_and_product_profile.tags** *(array, optional)*: Associated tags.
- **market_and_product_profile.sdgs** *(array, optional)*: Sustainability goal tags.
- **market_and_product_profile.technologies** *(array, optional)*: Technology labels.
- **market_and_product_profile.tech_stack** *(array, optional)*: Technology stack entries.
- **market_and_product_profile.lists.items** *(array, optional)*: Public list memberships.
- **market_and_product_profile.lists.total** *(number, optional)*: Total lists count.
- **growth_and_traction.employees** *(string, optional)*: Employee band.
- **growth_and_traction.team_total** *(number, optional)*: Team size estimate.
- **growth_and_traction.job_offers_total** *(number, optional)*: Open job postings count.
- **growth_and_traction.employees_chart** *(array, optional)*: Employee trend time series.
- **growth_and_traction.similarweb_chart** *(array, optional)*: Traffic trend time series.
- **growth_and_traction.traffic.visitors** *(string, optional)*: Latest visitor estimate.
- **funding_and_financials.total_funding_enhanced.amount** *(number, optional)*: Total funding amount.
- **funding_and_financials.total_funding_enhanced.currency** *(string, optional)*: Funding currency.
- **funding_and_financials.latest_valuation_enhanced.valuation_min** *(number, optional)*: Latest valuation lower bound.
- **funding_and_financials.latest_valuation_enhanced.valuation_max** *(number, optional)*: Latest valuation upper bound.
- **funding_and_financials.latest_valuation_enhanced.valuation_currency** *(string, optional)*: Valuation currency.
- **funding_and_financials.kpi_summary.values** *(array, optional)*: KPI history entries.
- **investors_and_ownership.investors.items** *(array, optional)*: Investor entities.
- **investors_and_ownership.investors.total** *(number, optional)*: Investor count.
- **investors_and_ownership.legal_entities** *(array, optional)*: Registered legal entities.
- **investors_and_ownership.ownerships** *(array, optional)*: Ownership classifications.
- **investors_and_ownership.patents_count** *(number, optional)*: Patent count.
- **locations_and_operations.company_status** *(string, optional)*: Operating status.
- **locations_and_operations.growth_stage** *(string, optional)*: Growth stage label.
- **locations_and_operations.hq_locations** *(array, optional)*: Headquarters location objects.
- **locations_and_operations.launch_month** *(number, optional)*: Launch month.
- **locations_and_operations.launch_year** *(number, optional)*: Launch year.
- **locations_and_operations.is_government** *(boolean, optional)*: Government entity flag.
- **locations_and_operations.is_non_profit** *(boolean, optional)*: Non-profit flag.
- **web_and_social_presence.career_page_url** *(string, optional)*: Careers page URL.
- **web_and_social_presence.linkedin_url** *(string, optional)*: LinkedIn profile URL.
- **web_and_social_presence.facebook_url** *(string, optional)*: Facebook profile URL.
- **web_and_social_presence.twitter_url** *(string, optional)*: Twitter/X URL.
- **web_and_social_presence.instagram_handle** *(string, optional)*: Instagram handle.
- **web_and_social_presence.appstore_app_id** *(string, optional)*: App Store ID.
- **web_and_social_presence.playmarket_app_id** *(string, optional)*: Google Play ID.

## Data guarantees & handling

- **Best-effort extraction:** fields may vary by region/session/availability/UI experiments.
- **Optional fields:** null-check in downstream code.
- **Deduplication:** recommend `type + ":" + id`.

## How to Run on Apify

1. Open the actor in Apify Console.
2. Configure your search parameters (for example, target URLs and collection scope).
3. Set the maximum number of outputs to collect.
4. Click **Start** and wait for the run to finish.
5. Download results in JSON, CSV, Excel, or other supported formats.

## Scheduling & Automation

### Scheduling

**Automated Data Collection**
You can schedule recurring runs to keep your dataset continuously up to date. Scheduled runs are useful for monitoring changes without manual restarts.

- Navigate to **Schedules** in Apify Console
- Create a new schedule (daily, weekly, or custom cron)
- Configure input parameters
- Enable notifications for run completion
- Add webhooks for automated processing

### Integration Options

- **Webhooks:** Trigger downstream actions when a run completes
- **Zapier:** Connect to 5,000+ apps without coding
- **Make :** Build multi-step automation workflows
- **Google Sheets:** Export results to a spreadsheet
- **Slack/Discord:** Receive notifications and summaries
- **Email:** Send automated reports via email

## Performance

Estimated run times:

- **Small runs (< 1,000 outputs):** ~2–3 minutes
- **Medium runs (1,000–5,000 outputs):** ~5–15 minutes
- **Large runs (5,000+ outputs):** ~15–30 minutes

Execution time varies based on filters, result volume, and how much information is returned per record.

## Compliance & Ethics

### Responsible Data Collection

This actor collects publicly available **company and market intelligence** information from **{{TARGET_SITE}}** for legitimate business purposes, including:

- **startup ecosystem** research and market analysis
- **lead generation and enrichment**
- **competitive benchmarking and monitoring**

Users are responsible for ensuring their collection and use of data complies with applicable laws, regulations, and contractual obligations. This section is informational and not legal advice.

### Best Practices

- Use collected data in accordance with applicable laws, regulations, and the target site’s terms
- Respect individual privacy and personal information
- Use data responsibly and avoid disruptive or excessive collection
- Do not use this actor for spamming, harassment, or other harmful purposes
- Follow relevant data protection requirements where applicable (e.g., GDPR, CCPA)

## Support

If you need help, use the Issues tab or support section on the actor page. Include the input you used (redacted), run ID, expected vs actual behavior, and an optional small output sample so troubleshooting can be done quickly.