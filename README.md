# Awesome-Web-Conferencing-Virtual-Classroom

## Top Web Content Authoring Tools Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Database-First Admin Panels, Git-Backed Markdown Authoring & Visual Page Building*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Web Content Authoring**. These tools give editors and marketers a structured interface for creating and managing content — pages, blog posts, assets, and structured data — without touching code, while developers get APIs and schemas that fit their stack.

**Examples** include Directus, Strapi, Payload, TinaCMS, Sveltia CMS, Contentful, Sanity, and Storyblok (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, database ownership, and Git-backed content workflows — ideal for teams who want editorial convenience without surrendering their data to a proprietary SaaS.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Contentful** — **The enterprise headless CMS standard.** Structured content platform with a mature API, workflow approvals, multi-locale support, and SLAs. **Best for large organizations** needing enterprise governance and vendor support, accepting per-seat pricing and cloud-only deployment [citation:2][citation:4].

- **Sanity** — **The design-led content platform with the best editor UX.** Real-time collaborative editing built into Studio, GROQ query language, and a customizable React-based editing environment. **Free tier** for small projects; paid tiers for scale. **Best for marketing and content sites** where editor experience matters most [citation:2][citation:13].

- **Storyblok** — **The visual page-building CMS.** Combines structured content with a visual editor for building pages component-by-component. **Best for non-technical editors** who need to assemble pages visually without developer involvement [citation:2][citation:4].

- **Prismic** — Headless CMS with a visual editor and slice-based page building. **Best for marketing teams** wanting reusable content components.

## Open-Source GitHub Projects

- **Directus** — **The database-first admin panel that wraps any SQL database.** **Source-available under a Business Source License** (not OSI-approved, matters for licensing requirements) [citation:4]. **Connects to existing PostgreSQL, MySQL, SQLite, MS SQL, MariaDB, or CockroachDB** — the data lives in your database, not Directus, so you could remove Directus tomorrow and your data remains in a format you own [citation:4]. **Polished admin UI** designed for non-technical users, with field-level role-based permissions, REST + GraphQL + WebSocket subscriptions, and a **native MCP server** for AI agent integrations [citation:4]. **Free for organizations under $5M annual revenue and under 50 employees**; Cloud at $99/mo [citation:4]. **Best for teams with an existing database** wanting an instant admin UI and API without schema migration [citation:14].

- **Strapi** — **The most popular open-source headless CMS by GitHub stars (72.9k).** **MIT licensed Community edition** — OSI-approved, forkable, and modifiable [citation:4][citation:7]. **Code-first content types** with a visual Content-Type Builder in the admin UI that writes schema files into your project. **Largest plugin marketplace** (100+ plugins) and extensive documentation. **Supports PostgreSQL, MySQL, MariaDB, and SQLite** — but **does not support MongoDB or any NoSQL database**, and **is not designed to connect to a pre-existing database** not created by Strapi [citation:7]. **Pricing**: Community free forever; Growth at $45/month including 3 seats, then $15/month per additional seat [citation:7]. **Best for teams wanting the largest community and plugin ecosystem**, especially those starting greenfield projects [citation:4][citation:14].

- **Payload** — **The TypeScript-native CMS that installs into your Next.js app.** **MIT licensed** — OSI-approved [citation:7]. **Configuration-as-code**: collections are defined in TypeScript, types are generated automatically, and every schema change goes through code review and ships with your deploy [citation:7]. **Native Next.js integration** — Payload drops into your existing `/app` folder, and the **Local API** lets you query content directly in React Server Components with no network hop [citation:7]. **Database support**: MongoDB via Mongoose, PostgreSQL via Drizzle, and SQLite via Drizzle [citation:7]. **44.1k GitHub stars** with active development [citation:7]. **Best for engineering-led teams** building Next.js applications who want their CMS to feel like their own code rather than a third-party dependency [citation:2][citation:4].

- **TinaCMS** — **The Git-backed Markdown CMS with visual editing.** Open-source, **content stored in your own GitHub repository** — no database, no vendor lock-in . **Supports Markdown, MDX, JSON, YAML** with a GraphQL API for querying content . **Live preview** makes editing Markdown intuitive for less-technical users . **Best for Jamstack sites** built with Astro, Eleventy, Hugo, or Next.js where content lives in Git .

- **Sveltia CMS** — **The modern successor to Netlify/Decap CMS.** Open-source, **Git-based headless CMS** for Jamstack sites . **Complete rewrite of Netlify CMS** with 310 solved issues from the original project, improved performance, security, and first-class i18n support . **Single-page web application served from a CDN** — small, maintenance-free, and framework-agnostic . **450+ real-world examples** including a U.S. government website and 65 sites migrated from WordPress . **Best for teams migrating from Netlify/Decap CMS** or wanting a lightweight Git-backed editing experience.

### Additional Strong Open-Source Options

- **Kirby** — File-based CMS with a polished admin panel. **Content stored as files on disk** rather than a database. 1,208 GitHub stars [citation:5]. Best for designers and agencies wanting a flat-file CMS with a strong editing experience.
- **Squidex** — Headless CMS and content management hub in C#. 2,153 GitHub stars [citation:5]. Best for .NET teams wanting a headless CMS built on their stack.
- **dotCMS** — Headless/hybrid CMS for enterprises in Java. 819 GitHub stars [citation:5]. Best for Java shops needing enterprise CMS capabilities.
- **FireCMS** — Firebase/Firestore-based CMS. 1,088 GitHub stars [citation:5]. Best for teams already on Firebase wanting an admin panel for their data.

**Frameworks for building custom systems**: Combine **Directus** for an instant admin UI over an existing SQL database with field-level permissions, **Payload** for TypeScript-native CMS inside a Next.js app with Local API access, **Strapi** for the largest plugin ecosystem and community support, **TinaCMS** or **Sveltia CMS** for Git-backed Markdown authoring without a database — to build a web content authoring stack tailored to your database ownership requirements, framework, and editorial team's technical comfort.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Web content authoring tools differ significantly in licensing, database ownership, and editorial workflow. **Directus is source-available, not OSI-approved** — matters if your organization has strict open-source licensing requirements [citation:4]. **Strapi does not support MongoDB** and **cannot connect to a pre-existing database** not created by Strapi [citation:7]. **Payload requires a Next.js app** — if your primary consumer is not Next.js, a large part of its value proposition does not apply [citation:7]. **TinaCMS and Sveltia CMS store content in Git** — ideal for Jamstack sites but not for teams needing a database-backed CMS with complex relational content. **Contentful and Sanity are cloud-only** — no self-hosting path.
- Self-hosted open-source solutions require proper database configuration (PostgreSQL for Directus, Payload, or Strapi), Node.js runtime setup, and awareness that "free" self-hosted still has infrastructure and maintenance costs.

---

**Made for content teams, marketers, and developers choosing authoring tools that match their database, framework, and editorial workflow.**
Let's make web content authoring more open, self-hostable, and editor-friendly.
