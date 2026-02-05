# BrandArgus

**AI-Powered Domain Intelligence for Brand Protection**

BrandArgus is a domain threat intelligence platform built for trademark attorneys, brand protection teams, and security professionals. We provide 24/7 automated domain monitoring with multi-layer AI analysis to detect trademark infringement the moment it happens.

## Open Research Program

We provide **free API access** to our domain intelligence feeds for qualified professionals committed to making the internet safer.

### Available APIs

#### NRDS Search API

Search and analyze newly registered gTLD domains within the past 30 days.

```

- **Search** — Query NRDs with advanced filtering (keyword, TLD, date range, pattern matching)
- **Count** — Get matched domain count without full results
- **Export** — Download results as CSV
- **Health** — Check service status and data freshness

Key filters: `keyword`, `tld`, `match` (contains/prefix/suffix), `reg_after`, `reg_before`, `has_hyphen`, `has_number`, `pure_alpha`, `min_len`, `max_len`

**Quick Example:**
```bash
curl -H "Authorization: Bearer YOUR_API_KEY" \
  "/nrds-search/domains?keyword=nike&tld=com&limit=100"
```

#### NS Reverse Lookup API

Identify all gTLD domains hosted under a specific nameserver infrastructure.
```
Base URL: https://api.brandargus.com/v1/ns-reverse
```

- **Search** — Query domains by nameserver with advanced filtering
- **Count** — Get total domains under a nameserver
- **Export** — Download full domain list as CSV
- **Health** — Check service status and data freshness

Supports the same advanced filters as NRDS Search, plus nameserver-based queries.

**Quick Example:**
```bash
curl -H "Authorization: Bearer YOUR_API_KEY" \
  "/ns-reverse/domains?ns=ns1.example.com&tld=com"
```

### Data Coverage

| Attribute | Details |
|-----------|---------|
| Domain Types | Major gTLDs (com, net, org, info, xyz, etc.) |
| Update Frequency | Daily |
| Data Sources | Multi-source|
| Authentication | Bearer Token + IP Whitelist |
| Rate Limit | 50-120 requests/min |

### Use Cases

- **Brand Protection** — Daily alerts for domains containing your brand name
- **Threat Campaign Tracking** — Identify malicious registration patterns
- **Infrastructure Analysis** — Map domain portfolios by nameserver

### Who Can Apply

- Brand protection professionals
- Cybersecurity students and academic researchers

### How to Apply

Send your application to **info@lyalpha-gmbh.com** or **info@abtdomain.com** with:

1. Your name and affiliation
2. Intended use case
3. A static IP address or CIDR range for API access

Full API documentation will be provided upon approval.

## Platform Features

- **24/7 Domain Monitoring** — Continuous multi-source intelligence across all TLDs
- **AI Threat Analysis** — Semantic and visual analysis powered by multi-layer AI engine
- **Traffic Light Classification** — Threat (alert), Uncertain (re-observe), Clean (exclude)
- **Evidence Collection** — Screenshots, WHOIS data, and risk reports ready for legal action

## Links

- Website: [brandargus.com](https://brandargus.com)
- Contact: info@brandargus.com
- Platform: [members.brandargus.com](https://members.brandargus.com)

## About

BrandArgus is powered by [ABTdomain](https://abtdomain.com), a domain intelligence platform.

---

© 2025 Lyalpha GmbH. All rights reserved.