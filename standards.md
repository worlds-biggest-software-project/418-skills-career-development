# Standards & API Reference

> Project: Skills & Career Development Platform · Generated: 2026-05-07

## Industry Standards & Specifications

### Skills Taxonomy & Occupational Classification Standards

**ESCO — European Skills, Competences, Qualifications and Occupations**
- Official URL: https://esco.ec.europa.eu/en/classification
- ESCO is the multilingual classification developed by the European Commission covering 13,890+ skills and 3,000+ occupations across 27 European languages. It is licensed under EUPL 1.2 (free software) and provides the most comprehensive open skills taxonomy for international deployments. A REST API and downloadable datasets are freely available for integration.

**O\*NET — Occupational Information Network (U.S. Department of Labor)**
- Official URL: https://www.onetcenter.org
- The U.S. federal standard for occupational data, profiling nearly every job in the U.S. economy with detailed skills, abilities, knowledge, work activities, and task ratings. Updated continuously and freely available. The O\*NET-SOC taxonomy is the de-facto U.S. standard for role and skills definitions. A web services REST API is available for registered developers.

**ISCO — International Standard Classification of Occupations (ILO)**
- Official URL: https://www.ilo.org/public/english/bureau/stat/isco/
- The International Labour Organization's four-level hierarchical classification of occupations used by statistical agencies globally. ISCO-08 (current version) underpins ESCO's occupational classification, providing the international crosswalk layer. Essential for platforms targeting multi-country deployments.

**ESCO–O\*NET Crosswalk**
- Official URL: https://esco.ec.europa.eu/en/about-esco/data-science-and-esco/crosswalk-between-esco-and-onet
- A machine-learning-assisted mapping maintained by the European Commission connecting ESCO occupations to O\*NET-SOC codes. Critical for platforms needing to interoperate with both European and U.S. labour market data.

---

### IEEE Learning Technology Standards

**IEEE 1484.20.1-2007 — Data Model for Reusable Competency Definitions**
- Official URL: https://standards.ieee.org/ieee/1484.20.1/4012/
- Defines a data model for describing, referencing, and sharing competency definitions, primarily in online and distributed learning contexts. Provides a standard representation of key competency characteristics, enabling interoperability among learning systems. The foundational IEEE standard for competency data models.

**IEEE 1484.20.2 — Recommended Practices for Defining Competencies**
- Official URL: https://sagroups.ieee.org/1484-20-2/
- Published December 2022. Promotes a common understanding for those involved in defining policies, standards, and data structures for competency definitions and frameworks. Covers ethical development, documentation, and reuse of competency definitions. Directly relevant to skills taxonomy design.

**IEEE 1484.20.3 — Data Model for Shareable Competency Definitions**
- Official URL: https://standards.ieee.org/ieee/1484.20.3/10749/
- Defines a formal data model for describing, referencing, and sharing competency definitions and rubrics in online learning and employment contexts. Extends 1484.20.1 with richer data model constructs for cross-system sharing.

**IEEE 1484.12.1-2002 — Learning Object Metadata (LOM)**
- Official URL: https://standards.ieee.org/standard/1484_12_1-2002.html
- Defines the data model for describing learning objects and resources — what aspects should be described and which vocabularies are valid. Relevant for any platform integrating external learning content libraries.

---

### 1EdTech / IMS Global Learning Standards

**xAPI (Experience API / Tin Can API)**
- Official URL: https://xapi.com
- ADL specification (now maintained by the Advanced Distributed Learning Initiative) for recording any type of learning experience — not just web-based courses. Tracks learning statements in the form "actor verb object" (e.g., "Jane completed SQL Intermediate course"). The foundational open standard for learning activity data capture across platforms, mobile apps, simulations, and real-world activities. Requires a Learning Record Store (LRS) to persist data.

**cmi5 Profile for xAPI**
- Official URL: https://aicc.github.io/CMI-5_Spec_Current/
- Maintained by AICC. Bridges SCORM and xAPI by defining interoperability rules for launch, authorisation, reporting, and course structure between an LMS and xAPI-enabled learning activities. The current de-facto successor to SCORM, actively developed and backed by U.S. DoD as the official SCORM replacement. Recommended for new platform development.

**SCORM (Sharable Content Object Reference Model)**
- Official URL: https://scorm.com/scorm-explained/
- The most widely deployed eLearning interoperability standard (SCORM 1.2 and 2004). Despite being superseded by xAPI/cmi5, SCORM remains necessary for legacy content compatibility. Any platform integrating commercial content libraries must support SCORM.

