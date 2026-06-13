[Dealroom Scraper](https://apify.com/saswave/dealroom-scraper?fpr=data)

## Dealroom Company Scraper — The Most Complete Dealroom Data Extractor (No API Needed)

Effortlessly scrape Dealroom.co company profiles using only a company URL or domain name.

This Apify Actor crawls Dealroom pages at scale and returns structured, enriched data about companies, startups, investors, teams, funding rounds, tech stack, news, and market insights.

If you need a Dealroom API alternative or a way to extract startup, investor, and market intelligence data automatically, this scraper gives you full flexibility, high depth, and no API limits.

## 🔍 What This Dealroom Scraper Extracts

The scraper collects hundreds of datapoints from Dealroom, including:

## 🧩 Company Information

Company name, tagline & about section

Industry, sub-industries & SDGs

Growth stage

Location(s) & headquarters

Legal entities

Client focus

Delivery method

Company status

Related companies

Nearby companies

## 👥 Team & Talent

Key team members (name, titles, roles)

Founder & team profiles

Work experience

Education & universities

Growth & hiring pace

Team size with historical charts

## 💸 Funding, Investors & Financials

Funding rounds (Seed → Series → Late stage)

Amounts, currencies, valuation ranges

Investors & funds (corporate, VC, angels)

LP investors / LP investments

Funding history (full timeline)

Investment portfolio & investor activity

Revenue data when available

KPI summary & metrics history

## 📊 Market & Traffic Analytics

Similarweb traffic (visitors, growth, sources, top countries)

Similarweb 12-month traffic growth percentile

AppStore & Play Store app IDs

App downloads (iOS / Android)

Social analytics (Twitter/X, Facebook, Instagram)

## 📰 News & Signals

News articles mentioning the company

Press updates & funding announcements

Dealroom-generated company insights

## 🧠 AI-Generated Enrichment (optional)

AI-generated company descriptions

AI-generated insights & summaries

Keyword-rich company positioning

## 🧑‍💻 Why Use This Actor Instead of Dealroom’s API?

- No API key required
- Higher coverage than the public Dealroom API
- Scrape any company page, including hidden/enriched data
- Fully automated, scalable, and exportable

This scraper is perfect for:

Market research & competitive analysis

VC sourcing & investor intelligence

Sales prospecting & lead enrichment

Startup benchmarking & trend monitoring

Data pipelines & automated research workflows

## Output example

```
{
  "about": "Vibe.co is a digital advertising platform that specializes in streaming apps and TV channels. The company provides a user-friendly platform for businesses to advertise their products or services on over 500 apps and channels, including sports, movies, TV shows, local news, and Hispanic content. This broad range of channels allows businesses to reach a wide audience, from local communities to nationwide households, totaling up to 120 million households.\n\nThe company's primary clients are small to medium-sized businesses that are looking to increase their visibility and reach their target audience more effectively. Vibe.co's platform allows these businesses to target viewers based on socio-demographic characteristics, interests, and intent-to-buy, ensuring that their ads are shown to the audiences who are most likely to be interested in their products or services.\n\nVibe.co operates in the digital advertising market, which has seen significant growth with the rise of streaming services. The company's business model is based on a cost-per-view system, meaning businesses only pay when their ad is viewed. This model, combined with the ability to target specific audiences, can lead to a higher return on investment for advertisers.\n\nIn terms of revenue generation, Vibe.co makes money by charging businesses for the ads they run on the platform. The cost is determined by the number of views the ad receives, which is known as 'cost per view'. This model ensures that businesses only pay for ads that are actually viewed, making it a cost-effective advertising solution.\n\nKeywords: Digital Advertising, Streaming Apps, TV Channels, Targeted Advertising, Cost-Per-View, Small to Medium Businesses, User-Friendly Platform, Socio-Demographic Targeting, Local and Nationwide Reach, Digital Advertising Market.",
  "about_ai_generated": true,
  "affiliated_funds": [],
  "appstore_app_id": null,
  "can_edit": false,
  "career_page_url": null,
  "client_focus": [
    {
      "name": "business",
      "count": 1149337
    }
  ],
  "closing_month": null,
  "closing_year": null,
  "company_status": "operational",
  "corporate_industries": [],
  "country_experience": [
    {
      "name": "United States",
      "count": 1
    }
  ],
  "current_and_prev_year_fundings_num": 0,
  "delivery_method": null,
  "employees_chart": [
    {
      "date": "2022-10-25",
      "value": 1
    },
    {
      "date": "2022-11-24",
      "value": 1.1
    },
    // truncated for example
  ],
  "employees_latest": null,
  "employee_12_months_growth_percentile": "top 5%",
  "employee_12_months_growth_unique": 4080,
  "similarweb_12_months_growth_percentile": "top 25%",
  "similarweb_12_months_growth_unique": 98614,
  "employees": "51-200",
  "entity_sub_types": [],
  "exits_higher_800m": {
    "items": [],
    "total": 0
  },
  "facebook_url": null,
  "fundings_investor": {
    "items": [
      {
        "id": 884173,
        "year": 2021,
        "month": 4,
        "amount": null,
        "amount_source": 0,
        "currency": "KRW",
        "round": "EARLY VC",
        "investors": [
          {
            "uuid": "ee8da1a4-2085-4519-99f2-5d28b2c1ac37",
            "name": "Vibe",
            "entity_type": "organization",
            "labels": [
              "company",
              "investor"
            ],
            "path": "vibe_1_5",
            "type": "corporate",
            "images": {
              "32x32": "https://storage.googleapis.com/dealroom-images-production/c1/MzI6MzI6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNS8wMS8wMy83N2I0ZDgxYTVhMDAwZTFiODI3MDkxM2YwN2Y4MjQ5Mg==.png",
              "74x74": "https://storage.googleapis.com/dealroom-images-production/12/NzQ6NzQ6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNS8wMS8wMy83N2I0ZDgxYTVhMDAwZTFiODI3MDkxM2YwN2Y4MjQ5Mg==.png",
              "100x100": "https://storage.googleapis.com/dealroom-images-production/88/MTAwOjEwMDpjb21wYW55QHMzLWV1LXdlc3QtMS5hbWF6b25hd3MuY29tL2RlYWxyb29tLWltYWdlcy8yMDI1LzAxLzAzLzc3YjRkODFhNWEwMDBlMWI4MjcwOTEzZjA3ZjgyNDky.png"
            },
            "lead": false
          }
        ],
        "company": {
          "uuid": "98ad0528-059f-419f-a764-4f294ff1ec33",
          "name": "Sears Labs",
          "entity_type": "organization",
          "labels": [
            "company"
          ],
          "path": "seerslab",
          "type": "company"
        },
        "unknown_investors": [],
        "is_undisclosed": false,
        "news_source": "https://wowtale.net/2021/04/08/24465/",
        "valuation": null,
        "valuation_generated_min": null,
        "valuation_generated_max": null,
        "transaction_multiples": {
          "ev_ltm_revenue_multiple": null,
          "ev_ltm_ebitda_multiple": null,
          "ev_ltm_profit_multiple": null,
          "ev_ntm_revenue_multiple": null,
          "ev_ntm_ebitda_multiple": null,
          "ev_ntm_profit_multiple": null
        }
      }
    ],
    "total": 1
  },
  "growth_stage": "late growth",
  "hq_locations": [
    {
      "id": 3905240,
      "address": "Chicago, Cook County, Illinois, United States",
      "street": "",
      "street_number": "",
      "zip": "",
      "lat": 41.8755616,
      "lon": -87.6244212,
      "country": {
        "id": 23,
        "name": "United States",
        "lat": 40.730137,
        "lon": -73.990129
      },
      "city": {
        "id": 104717,
        "name": "Chicago",
        "lat": 1,
        "lon": -87.629457
      },
      "continent": {
        "id": 8,
        "name": "North America"
      },
      "is_headquarters": true,
      "is_founding_location": false,
      "state": {
        "id": 18673,
        "name": "Illinois",
        "lat": 1,
        "lon": -89.433729
      }
    }
  ],
  "uuid": "ee8da1a4-2085-4519-99f2-5d28b2c1ac37",
  "images": {
    "100x100": "https://storage.googleapis.com/dealroom-images-production/88/MTAwOjEwMDpjb21wYW55QHMzLWV1LXdlc3QtMS5hbWF6b25hd3MuY29tL2RlYWxyb29tLWltYWdlcy8yMDI1LzAxLzAzLzc3YjRkODFhNWEwMDBlMWI4MjcwOTEzZjA3ZjgyNDky.png"
  },
  "income_streams": [
    {
      "id": 3,
      "name": "subscription",
      "count": 705009
    }
  ],
  "industries": [
    {
      "id": 100129,
      "name": "marketing",
      "count": 136401
    }
  ],
  "industry_experience": [
    {
      "id": 100012,
      "name": "Media",
      "count": 1
    },
    {
      "id": 100016,
      "name": "Dating",
      "count": 1
    }
  ],
  "innovations_count": 0,
  "investments_higher_800m": {
    "items": [],
    "total": 0
  },
  "investments_num": 1,
  "investments": [
    {
      "uuid": "98ad0528-059f-419f-a764-4f294ff1ec33",
      "name": "Sears Labs",
      "entity_type": "organization",
      "labels": [
        "company"
      ],
      "type": "company",
      "path": "seerslab",
      "images": {
        "32x32": "https://storage.googleapis.com/dealroom-images-production/f6/MzI6MzI6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNS8wMS8wMi84ZGYwNjQ0MWJjODg1NmZjYjZiZDUyNmEyNGRhNmJiMA==.png",
        "74x74": "https://storage.googleapis.com/dealroom-images-production/e9/NzQ6NzQ6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNS8wMS8wMi84ZGYwNjQ0MWJjODg1NmZjYjZiZDUyNmEyNGRhNmJiMA==.png",
        "100x100": "https://storage.googleapis.com/dealroom-images-production/fd/MTAwOjEwMDpjb21wYW55QHMzLWV1LXdlc3QtMS5hbWF6b25hd3MuY29tL2RlYWxyb29tLWltYWdlcy8yMDI1LzAxLzAyLzhkZjA2NDQxYmM4ODU2ZmNiNmJkNTI2YTI0ZGE2YmIw.png"
      },
      "tagline": "Media tech company to bring hollywood into your everyday life with lollicam",
      "hq_locations": [
        {
          "id": 137706,
          "address": "Palo Alto, United States",
          "street": "",
          "street_number": "",
          "zip": "",
          "lat": 37.441883,
          "lon": -122.143019,
          "country": {
            "id": 23,
            "name": "United States",
            "lat": 40.730137,
            "lon": -73.990129
          },
          "city": {
            "id": 45013,
            "name": "Palo Alto",
            "lat": 1,
            "lon": -122.159847
          },
          "continent": {
            "id": 8,
            "name": "North America"
          },
          "is_headquarters": true,
          "is_founding_location": false,
          "state": {
            "id": 11126,
            "name": "California",
            "lat": 36.778261,
            "lon": -119.4179324
          }
        }
      ],
      "revenues": [],
      "employees": "2-10",
      "traffic_summary": "0.8K",
      "traffic": {
        "visitors": "730",
        "annual_growth": -51.33333333333333,
        "sources": [],
        "top_countries": []
      },
      "total_funding": 8.53,
      "total_funding_enhanced": {
        "amount": 9378049,
        "currency": "USD"
      },
      "exited": false,
      "lead": false,
      "industries": [
        {
          "id": 100012,
          "name": "media"
        },
        {
          "id": 100016,
          "name": "dating"
        }
      ],
      "corporate_industries": [],
      "service_industries": [],
      "growth_stage": "seed",
      "is_editorial": true,
      "is_acquired": false,
      "is_ipo": false,
      "ipo_round": null,
      "acquisition_round": null,
      "is_verified": true,
      "latest_valuation": {
        "id": 13763948,
        "year": 2016,
        "month": 6,
        "day": null,
        "source": "funding",
        "source_round": "SEED",
        "valuation": null,
        "valuation_min": 8000000,
        "valuation_max": 12000000,
        "valuation_currency": "USD",
        "market_cap": null,
        "market_cap_currency": null,
        "net_debt": null,
        "net_debt_currency": null
      },
      "latest_valuation_enhanced": {
        "id": 13763948,
        "year": 2016,
        "month": 6,
        "day": null,
        "source": "funding",
        "source_round": "SEED",
        "valuation": null,
        "valuation_min": 8000000,
        "valuation_max": 12000000,
        "valuation_currency": "USD",
        "market_cap": null,
        "market_cap_currency": "USD",
        "net_debt": null,
        "net_debt_currency": null
      },
      "last_funding_round": {
        "id": 734969,
        "year": 2022,
        "month": 10,
        "amount": 8800,
        "currency": "KRW",
        "round": "SERIES B",
        "valuation": null,
        "valuation_generated_min": 35200000000,
        "valuation_generated_max": 52800000000
      },
      "kpi_summary": {
        "id": 114609,
        "last_update_date": "2024-01-04T09:48:07+00:00",
        "currency": null,
        "share_price_chart": [],
        "share_price_currency": null,
        "values": [],
        "valuations": [
          {
            "id": 13763948,
            "year": 2016,
            "month": 6,
            "day": null,
            "source": "funding",
            "source_round": "SEED",
            "valuation": null,
            "valuation_min": 8000000,
            "valuation_max": 12000000,
            "valuation_currency": "USD",
            "market_cap": null,
            "market_cap_currency": null,
            "net_debt": null,
            "net_debt_currency": null
          },
          {
            "id": 9189975,
            "year": 2022,
            "month": 10,
            "day": null,
            "source": "funding",
            "source_round": "SERIES B",
            "valuation": null,
            "valuation_min": 35200000000,
            "valuation_max": 52800000000,
            "valuation_currency": "KRW",
            "market_cap": null,
            "market_cap_currency": null,
            "net_debt": null,
            "net_debt_currency": null
          }
        ],
        "revenues_hidden": false,
        "ebitda_hidden": false,
        "rnd_hidden": false,
        "market_cap_hidden": false,
        "valuation_hidden": false,
        "profit_hidden": false,
        "values_sources": []
      },
      "affiliate": null
    }
  ],
  "investor_exits_funding_enhanced": {
    "amount": 0,
    "currency": "USD"
  },
  "investor_exits_num": 0,
  "investor_total_rank": null,
  "investor_total": null,
  "investors": {
    "items": [
      {
        "uuid": "64db6521-1409-4b14-839c-94f11fd10236",
        "name": "Elaia Partners",
        "images": {
          "32x32": "https://storage.googleapis.com/dealroom-images-production/cb/MzI6MzI6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAxOS8wNy8xMS84MjkxNTlhZTQ3MGQyOThlMTNmY2Y5OWFhNTE4ODM1Nw==.jpg",
          "74x74": "https://storage.googleapis.com/dealroom-images-production/db/NzQ6NzQ6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAxOS8wNy8xMS84MjkxNTlhZTQ3MGQyOThlMTNmY2Y5OWFhNTE4ODM1Nw==.jpg",
          "100x100": "https://storage.googleapis.com/dealroom-images-production/4b/MTAwOjEwMDpjb21wYW55QHMzLWV1LXdlc3QtMS5hbWF6b25hd3MuY29tL2RlYWxyb29tLWltYWdlcy8yMDE5LzA3LzExLzgyOTE1OWFlNDcwZDI5OGUxM2ZjZjk5YWE1MTg4MzU3.jpg"
        },
        "exited": false,
        "path": "elaia_partners"
      },
      // truncated for example
    ],
    "total": 12
  },
  "is_ai_data": true,
  "is_editorial": false,
  "is_government": false,
  "is_non_profit": false,
  "is_from_traderegister": false,
  "job_offers_total": 0,
  "kpi_summary": {
    "id": 3336385,
    "last_update_date": "2024-10-03T14:20:53+01:00",
    "currency": "USD",
    "share_price_chart": [],
    "share_price_currency": "USD",
    "values": [
      {
        "year": 2022,
        "valuation": null,
        "valuation_source": null,
        "revenue": 2400000,
        "revenue_growth": null,
        "revenue_source": 1,
        "ebitda": null,
        "ebitda_margin": null,
        "ebitda_source": null,
        "profit": null,
        "profit_margin": null,
        "profit_source": null,
        "rnd": null,
        "rnd_margin": null,
        "rnd_source": null,
        "ev_revenue": null,
        "ev_ebitda": null
      },
      {
        "year": 2023,
        "valuation": null,
        "valuation_source": null,
        "revenue": 3700000,
        "revenue_growth": 54,
        "revenue_source": 1,
        "ebitda": null,
        "ebitda_margin": null,
        "ebitda_source": null,
        "profit": null,
        "profit_margin": null,
        "profit_source": null,
        "rnd": null,
        "rnd_margin": null,
        "rnd_source": null,
        "ev_revenue": null,
        "ev_ebitda": null
      }
    ],
    "valuations": [
      {
        "id": 6557148,
        "year": 2022,
        "month": 9,
        "day": null,
        "source": "funding",
        "source_round": "SEED",
        "valuation": null,
        "valuation_min": 25600000,
        "valuation_max": 38400000,
        "valuation_currency": "USD",
        "market_cap": null,
        "market_cap_currency": null,
        "net_debt": null,
        "net_debt_currency": null
      },
      {
        "id": 18276992,
        "year": 2024,
        "month": 2,
        "day": null,
        "source": "funding",
        "source_round": "SERIES A",
        "valuation": null,
        "valuation_min": 90000000,
        "valuation_max": 135000000,
        "valuation_currency": "USD",
        "market_cap": null,
        "market_cap_currency": null,
        "net_debt": null,
        "net_debt_currency": null
      }
    ],
    "revenues_hidden": false,
    "ebitda_hidden": false,
    "rnd_hidden": false,
    "market_cap_hidden": false,
    "valuation_hidden": false,
    "profit_hidden": false,
    "values_sources": []
  },
  "landscapes": [
    {
      "id": 8269,
      "name": "Doctolib",
      "count": 10,
      "list": {
        "id": 17638,
        "title": "The European Startup Mafias"
      }
    }
  ],
  "latest_valuation_enhanced": {
    "id": 18276992,
    "year": 2024,
    "month": 2,
    "day": null,
    "source": "funding",
    "source_round": "SERIES A",
    "valuation": null,
    "valuation_min": 90000000,
    "valuation_max": 135000000,
    "valuation_currency": "USD",
    "market_cap": null,
    "market_cap_currency": "USD",
    "net_debt": null,
    "net_debt_currency": null
  },
  "launch_month": 1,
  "launch_year": 2021,
  "legal_entities": [],
  "linkedin_url": "https://www.linkedin.com/company/vibe-ctv-ott/",
  "lists_ids": [],
  "lists": {
    "items": [
      {
        "id": 17638,
        "title": "The European Startup Mafias",
        "type": 1,
        "is_public": true,
        "created": "2020-10-23T02:29:21+01:00"
      }
    ],
    "total": 1
  },
  "lp_investments": [],
  "lp_investors": [],
  "name": "Vibe",
  "ownerships": [
    {
      "id": 1137,
      "name": "Angel"
    },
    {
      "id": 1140,
      "name": "Venture Capital"
    }
  ],
  "patents_count": 0,
  "path": "vibe_1_5",
  "playmarket_app_id": null,
  "revenues": [
    {
      "id": 836,
      "name": "saas",
      "count": 457206
    }
  ],
  "rounds_experience": [
    {
      "name": "EARLY VC",
      "count": 1
    }
  ],
  "sdgs": [],
  "service_industries": [],
  "share_ticker_symbol": null,
  "similarweb_chart": [
    {
      "date": "2022-10-01",
      "value": 5700
    },
    {
      "date": "2022-11-01",
      "value": 9300
    },
    // truncated for example
  ],
  "similarweb_hidden": false,
  "sub_industries": [
    {
      "id": 72,
      "name": "adtech",
      "count": 9121
    }
  ],
  "tagline": "Advertises brand on CTV and OTT content with Vibe's self-serve ad platform",
  "tags": [],
  "team_total": 7,
  "tech_stack": [],
  "technologies": [],
  "total_funding_enhanced": {
    "amount": 28900000,
    "currency": "USD"
  },
  "traffic": {
    "visitors": "170000",
    "sources": [],
    "top_countries": []
  },
  "twitter_url": "https://twitter.com/vibe_ads",
  "instagram_handle": null,
  "type": "corporate",
  "website_url": "http://vibe.co",
  "analytics": {
    "facebook_likes_chart": [],
    "twitter_tweets_chart": [
      {
        "date": "2022-03-05",
        "value": 1
      },
      {
        "date": "2022-04-08",
        "value": 1
      },
      // truncated for example
    ],
    "twitter_followers_chart": [
      {
        "date": "2022-03-05",
        "value": 4
      },
      {
        "date": "2022-04-08",
        "value": 4
      },
      // truncated for example
    ],
    "twitter_favorites_chart": [
      {
        "date": "2022-03-05",
        "value": 7
      },
      {
        "date": "2022-04-08",
        "value": 7
      },
      // truncated for example
    ],
    "instagram_followers_chart": [],
    "instagram_posts_chart": [],
    "similarweb_chart": [
      {
        "date": "2022-10-01",
        "value": 5700
      },
      {
        "date": "2022-11-01",
        "value": 9300
      },
      // truncated for example
    ],
    "employee_12_months_growth_delta_chart": [
      {
        "date": "2023-10-02",
        "value": 0
      },
      {
        "date": "2023-10-05",
        "value": -330
      },
      // truncated for example
    ],
    "app_downloads_ios_incremental_chart": [],
    "app_downloads_android_incremental_chart": [],
    "employees_chart": [
      {
        "date": "2022-10-25",
        "value": 1
      },
      {
        "date": "2022-11-24",
        "value": 1.1
      },
      // truncated for example
    ],
    "traffic": {
      "traffic": "170K",
      "growth": 2882.456140350877,
      "growth_yearly": 385.7142857142857,
      "visitors": "170000",
      "rank": "25",
      "sources": [],
      "top_countries": [],
      "date": "12/2024",
      "domain": "vibe.co"
    },
    "growth_stage": "late",
    "kpi_summary": {
      "id": 3336385,
      "last_update_date": "2024-10-03T14:20:53+01:00",
      "currency": "USD",
      "share_price_chart": [],
      "share_price_currency": "USD",
      "values": [
        {
          "year": 2022,
          "valuation": null,
          "valuation_source": null,
          "revenue": 2400000,
          "revenue_growth": null,
          "revenue_source": 1,
          "ebitda": null,
          "ebitda_margin": null,
          "ebitda_source": null,
          "profit": null,
          "profit_margin": null,
          "profit_source": null,
          "rnd": null,
          "rnd_margin": null,
          "rnd_source": null,
          "ev_revenue": null,
          "ev_ebitda": null
        },
        {
          "year": 2023,
          "valuation": null,
          "valuation_source": null,
          "revenue": 3700000,
          "revenue_growth": 54,
          "revenue_source": 1,
          "ebitda": null,
          "ebitda_margin": null,
          "ebitda_source": null,
          "profit": null,
          "profit_margin": null,
          "profit_source": null,
          "rnd": null,
          "rnd_margin": null,
          "rnd_source": null,
          "ev_revenue": null,
          "ev_ebitda": null
        }
      ],
      "valuations": [
        {
          "id": 6557148,
          "year": 2022,
          "month": 9,
          "day": null,
          "source": "funding",
          "source_round": "SEED",
          "valuation": null,
          "valuation_min": 25600000,
          "valuation_max": 38400000,
          "valuation_currency": "USD",
          "market_cap": null,
          "market_cap_currency": null,
          "net_debt": null,
          "net_debt_currency": null
        },
        {
          "id": 18276992,
          "year": 2024,
          "month": 2,
          "day": null,
          "source": "funding",
          "source_round": "SERIES A",
          "valuation": null,
          "valuation_min": 90000000,
          "valuation_max": 135000000,
          "valuation_currency": "USD",
          "market_cap": null,
          "market_cap_currency": null,
          "net_debt": null,
          "net_debt_currency": null
        }
      ],
      "revenues_hidden": false,
      "ebitda_hidden": false,
      "rnd_hidden": false,
      "market_cap_hidden": false,
      "valuation_hidden": false,
      "profit_hidden": false,
      "values_sources": []
    },
    "similarweb_hidden": false
  },
  "team": [
    {
      "uuid": "0170cba8-0ea7-4a5f-a201-49025666f196",
      "name": "Franck Tetzlaff",
      "entity_type": "person",
      "labels": [
        "angel investor"
      ],
      "type": "investor",
      "path": "franck_tetzlaff",
      "twitter_url": null,
      "linkedin_url": "https://www.linkedin.com/in/tetzlaff/",
      "angellist_url": null,
      "is_editorial": false,
      "gender": "male",
      "images": {
        "32x32": "https://storage.googleapis.com/dealroom-images-production/e5/MzI6MzI6dXNlckBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNC8xMS8yNS8zNDM0Y2I2OTIwMTNmZjFiOTM5MjA0NjJlYzcyMmY0Mw==.png",
        "74x74": "https://storage.googleapis.com/dealroom-images-production/d0/NzQ6NzQ6dXNlckBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNC8xMS8yNS8zNDM0Y2I2OTIwMTNmZjFiOTM5MjA0NjJlYzcyMmY0Mw==.png",
        "100x100": "https://storage.googleapis.com/dealroom-images-production/1e/MTAwOjEwMDp1c2VyQHMzLWV1LXdlc3QtMS5hbWF6b25hd3MuY29tL2RlYWxyb29tLWltYWdlcy8yMDI0LzExLzI1LzM0MzRjYjY5MjAxM2ZmMWI5MzkyMDQ2MmVjNzIyZjQz.png"
      },
      "titles": [
        {
          "id": 10,
          "name": "CTO"
        },
        {
          "id": 15,
          "name": "Co-Founder"
        },
        {
          "id": 146413,
          "name": "Founder"
        }
      ],
      "approved": true,
      "has_email": true,
      "signup_date": "2020-09-08T15:16:34+01:00",
      "is_founder": true,
      "is_serial_founder": true,
      "year_start": 2021,
      "month_start": 1,
      "year_end": null,
      "month_end": null,
      "companies": [
        {
          "uuid": "c626ed38-6d25-4332-935d-346ae4079ec8",
          "name": "Societe Generale",
          "entity_type": "organization",
          "labels": [
            "company",
            "investor"
          ],
          "type": "corporate",
          "path": "societe_generale",
          "images": {
            "32x32": "https://storage.googleapis.com/dealroom-images-production/bb/MzI6MzI6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyMS8xMi8xNi8yN2UxYWQzMTFkNzUxMjY2NjQ5MjliOGViMDYyMGRhMQ==.png",
            "74x74": "https://storage.googleapis.com/dealroom-images-production/89/NzQ6NzQ6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyMS8xMi8xNi8yN2UxYWQzMTFkNzUxMjY2NjQ5MjliOGViMDYyMGRhMQ==.png",
            "100x100": "https://storage.googleapis.com/dealroom-images-production/16/MTAwOjEwMDpjb21wYW55QHMzLWV1LXdlc3QtMS5hbWF6b25hd3MuY29tL2RlYWxyb29tLWltYWdlcy8yMDIxLzEyLzE2LzI3ZTFhZDMxMWQ3NTEyNjY2NDkyOWI4ZWIwNjIwZGEx.png"
          },
          "titles": [
            {
              "id": 894,
              "name": "R&D"
            }
          ],
          "past": true,
          "total_funding": 0,
          "total_funding_enhanced": {
            "amount": 0,
            "currency": "USD"
          },
          "industries": [
            {
              "id": 1264,
              "name": "fintech"
            }
          ],
          "tagline": "French financial institution covering international retail banking along with global banking and investor solutions",
          "is_founder": false
        },
        // truncated for example
      ],
      "universities": [
        {
          "id": 153023,
          "degree": {
            "id": 3,
            "name": "Msc",
            "years": 5
          },
          "majors": [],
          "year_start": 2000,
          "year_end": 2005,
          "university": {
            "uuid": "2fba0601-f1b4-4aa6-a4ee-6bbd910e64f6",
            "name": "EPITA",
            "entity_type": "organization",
            "labels": [
              "university"
            ],
            "path": "epita",
            "type": "university",
            "images": {
              "32x32": "https://storage.googleapis.com/dealroom-images-production/ca/MzI6MzI6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNC8wMi8yOS81NjU0OGQzZmRjODkzN2NlYjdiYmQzNGE1NTIxNjQwYg==.jpg",
              "74x74": "https://storage.googleapis.com/dealroom-images-production/d6/NzQ6NzQ6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNC8wMi8yOS81NjU0OGQzZmRjODkzN2NlYjdiYmQzNGE1NTIxNjQwYg==.jpg",
              "100x100": "https://storage.googleapis.com/dealroom-images-production/be/MTAwOjEwMDpjb21wYW55QHMzLWV1LXdlc3QtMS5hbWF6b25hd3MuY29tL2RlYWxyb29tLWltYWdlcy8yMDI0LzAyLzI5LzU2NTQ4ZDNmZGM4OTM3Y2ViN2JiZDM0YTU1MjE2NDBi.jpg"
            }
          }
        },
        // truncated for example
      ],
      "premium": {
        "premium": false,
        "premium_started_at": null,
        "trial": false,
        "trial_used": false,
        "trial_used_at": null,
        "trial_expired_at": null,
        "until": null
      },
      "founder_score": 94,
      "is_strong_founder": false,
      "is_super_founder": true
    },
    // truncated for example
  ],
  "rankings": {
    "bobject_id": 3538559,
    "rank": 675,
    "score": 92.26,
    "rating": 92,
    "completeness": 80,
    "hiring_pace": 0,
    "team_strength": 98.05,
    "growth_rate": 98.74,
    "timing": 100,
    "employees_to_funding": 0.47,
    "change_yesterday": -7,
    "change_last_week": -12,
    "runners_up_rank": 745118
  },
  "fundings": [
    {
      "id": 914874,
      "year": 2024,
      "month": 2,
      "amount": 22.5,
      "amount_source": 22500000,
      "currency": "USD",
      "round": "SERIES A",
      "standardised_round_label": "SERIES A",
      "valuation": null,
      "valuation_generated_min": 90000000,
      "valuation_generated_max": 135000000,
      "news_source": "https://www.vibe.co/blog/vibe-co-raises-22-5m-to-become-go-to-streaming-tv-ad-platform-for-smbs",
      "investors": [
        {
          "uuid": "64db6521-1409-4b14-839c-94f11fd10236",
          "name": "Elaia Partners",
          "entity_type": "organization",
          "labels": [
            "investor"
          ],
          "type": "fund",
          "path": "elaia_partners",
          "lead": false
        },
        // truncated for example
      ],
      "unknown_investors": [],
      "is_verified": true,
      "transaction_multiples": {
        "ev_ltm_revenue_multiple": null,
        "ev_ltm_ebitda_multiple": null,
        "ev_ltm_profit_multiple": null,
        "ev_ntm_revenue_multiple": null,
        "ev_ntm_ebitda_multiple": null,
        "ev_ntm_profit_multiple": null
      }
    },
    // truncated for example
  ],
  "news": [
    {
      "id": 9265349,
      "title": "Actionable Lève 2 Millions D’Euros Pour Son Outil D’Analyse De La Satisfaction Client",
      "pub_date": "2024-09-10T03:56:07+00:00",
      "summary": "Nans Thomas et Nicolas Rieul, fondateurs d'ACTIONABLEActionable, une startup spécialisée dans l’analyse prédictive de la satisfaction client, annonce une levée de fonds de 2 millions d’euros en pré-amorçage, seulement cinq mois après son lancement en avril 2024. Ce tour de table, réalisé en augmentation de capital et en endettement, permettra à l’entreprise de développer son intelligence artificielle destinée à prédire la satisfaction des clients et à identifier ses facteurs clés. Le financement a été mené par Axeleo, représenté par Éric Burdier. Axeleo vient elle-même de boucler son nouveau fonds de 73 millions d’euros, AXC2, spécialisé dans les startups Tech B2B. Aux côtés d’Axeleo, le micro-fonds early-stage Source Ventures et plus de 30 business angels ont participé à cette levée, parmi lesquels Stéphane Distinguin (Fondateur de Fabernovel), Mathieu Azorin (CEO et Co-Fondateur de Storetail) et Arthur Querou (CEO et Co-Fondateur de Vibe.co). Fondée par Nans Thomas et Nicolas Rieul, Actionable a pour mission de révolutionner l’analyse de la satisfaction client grâce à l’IA",
      "content": "Nans Thomas et Nicolas Rieul, fondateurs d'ACTIONABLEActionable, une startup spécialisée dans l’analyse prédictive de la satisfaction client, annonce une levée de fonds de 2 millions d’euros en pré-amorçage, seulement cinq mois après son lancement en avril 2024. Ce tour de table, réalisé en augmentation de capital et en endettement, permettra à l’entreprise de développer son intelligence artificielle destinée à prédire la satisfaction des clients et à identifier ses facteurs clés.\nLe financement a été mené par Axeleo, représenté par Éric Burdier. Axeleo vient elle-même de boucler son nouveau fonds de 73 millions d’euros, AXC2, spécialisé dans les startups Tech B2B. Aux côtés d’Axeleo, le micro-fonds early-stage Source Ventures et plus de 30 business angels ont participé à cette levée, parmi lesquels Stéphane Distinguin (Fondateur de Fabernovel), Mathieu Azorin (CEO et Co-Fondateur de Storetail) et Arthur Querou (CEO et Co-Fondateur de Vibe.co).\nFondée par Nans Thomas et Nicolas Rieul, Actionable a pour mission de révolutionner l’analyse de la satisfaction client grâce à l’IA. Sa plateforme offre des analyses en temps réel et des insights actionnables en utilisant les données collectées tout au long du parcours client. Cette approche innovante permet aux entreprises de prédire et d’améliorer la satisfaction de l’ensemble de leur base clients, améliorant ainsi la rétention et réduisant le churn.\nPour en parler plus en détail nous recevons dans notre podcast FRENCHWEB BUSINESS les deux co fondateurs d’ACTIONABLE:« Nous construisons l’IA la plus avancée au monde dans le domaine de l’expérience client. Ce financement nous permet de recruter les meilleurs experts en la matière; nous comptons déjà deux docteurs en machine learning et mathématiques dans l’équipe », a déclaré Nans Thomas, Co-Fondateur et Co-CEO d’Actionable. Nicolas Rieul, Co-Fondateur et Co-CEO, ajoute : « Ce tour de table est une étape importante pour Actionable. Il nous permet de mettre les moyens nécessaires pour satisfaire nos premiers bêta-testeurs et ainsi construire en conditions réelles la meilleure plateforme d’expérience client prédictive. »\nDéjà six entreprises de secteurs et de tailles variés ont été séduites par la proposition de valeur d’Actionable et participent à la phase de bêta-test :Mirakl, la licorne française SaaS spécialiste du e-commerce avec 8,6 milliards d’euros de volume d’affaires. Philippe Corrot, Co-fondateur et Co-CEO de Mirakl, déclare : « L’IA révolutionne tous les domaines; son application à l’amélioration de l’expérience client est très prometteuse. Nous sommes ravis de mettre cette technologie au service de la satisfaction de nos clients et partenaires e-commerçants et sellers. »\nOuigo, la société ferroviaire low-cost de la SNCF ayant transporté 110 millions de voyageurs en 10 ans. Maxime Legrand, Directeur Marque et Expérience Client, explique : « Chez Ouigo, nous mettons un point d’honneur à satisfaire nos clients en proposant des prix attractifs mais également en travaillant sur l’amélioration continue de la qualité des services. Grâce à Actionable, nous souhaitons utiliser l’IA pour mieux comprendre les besoins de nos clients et offrir une expérience personnalisée à chacun. »\nAudiens, le groupe de protection sociale des professionnels de la création et de l’information, accompagnant plus de 45 000 entreprises et couvrant près de 1 million de personnes. Marie-Christine Dall’Osto, Directrice de la Transformation, de l’Expérience Client et du Marketing, affirme : « Nos clients satisfaits sont nos meilleurs ambassadeurs. Avec l’IA d’Actionable, nous irons plus loin dans l’anticipation de leurs attentes pour renforcer notre engagement à accompagner chacun de manière proactive et humaine. »\nUnited Heroes, l’application d’engagement collaborateurs avec 500 000 utilisateurs en entreprise. Paul-Emile Saab, CEO de United Heroes, souligne : « Nous offrons aux grandes entreprises une plateforme bien-être pour leurs collaborateurs et devons garantir la satisfaction des salariés tout en restant attentifs aux enjeux des décideurs. Actionable est le seul acteur capable de gérer ces deux niveaux de complexité. »\nTicketac, le site de billetterie en ligne avec plus de 1 million de clients annuels. Morgane Thieblemont, Chief Marketing  Product Officer, indique : « La fidélisation de nos clients est un enjeu clé pour Ticketac. Actionable nous aide à identifier et suivre les principaux moteurs de satisfaction afin de maintenir un haut niveau de service. »\nStrapi, la startup Headless CMS ayant levé 45 millions de dollars et comptant la NASA, Toyota, Walmart ou IBM parmi ses clients. Aurélien Georget, CPO  Co-Fondateur de Strapi, déclare : « Actionable est une aide précieuse à la prise de décisions stratégiques. Les insights générés nous permettent de prioriser nos initiatives sur ce qui aura le plus d’impact en termes de satisfaction client, de rétention ou d’expansion de revenus. Notre équipe Customer Success l’utilise également pour contacter proactivement chaque client dès qu’un signal faible est détecté. »\n                         Pour nous contacter, nous vous avons préparé un petit formulaire pour bien gérer votre demande et pouvoir l'adresser en toute confidentialité. Cliquez ici pour y accéder Les derniers articles par LA REDACTION DE FRENCHWEB.FR (tout voir)",
      "link": "https://www.frenchweb.fr/actionable-leve-2-millions-deuros-pour-son-outil-danalyse-de-la-satisfaction-client/449019",
      "image": "https://www.frenchweb.fr/wp-content/uploads/2024/09/actionable-fondateurs.png",
      "feed": {
        "id": 145,
        "name": "FrenchWeb",
        "link": "https://www.frenchweb.fr/feed"
      },
      "author": null,
      "keyword": {
        "id": "3",
        "name": "French"
      },
      "is_ai_summarised": false,
      "company_summary": null,
      "news_type": null,
      "categories": [],
      "related_companies": [
        {
          "uuid": "ee8da1a4-2085-4519-99f2-5d28b2c1ac37",
          "name": "Vibe",
          "entity_type": "organization",
          "labels": [
            "company",
            "investor"
          ],
          "path": "vibe_1_5",
          "type": "corporate",
          "images": {
            "32x32": "https://storage.googleapis.com/dealroom-images-production/c1/MzI6MzI6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNS8wMS8wMy83N2I0ZDgxYTVhMDAwZTFiODI3MDkxM2YwN2Y4MjQ5Mg==.png",
            "74x74": "https://storage.googleapis.com/dealroom-images-production/12/NzQ6NzQ6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNS8wMS8wMy83N2I0ZDgxYTVhMDAwZTFiODI3MDkxM2YwN2Y4MjQ5Mg==.png",
            "100x100": "https://storage.googleapis.com/dealroom-images-production/88/MTAwOjEwMDpjb21wYW55QHMzLWV1LXdlc3QtMS5hbWF6b25hd3MuY29tL2RlYWxyb29tLWltYWdlcy8yMDI1LzAxLzAzLzc3YjRkODFhNWEwMDBlMWI4MjcwOTEzZjA3ZjgyNDky.png"
          },
          "industries": [
            {
              "id": 100129,
              "name": "marketing"
            }
          ],
          "hq_locations": [
            {
              "id": 3905240,
              "address": "Chicago, Cook County, Illinois, United States",
              "street": "",
              "street_number": "",
              "zip": "",
              "lat": 41.8755616,
              "lon": -87.6244212,
              "country": {
                "id": 23,
                "name": "United States",
                "lat": 40.730137,
                "lon": -73.990129
              },
              "city": {
                "id": 104717,
                "name": "Chicago",
                "lat": 1,
                "lon": -87.629457
              },
              "continent": {
                "id": 8,
                "name": "North America"
              },
              "is_headquarters": true,
              "is_founding_location": false,
              "state": {
                "id": 18673,
                "name": "Illinois",
                "lat": 1,
                "lon": -89.433729
              }
            }
          ]
        }
      ],
      "funding_round": null
    },
    // truncated for example
  ],
  "related": [
    {
      "id": 17638,
      "title": "The European Startup Mafias",
      "summary": "Europe's startup founder factories",
      "type": 1,
      "is_public": true,
      "created": "2020-10-23T02:29:21+01:00",
      "landscape": {
        "id": 8269,
        "name": "Doctolib"
      },
      "items_total": 10,
      "items": [
        {
          "id": 3538559,
          "uuid": "ee8da1a4-2085-4519-99f2-5d28b2c1ac37",
          "name": "Vibe",
          "path": "vibe_1_5",
          "images": {
            "32x32": "https://storage.googleapis.com/dealroom-images-production/c1/MzI6MzI6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNS8wMS8wMy83N2I0ZDgxYTVhMDAwZTFiODI3MDkxM2YwN2Y4MjQ5Mg==.png",
            "74x74": "https://storage.googleapis.com/dealroom-images-production/12/NzQ6NzQ6Y29tcGFueUBzMy1ldS13ZXN0LTEuYW1hem9uYXdzLmNvbS9kZWFscm9vbS1pbWFnZXMvMjAyNS8wMS8wMy83N2I0ZDgxYTVhMDAwZTFiODI3MDkxM2YwN2Y4MjQ5Mg==.png",
            "100x100": "https://storage.googleapis.com/dealroom-images-production/88/MTAwOjEwMDpjb21wYW55QHMzLWV1LXdlc3QtMS5hbWF6b25hd3MuY29tL2RlYWxyb29tLWltYWdlcy8yMDI1LzAxLzAzLzc3YjRkODFhNWEwMDBlMWI4MjcwOTEzZjA3ZjgyNDky.png"
          }
        },
        // truncated for example
      ]
    }
  ],
  "nearby": [
    {
      "name": "Cuerdas Clasicas",
      "path": "cuerdas_clasicas",
      "hq_locations": [
        {
          "id": 5130708,
          "address": "Chicago, Cook County, Illinois, United States",
          "street": "",
          "street_number": "",
          "zip": "",
          "lat": 41.8755616,
          "lon": -87.6244212,
          "country": {
            "id": 23,
            "name": "United States",
            "lat": 40.730137,
            "lon": -73.990129
          },
          "city": {
            "id": 104717,
            "name": "Chicago",
            "lat": 1,
            "lon": -87.629457
          },
          "continent": {
            "id": 8,
            "name": "North America"
          },
          "is_headquarters": true,
          "is_founding_location": false,
          "state": {
            "id": 18673,
            "name": "Illinois",
            "lat": 1,
            "lon": -89.433729
          }
        }
      ],
      "industries": [
        {
          "id": 100070,
          "name": "event tech"
        }
      ]
    },
    // truncated for example
  ]
}
```

## 🛟 SUPPORT

Share your runs with the developer team and create issues on error to help us improve actor quality.

You might discover edge case we didn't test yet

We stay available anytime