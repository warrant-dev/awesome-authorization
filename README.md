<div align="center" alt="Warrant">
    <a href="https://warrant.dev/?utm_source=awesome-authz" target="_blank">
        <img src="https://warrant.dev/images/logo-primary-wide.png" width="300">
    </a>
    </br>
    </br>
</div>

# Awesome Authorization [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

> A curated list of information and best practices for authorization and access control.

## Contents
- [Overview](#overview)
- [Authentication vs. Authorization](#authentication-vs-authorization)
- [Access Control Models](#access-control-models)
- [Security Concerns](#security-concerns)
- [Best Practices](#best-practices)
- [Useful Articles & Tutorials](#useful-articles--tutorials)
- [Authz In Practice](#authz-in-practice)
- [Videos & Talks](#videos--talks)

---

## Overview
- [NIST Authorization Definition](https://csrc.nist.gov/glossary/term/authorization) - "The process of verifying that a requested action or service is approved for a specific entity".

## Authentication vs. Authorization
- [Authentication](https://en.wikipedia.org/wiki/Authentication) - Determines *who* someone or something is (identity).
- [Authorization](https://en.wikipedia.org/wiki/Authorization) - Determines *what* someone or something can do in a system (privileges and permissions).
- [Understanding Authentication, Authorization, and Encryption](https://www.bu.edu/tech/about/security-resources/bestpractice/auth/) - Quick comparison of authn, authz and encryption.

## Access Control Models
- [ABAC](https://en.wikipedia.org/wiki/Attribute-based_access_control) - Attribute based access control.
- [DAC](https://en.wikipedia.org/wiki/Discretionary_access_control) - Discretionary access control.
- [GBAC](https://en.wikipedia.org/wiki/Graph-based_access_control) - Graph based access control.
- [MAC](https://en.wikipedia.org/wiki/Mandatory_access_control) - Mandatory access control.
- [OrBAC](https://en.wikipedia.org/wiki/Organisation-based_access_control) - Organization based access control.
- [ReBAC](https://www.scaledaccess.com/whitepapers/the-developers-guide-to-relationship-based-access-control) - Relationship based access control.
- [RBAC](https://en.wikipedia.org/wiki/Role-based_access_control) - Role based access control.

## Security Concerns
- [OWASP's Top 10 for 2021](https://owasp.org/Top10/) - List of the top 10 web application security risks. Broken access control is [#1](https://owasp.org/Top10/A01_2021-Broken_Access_Control/) on the list.
- Insecure Direct Object Reference
  - [IDOR & How to Protect Against It](https://blog.warrant.dev/insecure-direct-object-reference)
  - [The Rise of IDOR](https://www.hackerone.com/resources/hackerone/the-rise-of-idor)
  - [What is IDOR?](https://portswigger.net/web-security/access-control/idor)
  - [Broken Object Level Authorization](https://apisecurity.io/encyclopedia/content/owasp/api1-broken-object-level-authorization)
- [Broken Function Level Authorization](https://apisecurity.io/encyclopedia/content/owasp/api5-broken-function-level-authorization) - API incorrectly relies on the client to use the correct access level making it susceptible to hackers.

## Best Practices
- [OWASP Authorization Cheat Sheet & Recommendations](https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html) - Authz overview and recommendations for best practices.
  - Enforce least privileges and deny by default - Ensure that users and systems only have access to what they need and nothing else.
  - As fine-grained as possible - Authorization checks should be as specific as possible. Ideally, this means the system has the ability to check access based on specific records and resources.
  - Implement once and reuse - Keep authz logic in one place to ensure consistent checks and to prevent missed cases and potential security holes.
  - Maintain an audit log - Keep an authorization log (allow/deny) to track access and conduct audits where necessary.

## Useful Articles & Tutorials
- [API Tokens: A Tedious Survey](https://fly.io/blog/api-tokens-a-tedious-survey/) - An overview of different approaches to API security.
- [Ask HN: Best Practices for Web Authorization? (2016)](https://news.ycombinator.com/item?id=11151790) - HN discussion about application authorization best practices.
- [AWS - Authz & Access Control for SaaS Multi-tenant Apps](https://docs.aws.amazon.com/prescriptive-guidance/latest/saas-multitenant-api-access-authorization/welcome.html) - How-to/implementation guide for authz in multi-tenant apps using AWS.
- [Best Practices for Building Secure API Keys](https://www.freecodecamp.org/news/best-practices-for-building-api-keys-97c26eabfea9/) - Covers hashing, storage and key retrieval.
- [Implementing Role Based Access Control](https://blog.warrant.dev/implementing-role-based-access-control) - How-to/implementation guide for basic RBAC in an application.
- [Permissions Systems: Category Notes](https://kojo.blog/permissions-sytems/) - An overview of the permissions systems landscape.
- [Web App Access Control Design](https://owasp.org/www-pdf-archive/ASDC12-Access_Control_Designs_and_Pitfalls.pdf) - A presentation highlighting best practices for implementing access control in web apps.
- [Authorization in a Microservices World](https://www.alexanderlolis.com/authorization-in-a-microservices-world) - Covers approaches to authorization in microservices.

## Authz In Practice
- [What's the Best Authorization Framework? None At All](https://www.betterment.com/engineering/security-framework) - Opinionated blog post detailing Betterment's approach to authz.
- [GitHub Secret Scanning](https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning) - How GitHub scans repos to search for exposed secrets.
- [Open Policy Agent](https://www.openpolicyagent.org/) - A policy-based framework for authorization and access control.
- [Stripe API Docs](https://stripe.com/docs/keys) - Stripe's approach to issuing and managing API keys securely.
- [XACML](https://en.wikipedia.org/wiki/XACML) - Standard that defines the "Extensible Access Control Markup Language," a declarative fine-grained, attribute-based access control policy language.
  - [Intuit AuthZ](https://medium.com/intuit-engineering/authz-intuits-unified-dynamic-authorization-system-bea554d18f91) - Post detailing Intuit's implementation of an XACML-based authz service.
- [Google Zanzibar](https://research.google/pubs/pub48190/) - Google's consistent, global authorization system.
  - [Airbnb Himeji](https://medium.com/airbnb-engineering/himeji-a-scalable-centralized-system-for-authorization-at-airbnb-341664924574) - Based on Zanzibar.
  - [Carta AuthZ](https://medium.com/building-carta/authz-cartas-highly-scalable-permissions-system-782a7f2c840f) - Also based on Zanzibar.

## Videos & Talks
- [Hashicorp - Microservice Authentication and Authorization (2019)](https://www.youtube.com/watch?v=ZjPF8yZ83Wo)
- [How Netflix Is Solving Authorization Across Their Cloud (2017)](https://www.youtube.com/watch?v=R6tUNpRpdnY)