**LTI — Learning Tools Interoperability (v1.3 Advantage)**
- Official URL: https://www.1edtech.org/standards/lti
- 1EdTech (formerly IMS Global) specification enabling LMS platforms to securely connect to external learning tools using OAuth 2.0 and OpenID Connect. LTI 1.3 Advantage includes Assignment and Grade Services v2.0, Names and Role Provisioning Services v2.0, and Deep Linking v2.0. Essential for integrating third-party learning tools and content providers.

**Open Badges 3.0**
- Official URL: https://www.imsglobal.org/spec/ob/v3p0
- Maintained by 1EdTech. The open standard for digital credentials recognising learning achievements. Version 3.0 (released 2023) aligns Open Badges with the W3C Verifiable Credentials Data Model v2.0, making badges cryptographically signed, tamper-proof, and portable across systems. Defines a RESTful API with OAuth 2.0 authentication. Directly applicable for skills certification and achievement recognition.

**IMS Caliper Analytics**
- Official URL: https://www.imsglobal.org/caliper
- IMS Global standard for learning analytics events. Complements xAPI by defining agreed-upon event vocabularies for aggregation across educational systems. More prescriptive than xAPI for institutional analytics.

---

### W3C & IETF Standards

**W3C Verifiable Credentials Data Model v2.0**
- Official URL: https://www.w3.org/TR/vc-data-model-2.0/
- Published as a W3C Recommendation in May 2025. Defines the data model for tamper-proof, cryptographically verifiable digital credentials (skills, qualifications, achievements). Seven W3C Recommendations were published together, covering the data model, JSON-LD context, and proof mechanisms. Fully backwards compatible with v1.1. Foundation for portable, verifiable skills credentials that employees own and carry between employers.

**Schema.org — EducationalOccupationalCredential**
- Official URL: https://schema.org/EducationalOccupationalCredential
- Schema.org vocabulary for structured data markup of educational and occupational credentials, including `competencyRequired` and `credentialCategory` properties. Enables search engines and HR systems to parse credential and skills data semantically. Backed by JSON-LD for linked data compatibility.

**Schema.org — Occupation**
- Official URL: https://schema.org/Occupation
- Schema.org type for representing occupations with skills, qualifications, salary range, and relevant experience. Enables structured data for job descriptions and role definitions interoperable with search and job board platforms.

**RFC 7519 — JSON Web Tokens (JWT)**
- Official URL: https://datatracker.ietf.org/doc/html/rfc7519
- IETF standard for compact, URL-safe means of representing claims between parties as a JSON object, cryptographically signed. JWT is the token format used by OAuth 2.0, OpenID Connect, and LTI 1.3. Fundamental for all modern API authentication in HR systems.

**RFC 6749 — OAuth 2.0 Authorization Framework**
- Official URL: https://datatracker.ietf.org/doc/html/rfc6749
- IETF standard for delegated authorisation. De-facto standard for API access in enterprise HR platforms (Workday, SAP SuccessFactors, iMocha, Cornerstone all use OAuth 2.0). Required for any platform exposing APIs to third-party integrators.

---

### Data Model & API Specification Standards

**HR Open Standards (formerly HR-XML Consortium)**
- Official URL: https://www.hropenstandards.org/
- Non-profit consortium providing open JSON and XML standards for HR data exchanges covering recruiting, onboarding, payroll, competencies, and learning. Version 4.5 (2025–2026) introduces the Trusted Career Profile (TCP) evolving from the Learning and Employment Record Resume Standard (LER-RS), with an Open API for HRIS vendors. JSON Schema and JSON-LD based. Free to download and implement.

**OpenAPI Specification 3.1**
- Official URL: https://spec.openapis.org/oas/v3.1.0
- The de-facto standard for describing RESTful APIs. All major HR platforms (Workday, SAP SuccessFactors, Cornerstone, iMocha) expose OpenAPI-described REST APIs. Any new skills platform API should be documented with OpenAPI 3.1 for developer adoption and ecosystem integration.

---

### Security & Compliance Standards

**OAuth 2.0 / OpenID Connect (OIDC)**
- Official URL: https://openid.net/connect/
- OIDC builds on OAuth 2.0 to add identity layer and standardised user authentication using JSON Web Tokens. Used by Workday, SAP SuccessFactors, Cornerstone, and iMocha for API authentication. The standard for SSO in enterprise HR deployments.

