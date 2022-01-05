<div align="center" alt="Warrant">
    <a href="https://warrant.dev/" target="_blank">
        <img src="https://warrant.dev/images/warrant_logo_wide.png" width="400">
    </a>
    </br>
    </br>
    </br>
</div>

# Awesome Authorization [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

> A curated list of information and resources about authorization.

Contributions welcome! Please see the [contribution guide](CONTRIBUTING.md).

## Table of Contents
- [Overview](#overview)
- [Authentication vs. Authorization](#authentication-vs-authorization)
- [Access Control Models](#access-control-models)
- [Security Concerns](#security-concerns)
- [Best Practices](#best-practices)
- [Useful Articles & Tutorials](#useful-articles--tutorials)
- [Authz In Practice](#authz-in-practice)
- [Videos & Talks](#videos--talks)
- [Books](#books)

---

## Overview
Authorization / Authorisation / Authz - "the process of verifying that a requested action or service is approved for a specific entity" [[NIST](https://csrc.nist.gov/glossary/term/authorization)]
- [OWASP Authorization Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html)
- [Wikipedia](https://en.wikipedia.org/wiki/Authorization)

## Authentication vs. Authorization
- Authentication - Determines *who* someone or something is (identity)
- Authorization - Determines *what* someone or something can do in a system (permissions)
- [Understanding Authentication, Authorization, and Encryption](https://www.bu.edu/tech/about/security-resources/bestpractice/auth/)

## Access Control Models
- [Role Based Access Control (RBAC)](https://en.wikipedia.org/wiki/Role-based_access_control)
- [Attribute Based Access Control (ABAC)](https://en.wikipedia.org/wiki/Attribute-based_access_control)
- [Graph Based Access Control (GBAC)](https://en.wikipedia.org/wiki/Graph-based_access_control)
- Relationship Based Access Control (ReBAC)
- [Organization Based Access Control (OrBAC)](https://en.wikipedia.org/wiki/Organisation-based_access_control)
- [Discretionary Access Control (DAC)](https://en.wikipedia.org/wiki/Discretionary_access_control)
- [Mandatory Access Control (MAC)](https://en.wikipedia.org/wiki/Mandatory_access_control)

## Security Concerns
- Broken access control is [#1](https://owasp.org/Top10/A01_2021-Broken_Access_Control/) on [OWASP's Top 10 for 2021](https://owasp.org/Top10/)
- Insecure Direct Object Reference
  - [IDOR & How to Protect Against It](https://blog.warrant.dev/insecure-direct-object-reference)
  - [The Rise of IDOR](https://www.hackerone.com/resources/hackerone/the-rise-of-idor)

## Best Practices
- [OWASP Recommendations](https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html#recommendations)
- *Enforce least privileges and deny by default* - Ensure that users and systems only have access to what they need and nothing else.
- *As fine-grained as possible* - Authorization checks should be as specific as possible. Ideally, this means the system has the ability to check access based on specific records and resources.
- *Implement once and reuse* - Keep authz logic in one place to ensure consistent checks and to prevent missed cases and potential security holes.
- *Maintain an audit log* - Keep an authorization log (allow/deny) to track access and conduct audits where necessary.

## Useful Articles & Tutorials
- [Web App Access Control Design](https://owasp.org/www-pdf-archive/ASDC12-Access_Control_Designs_and_Pitfalls.pdf) - A presentation highlighting best practices for implementing access control in web apps.
- [Ask HN: Best Practices for Web Authorization? (2016)](https://news.ycombinator.com/item?id=11151790)
- [Implementing Role Based Access Control](https://blog.warrant.dev/implementing-role-based-access-control)
- [AWS - Authz & Access Control for SaaS Multi-tenant Apps](https://docs.aws.amazon.com/prescriptive-guidance/latest/saas-multitenant-api-access-authorization/welcome.html)
- [Permissions Systems: Category Notes](https://kojo.blog/permissions-sytems/) - An overview of the permissions systems landscape.
- [Best Practices for Building Secure API Keys](https://www.freecodecamp.org/news/best-practices-for-building-api-keys-97c26eabfea9/)

## Authz In Practice
- [Zanzibar: Google's Consistent, Global Authorization System](https://research.google/pubs/pub48190/)
  - [Airbnb's Himeji](https://medium.com/airbnb-engineering/himeji-a-scalable-centralized-system-for-authorization-at-airbnb-341664924574)
  - [Carta's AuthZ](https://medium.com/building-carta/authz-cartas-highly-scalable-permissions-system-782a7f2c840f)
- [Open Policy Agent](https://www.openpolicyagent.org/)
- [XACML](https://en.wikipedia.org/wiki/XACML)
  - [Intuit's AuthZ](https://medium.com/intuit-engineering/authz-intuits-unified-dynamic-authorization-system-bea554d18f91)
- [Stripe's Approach to API Keys](https://stripe.com/docs/keys)

## Videos & Talks
- [How Netflix Is Solving Authorization Across Their Cloud (2017)](https://www.youtube.com/watch?v=R6tUNpRpdnY)
- [Hashicorp - Microservice Authentication and Authorization (2019)](https://www.youtube.com/watch?v=ZjPF8yZ83Wo)

## Books
- Contributions welcome!
