# OneTick (OneMarketData) (onetick)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