**SAML 2.0 — Security Assertion Markup Language**
- Official URL: https://www.oasis-open.org/standards#samlv2.0
- OASIS standard for XML-based federated identity and SSO, widely used in regulated enterprise environments with Active Directory integration. SAML 2.0 SSO support is mandatory for enterprise HR technology adoption (required by Workday, SAP, and major enterprise buyers).

**GDPR — General Data Protection Regulation (EU 2016/679)**
- Official URL: https://gdpr.eu/
- The primary European Union privacy regulation governing how organisations collect, store, and process personal data including employee skills data, assessment results, and career profiles. Non-compliance can result in fines up to €20 million or 4% of global annual revenue. Skills platforms processing EU employee data must establish lawful processing grounds, honour data subject rights (access, rectification, erasure), and implement data minimisation. Critical for any platform targeting European customers.

**NIST Privacy Framework v1.0**
- Official URL: https://www.nist.gov/privacy-framework
- U.S. voluntary framework for managing privacy risk in technology products. Complements GDPR for U.S. deployments and provides a structured approach to data classification, privacy risk assessment, and protection controls relevant to employee skills data.

---

## Similar Products — Developer Documentation & APIs

### O\*NET Web Services API
- **Description:** RESTful API providing programmatic access to the full O\*NET occupational database — skills, abilities, tasks, knowledge requirements, and work activities for nearly every U.S. occupation. Free for registered developers; read-only GET endpoints.
- **API Documentation:** https://services.onetcenter.org/reference/
- **Getting Started / Signup:** https://services.onetcenter.org/
- **Sample Code:** https://github.com/onetcenter/web-services-samples
- **Standards:** REST/JSON, GET-only, API key authentication
- **Authentication:** API key (registered developer access)

### ESCO Web Service API
- **Description:** REST API providing access to the full ESCO classification — 13,890+ skills/competences, 3,000+ occupations, qualifications, and their interrelationships. Multilingual (27 languages). Licensed under EUPL 1.2 (open source). Supports ESCO v1 dataset.
- **API Documentation:** https://esco.ec.europa.eu/en/use-esco/use-esco-services-api
- **Web Service API:** https://esco.ec.europa.eu/en/use-esco/use-esco-services-api/esco-web-service-api
- **Standards:** REST, linked data (URI-based concepts), JSON and RDF response formats
- **Authentication:** Open access (no authentication required for public classification)

### Workday REST API
- **Description:** REST API providing access to Workday HCM data including worker records, job profiles, learning completions, and organisational structure. Covers the full Workday HCM suite including Skills Cloud data via the broader Talent module endpoints.
- **API Documentation:** https://community.workday.com/articles/developer
- **Integration Guide:** https://samaintegrations.com/mastering-workday-rest-api-integration-the-complete-2025-guide-for-businesses/
- **SDKs/Libraries:** No official SDK; standard HTTP clients; third-party integration via Knit, Apideck, Merge.dev
- **Standards:** REST/JSON, OpenAPI
- **Authentication:** OAuth 2.0 (Bearer tokens); rate limit ~10 calls/second

### SAP SuccessFactors API (SAP API Business Hub)
- **Description:** OData v2.0 and REST APIs covering the full SuccessFactors HCM suite including Talent Intelligence Hub (skills data), Learning, Performance, Succession, and Recruiting modules. Documentation available on SAP Business Accelerator Hub with interactive API explorer.
- **API Documentation:** https://api.sap.com/products/SAPSuccessFactors/apis/REST
- **OData API Reference:** https://help.sap.com/docs/SAP_SUCCESSFACTORS_PLATFORM/d599f15995d348a1b45ba5603e2aba9b/03e1fc3791684367a6a76a614a2916de.html
- **SDKs/Libraries:** SAP Cloud SDK (Java, JavaScript); standard OData clients
- **Standards:** OData v2.0, REST/JSON, OpenAPI
- **Authentication:** OAuth 2.0 (SAML bearer assertion for enterprise SSO)

### iMocha Skills Assessment API
- **Description:** REST API providing access to iMocha's 10,000+ skills assessment library. Enables integration of validated assessments into ATS, LMS, and custom HR platforms. API delivers assessment invitations, results, and skills reports. Positioned as the world's largest skills assessment API platform.
- **API Documentation:** https://developer.imocha.io/
- **Developer Portal:** https://developer.imocha.co.in/
- **Integrations Page:** https://imocha.io/solutions/api-integrations-and-platforms
- **Standards:** REST/JSON, OpenAPI (Swagger)
- **Authentication:** API key (requested via support@imocha.io); OAuth 2.0 for enterprise SSO

