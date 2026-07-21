# OneTick (OneMarketData) (onetick)

OneTick, from OneMarketData, is an enterprise tick database and analytics platform for capital markets, capturing, storing, and analyzing trade, quote, and order-book time series at scale for quant research, transaction cost analysis, and trade surveillance. OneTick Cloud sells historical and reference market data covering 200+ global equities, options, and futures venues (history back to 1993, corporate actions, symbol cross-reference) delivered on demand through an OAuth2-secured REST WebAPI, a pandas-like Python API (onetick-py), a directed-graph Python API, SQL querying, and file delivery, with a self-serve trial registration. The detailed REST endpoint reference sits behind the cloud dashboard login. OneMarketData merged with KX in September 2025 under TA Associates ownership.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/onetick/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/onetick/refs/heads/main/apis.yml)

## Tags

- Financial
- Market Data
- Tick Data
- Historical Data
- Trading
- Analytics
- Surveillance
- Time Series
- Equities
- Options

## Timestamps

- **Created:** 2026-07-21
- **Modified:** 2026-07-21

## APIs

### OneTick Cloud REST API (WebAPI)

HTTPS REST access to OneTick Cloud market data and analytics queries, authenticated with an OAuth2 client-credentials Bearer token issued by the OneTick Keycloak realm. A REST URL builder and per-endpoint reference (parameters and output schemas) are provided behind the cloud dashboard login; the public page describes the API but does not enumerate endpoints.

- **Human URL:** [https://www.onetick.com/cloud-services/rest-api-end-point-documentation](https://www.onetick.com/cloud-services/rest-api-end-point-documentation)
- **Base URL:** `https://rest.cloud.onetick.com/omdwebapi/rest/`

#### Tags

- REST
- Market Data
- Tick Data
- Historical Data

#### Properties

- [Documentation](https://www.onetick.com/cloud-services/rest-api-end-point-documentation)
- [Documentation (WebAPI setup walkthrough)](https://blog.onetick.com/basic-setup-of-webapi-access-to-onetick-cloud)

### OneTick Python API - onetick-py (pandas-style)

A pandas-like Python API for querying tick-by-tick market data in OneTick, published on PyPI as onetick-py with openly browsable documentation. Against OneTick Cloud it executes over the WebAPI transport using the same OAuth2 client credentials, returning results as pandas DataFrames.

- **Human URL:** [https://docs.pip.distribution.sol.onetick.com/](https://docs.pip.distribution.sol.onetick.com/)
- **Base URL:** `https://rest.cloud.onetick.com`

#### Tags

- Python
- Pandas
- Market Data
- Analytics

#### Properties

- [Documentation](https://docs.pip.distribution.sol.onetick.com/)
- [GitHub Repository](https://github.com/onemarketdata/onetick-py)
- [Documentation (query examples)](https://www.onetick.com/cloud-services/onetick-python-queries-using-pandas-style-api)

### OneTick Python API - Directed Graph

The lower-level directed-graph-style Python query API for OneTick, composing event-processor graphs against tick series, with openly browsable documentation and worked examples on the OneTick Cloud site.

- **Human URL:** [https://pythonquery.docs.sol.onetick.com/intro.html](https://pythonquery.docs.sol.onetick.com/intro.html)

#### Tags

- Python
- Query
- Market Data

#### Properties

- [Documentation](https://pythonquery.docs.sol.onetick.com/intro.html)
- [Documentation (query examples)](https://www.onetick.com/cloud-services/onetick-python-queries-using-directed-graph-style-api)

### OneTick SQL API

SQL querying over OneTick tick and reference data, documented openly and runnable against OneTick Cloud (including via otp.SqlQuery in onetick-py over the WebAPI transport).

- **Human URL:** [https://sql.docs.sol.onetick.com/intro.html](https://sql.docs.sol.onetick.com/intro.html)

#### Tags

- SQL
- Query
- Market Data

#### Properties

- [Documentation](https://sql.docs.sol.onetick.com/intro.html)
- [GitHub Repository](https://github.com/onemarketdata/onetick-sql-docs)
- [Documentation (SQL querying examples)](https://www.onetick.com/cloud-services/sql-querying-examples)

### OneTick Point-in-Time TCA API

Cloud API for extracting adjusted and unadjusted point-in-time quotes and trades at nanosecond precision across 200+ venues for transaction cost analysis, packaged for Python integration; marketed sales-led (request a demo) with no public endpoint reference.

- **Human URL:** [https://www.onetick.com/pit-tca-api](https://www.onetick.com/pit-tca-api)

#### Tags

- TCA
- Transaction Cost Analysis
- Historical Data

#### Properties

- [Documentation](https://www.onetick.com/pit-tca-api)
- [Documentation (methodology)](https://www.onetick.com/pit-tca-methodology)

## Common Properties

- [Website](https://www.onetick.com/)
- [Portal (OneTick Cloud dashboard)](https://authdash.cloud.onetick.com/web_dashboard/?dash=sub_profile)
- [Documentation](https://docs.pip.distribution.sol.onetick.com/)
- [GitHub Organization](https://github.com/onemarketdata)
- [LinkedIn](https://www.linkedin.com/company/onemarketdata)
- [Blog](https://blog.onetick.com/)
- [Sign Up (OneTick Cloud trial registration)](https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/registrations?client_id=acf_onetick_cloud&scope=openid%20profile&redirect_uri=https://authdash.cloud.onetick.com/web_dashboard/j_security_check&response_type=code)
- [Terms of Service](https://www.onetick.com/terms-of-use)
- [Privacy Policy](https://www.onetick.com/privacy-policy)
- [Contact](https://www.onetick.com/contact)
- [Status Page (system availability)](https://www.onetick.com/cloud-services/system-availability)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