### Degreed API
- **Description:** REST API enabling integration with Degreed's Learning Experience Platform. Supports content management (add/update/delete), user management, required learning, and completion tracking. Also supports xAPI for learning activity statements. OAuth 2.0 with scope-based access control.
- **API Documentation:** https://developer.degreed.com/docs/degreed-integrations
- **API Reference:** https://developer.degreed.com/reference/overview
- **Getting Started:** https://developer.degreed.com/docs/getting-started-with-the-api
- **xAPI Integration:** https://developer.degreed.com/docs/getting-started-with-the-xapi
- **Standards:** REST/JSON, xAPI, OAuth 2.0
- **Authentication:** OAuth 2.0 (Client ID + Client Secret → Bearer token)

### Cornerstone OnDemand API
- **Description:** RESTful API (JSON and XML) covering learning management, skills, performance, and talent modules within the Cornerstone Galaxy platform. Developer portal with registration, scoped API keys, and interactive documentation. Broad HRIS connector ecosystem via Galaxy Extend Marketplace.
- **API Documentation:** https://csod.dev/
- **API Overview:** https://help.csod.com/help/csod_0/Content/User/Edge/Overview_Topics_-_Edge/APIs_Overview.htm
- **SDKs/Libraries:** No official SDK; REST/HTTP clients; GitHub samples: https://github.com/cpscc/wiki
- **Standards:** REST/JSON and XML, OpenAPI
- **Authentication:** OAuth 2.0 (Client ID + Secret); SAML 2.0 for SSO

### Eightfold AI API
- **Description:** REST API for the Eightfold Talent Intelligence Platform. Provides access to AI-driven talent matching, career recommendations, internal mobility, and skills inference capabilities. Pre-built integration adaptors for SAP SuccessFactors, Greenhouse, and ATS systems. Bidirectional data synchronisation.
- **API Documentation:** https://apidocs.eightfold.ai/
- **SAP Integration Guide:** https://eightfold.ai/wp-content/uploads/integrating_eightfold_talent_intelligence_platform_with_sap_successfactors.pdf
- **Standards:** REST/JSON
- **Authentication:** OAuth 2.0

### TalentGuard API
- **Description:** API-first architecture enabling integration with Workday, SAP SuccessFactors, Oracle HCM, and Cornerstone. Provides access to skills ontology, career pathing frameworks, role definitions, readiness scores, and succession planning data. Supports bidirectional data exchange with major HRIS platforms.
- **API Documentation:** https://www.talentguard.com/platform/integrations
- **Standards:** REST/JSON; API-first architecture
- **Authentication:** OAuth 2.0 / enterprise SSO

### Fuel50 Integrations API
- **Description:** REST API enabling integration of Fuel50's Career Pathways and Talent Marketplace with HRIS, ATS, and LMS systems. Bidirectional connector with Degreed for learning content; supports skills mapping and gig opportunity exchange. Pre-built connectors for major HR platforms.
- **API Documentation:** https://fuel50.com/integrations/
- **Standards:** REST/JSON
- **Authentication:** OAuth 2.0; pre-built connectors for HRIS/ATS platforms

---

## Notes

**Active Standards Evolution**

The skills technology standards landscape is evolving rapidly. Key developments to monitor:

- **W3C Verifiable Credentials v2.0** (W3C Recommendation, May 2025) is actively being adopted by 1EdTech for Open Badges 3.0 and by the HR Open Standards Consortium for the Trusted Career Profile (TCP). Portable, employee-owned skills credentials are likely to become a market expectation within 2–3 years.
- **HR Open Standards v4.5 Trusted Career Profile** (2025–2026) bridges the Learning and Employment Record ecosystem with enterprise HR platforms. This standard is designed to replace siloed skills records with portable verifiable profiles. An open API specification for HRIS vendors is part of the deliverables.
- **cmi5 adoption is accelerating** as U.S. DoD-mandated SCORM replacement. New platforms should implement cmi5 natively rather than SCORM 2004.
- **ESCO v1.2 update** is expected; the ESCO API update announcement (https://esco.ec.europa.eu/en/news/esco-api-be-updated-soon) signals an upcoming version change that will affect integrations built against the current API.

**Gaps in Available Standards**

- No open standard exists for **skills inference algorithms** or **readiness scoring methodologies** — these remain proprietary to each vendor.
- No interoperability standard covers **internal talent marketplace** data exchange between employers or platforms.
- **Predictive skill obsolescence** has no standardised data model or benchmark — an area where a new platform could establish early de-facto conventions.
