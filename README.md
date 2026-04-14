# Claude Code Plugins

A curated directory of plugins, skills, and MCP integrations for [Claude Code](https://claude.ai/code). Extend your AI coding assistant with persistent memory, live data access, and production-grade developer workflows.

Claude Code is the most powerful agentic coding tool available. These plugins make it unstoppable.

[![Plugins](https://img.shields.io/badge/Plugins-50%2B-brightgreen)](https://vinkius.com)
[![MCP Servers](https://img.shields.io/badge/MCP_Servers-2%2C600%2B-blue)](https://vinkius.com/en/categories)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## Contents

- [Getting Started with Claude Code Plugins](#getting-started-with-claude-code-plugins)
- [Memory and Context](#memory-and-context)
- [Developer Productivity](#developer-productivity)
- [Database Access](#database-access)
- [Cloud and Infrastructure](#cloud-and-infrastructure)
- [Communication](#communication)
- [CRM and Sales](#crm-and-sales)
- [Analytics and Monitoring](#analytics-and-monitoring)
- [AI and Search](#ai-and-search)
- [Finance and Payments](#finance-and-payments)
- [Design and Media](#design-and-media)
- [How to Install a Plugin](#how-to-install-a-plugin)
- [How to Create Your Own Plugin](#how-to-create-your-own-plugin)

---

## Getting Started with Claude Code Plugins

Claude Code loads MCP servers from a `.mcp.json` file in your project root. Each entry in that file is a plugin — a live connection to an external tool your agent can use.

```bash
# Quick setup — add memory to Claude Code in 10 seconds
echo '{"mcpServers":{"memory":{"url":"YOUR_MEM0_URL"}}}' > .mcp.json
claude
/mcp  # verify connection
```

All plugins below are available as managed MCP servers on the [Vinkius AI Gateway](https://vinkius.com) — deploy in one click, get an SSE endpoint URL, paste it into your `.mcp.json`.

---

## Memory and Context

Give Claude Code long-term memory. It remembers your project across sessions.

| Plugin | What It Does | Deploy |
|---|---|---|
| [mem0-mcp](https://vinkius.com/en/apps/mem0-mcp) | Persistent memory for AI agents — store and recall learnings, decisions, preferences | [Deploy →](https://vinkius.com/en/apps/mem0-mcp) |
| [context7-mcp](https://vinkius.com/en/apps/context7-mcp) | Session context management — carry context between conversations | [Deploy →](https://vinkius.com/en/apps/context7-mcp) |
| [qdrant-mcp](https://vinkius.com/en/apps/qdrant-mcp) | Vector search — semantic retrieval of past code, docs, and decisions | [Deploy →](https://vinkius.com/en/apps/qdrant-mcp) |
| [pinecone-mcp](https://vinkius.com/en/apps/pinecone-mcp) | Managed vector database — high-performance similarity search | [Deploy →](https://vinkius.com/en/apps/pinecone-mcp) |
| [chroma-vector-db-mcp](https://vinkius.com/en/apps/chroma-vector-db-mcp) | Local-first vector DB — lightweight embedding storage | [Deploy →](https://vinkius.com/en/apps/chroma-vector-db-mcp) |

**Best for most projects:** Start with **Mem0** for general memory. Add **Qdrant** if you need semantic code search.

---

## Developer Productivity

Connect Claude Code to your development workflow.

| Plugin | What It Does | Deploy |
|---|---|---|
| [github-mcp](https://vinkius.com/en/apps/github-mcp) | Repos, issues, PRs, Actions, code search, releases | [Deploy →](https://vinkius.com/en/apps/github-mcp) |
| [gitlab-mcp](https://vinkius.com/en/apps/gitlab-mcp) | GitLab repos, CI/CD pipelines, merge requests | [Deploy →](https://vinkius.com/en/apps/gitlab-mcp) |
| [linear-mcp](https://vinkius.com/en/apps/linear-mcp) | Linear issues, projects, cycles, team workload | [Deploy →](https://vinkius.com/en/apps/linear-mcp) |
| [jira-cloud-mcp](https://vinkius.com/en/apps/jira-cloud-mcp) | Jira tickets, sprints, boards, epics | [Deploy →](https://vinkius.com/en/apps/jira-cloud-mcp) |
| [sentry-mcp](https://vinkius.com/en/apps/sentry-mcp) | Error tracking — query exceptions, stack traces, trends | [Deploy →](https://vinkius.com/en/apps/sentry-mcp) |
| [figma-mcp](https://vinkius.com/en/apps/figma-mcp) | Design files — read components, tokens, layouts | [Deploy →](https://vinkius.com/en/apps/figma-mcp) |
| [postman-mcp](https://vinkius.com/en/apps/postman-mcp) | API collections — test endpoints, import schemas | [Deploy →](https://vinkius.com/en/apps/postman-mcp) |
| [npm-registry-mcp](https://vinkius.com/en/apps/npm-registry-mcp) | npm packages — search, versions, dependencies | [Deploy →](https://vinkius.com/en/apps/npm-registry-mcp) |
| [sonarqube-mcp](https://vinkius.com/en/apps/sonarqube-mcp) | Code quality — bugs, vulnerabilities, code smells | [Deploy →](https://vinkius.com/en/apps/sonarqube-mcp) |

**Recommended setup:** GitHub + Linear + Sentry. Covers repos, tasks, and errors.

---

## Database Access

Let Claude Code query your databases directly.

| Plugin | What It Does | Deploy |
|---|---|---|
| [postgresql-mcp](https://vinkius.com/en/apps/postgresql-mcp) | PostgreSQL — run queries, inspect schemas, manage migrations | [Deploy →](https://vinkius.com/en/apps/postgresql-mcp) |
| [mysql-mcp](https://vinkius.com/en/apps/mysql-mcp) | MySQL — query, schema inspection, data analysis | [Deploy →](https://vinkius.com/en/apps/mysql-mcp) |
| [mongodb-mcp](https://vinkius.com/en/apps/mongodb-mcp) | MongoDB — documents, aggregations, indexes | [Deploy →](https://vinkius.com/en/apps/mongodb-mcp) |
| [redis-mcp](https://vinkius.com/en/apps/redis-mcp) | Redis — key-value operations, caching, pub/sub | [Deploy →](https://vinkius.com/en/apps/redis-mcp) |
| [supabase-mcp](https://vinkius.com/en/apps/supabase-mcp) | Supabase — PostgreSQL, auth, storage, realtime | [Deploy →](https://vinkius.com/en/apps/supabase-mcp) |
| [airtable-mcp](https://vinkius.com/en/apps/airtable-mcp) | Airtable — spreadsheet-database hybrid | [Deploy →](https://vinkius.com/en/apps/airtable-mcp) |
| [snowflake-mcp](https://vinkius.com/en/apps/snowflake-mcp) | Snowflake — data warehouse queries | [Deploy →](https://vinkius.com/en/apps/snowflake-mcp) |
| [bigquery-mcp](https://vinkius.com/en/apps/bigquery-mcp) | BigQuery — serverless SQL analytics | [Deploy →](https://vinkius.com/en/apps/bigquery-mcp) |

---

## Cloud and Infrastructure

Manage your cloud resources from Claude Code.

| Plugin | What It Does | Deploy |
|---|---|---|
| [aws-s3-mcp](https://vinkius.com/en/apps/aws-s3-mcp) | AWS S3 — buckets, objects, presigned URLs | [Deploy →](https://vinkius.com/en/apps/aws-s3-mcp) |
| [cloudflare-mcp](https://vinkius.com/en/apps/cloudflare-mcp) | Cloudflare — DNS, Workers, R2, Pages | [Deploy →](https://vinkius.com/en/apps/cloudflare-mcp) |
| [vercel-mcp](https://vinkius.com/en/apps/vercel-mcp) | Vercel — deployments, domains, environment variables | [Deploy →](https://vinkius.com/en/apps/vercel-mcp) |
| [terraform-mcp](https://vinkius.com/en/apps/terraform-mcp) | Terraform — infrastructure as code operations | [Deploy →](https://vinkius.com/en/apps/terraform-mcp) |
| [docker-hub-mcp](https://vinkius.com/en/apps/docker-hub-mcp) | Docker Hub — images, tags, vulnerabilities | [Deploy →](https://vinkius.com/en/apps/docker-hub-mcp) |

---

## Communication

Send messages and manage conversations from Claude Code.

| Plugin | What It Does | Deploy |
|---|---|---|
| [slack-mcp](https://vinkius.com/en/apps/slack-mcp) | Slack — messages, channels, search, reactions | [Deploy →](https://vinkius.com/en/apps/slack-mcp) |
| [discord-mcp](https://vinkius.com/en/apps/discord-mcp) | Discord — servers, channels, messages | [Deploy →](https://vinkius.com/en/apps/discord-mcp) |
| [telegram-mcp](https://vinkius.com/en/apps/telegram-mcp) | Telegram — messages, bots, groups | [Deploy →](https://vinkius.com/en/apps/telegram-mcp) |

---

## CRM and Sales

Access customer and lead data from Claude Code.

| Plugin | What It Does | Deploy |
|---|---|---|
| [hubspot-crm-full-mcp](https://vinkius.com/en/apps/hubspot-crm-full-mcp) | HubSpot — contacts, deals, companies, pipelines | [Deploy →](https://vinkius.com/en/apps/hubspot-crm-full-mcp) |
| [salesforce-mcp](https://vinkius.com/en/apps/salesforce-mcp) | Salesforce — leads, opportunities, reports | [Deploy →](https://vinkius.com/en/apps/salesforce-mcp) |
| [pipedrive-crm-full-mcp](https://vinkius.com/en/apps/pipedrive-crm-full-mcp) | Pipedrive — deals, contacts, activities | [Deploy →](https://vinkius.com/en/apps/pipedrive-crm-full-mcp) |

---

## Analytics and Monitoring

Monitor your applications and infrastructure.

| Plugin | What It Does | Deploy |
|---|---|---|
| [datadog-mcp](https://vinkius.com/en/apps/datadog-mcp) | Datadog — metrics, logs, traces, dashboards | [Deploy →](https://vinkius.com/en/apps/datadog-mcp) |
| [google-analytics-mcp](https://vinkius.com/en/apps/google-analytics-mcp) | Google Analytics — traffic, events, audiences | [Deploy →](https://vinkius.com/en/apps/google-analytics-mcp) |
| [posthog-mcp](https://vinkius.com/en/apps/posthog-mcp) | PostHog — events, feature flags, session replay | [Deploy →](https://vinkius.com/en/apps/posthog-mcp) |
| [mixpanel-mcp](https://vinkius.com/en/apps/mixpanel-mcp) | Mixpanel — events, funnels, cohorts | [Deploy →](https://vinkius.com/en/apps/mixpanel-mcp) |
| [pagerduty-mcp](https://vinkius.com/en/apps/pagerduty-mcp) | PagerDuty — incidents, schedules, escalations | [Deploy →](https://vinkius.com/en/apps/pagerduty-mcp) |

---

## AI and Search

Extend Claude Code with external AI capabilities and web search.

| Plugin | What It Does | Deploy |
|---|---|---|
| [exa-ai-mcp](https://vinkius.com/en/apps/exa-ai-mcp) | Exa — neural web search purpose-built for AI | [Deploy →](https://vinkius.com/en/apps/exa-ai-mcp) |
| [openai-mcp](https://vinkius.com/en/apps/openai-mcp) | OpenAI — GPT, DALL-E, Whisper, embeddings | [Deploy →](https://vinkius.com/en/apps/openai-mcp) |
| [firecrawl-mcp](https://vinkius.com/en/apps/firecrawl-mcp) | Firecrawl — scrape any page to clean markdown | [Deploy →](https://vinkius.com/en/apps/firecrawl-mcp) |
| [serper-mcp](https://vinkius.com/en/apps/serper-mcp) | Serper — Google SERP results API | [Deploy →](https://vinkius.com/en/apps/serper-mcp) |
| [perplexity-mcp](https://vinkius.com/en/apps/perplexity-mcp) | Perplexity — AI-powered web research | [Deploy →](https://vinkius.com/en/apps/perplexity-mcp) |

---

## Finance and Payments

Query financial data and manage payments.

| Plugin | What It Does | Deploy |
|---|---|---|
| [stripe-mcp](https://vinkius.com/en/apps/stripe-mcp) | Stripe — payments, subscriptions, invoices | [Deploy →](https://vinkius.com/en/apps/stripe-mcp) |
| [quickbooks-mcp](https://vinkius.com/en/apps/quickbooks-mcp) | QuickBooks — accounting, reconciliation | [Deploy →](https://vinkius.com/en/apps/quickbooks-mcp) |
| [plaid-mcp](https://vinkius.com/en/apps/plaid-mcp) | Plaid — bank connections, transactions | [Deploy →](https://vinkius.com/en/apps/plaid-mcp) |

---

## Design and Media

Connect design and media tools to Claude Code.

| Plugin | What It Does | Deploy |
|---|---|---|
| [figma-mcp](https://vinkius.com/en/apps/figma-mcp) | Figma — design files, components, auto-layout | [Deploy →](https://vinkius.com/en/apps/figma-mcp) |
| [cloudinary-mcp](https://vinkius.com/en/apps/cloudinary-mcp) | Cloudinary — image/video upload, transform, optimize | [Deploy →](https://vinkius.com/en/apps/cloudinary-mcp) |
| [unsplash-mcp](https://vinkius.com/en/apps/unsplash-mcp) | Unsplash — search and download stock photos | [Deploy →](https://vinkius.com/en/apps/unsplash-mcp) |

---

## How to Install a Plugin

### Step 1: Deploy the MCP server

Go to [vinkius.com](https://vinkius.com), find the server, and deploy it. You receive an SSE endpoint URL:

```
https://edge.vinkius.com/vk_live_xxxxxxxxxxxx/mcp
```

### Step 2: Add to `.mcp.json`

Create or edit `.mcp.json` in your project root:

```json
{
  "mcpServers": {
    "memory": { "url": "https://edge.vinkius.com/vk_live_xxxxxxxxxxxx/mcp" }
  }
}
```

### Step 3: Start Claude Code

```bash
claude
/mcp  # verify the plugin is connected
```

Claude Code automatically discovers and uses every connected server.

---

## How to Create Your Own Plugin

Any MCP server is a Claude Code plugin. Build one with the [Vinkius SDK](https://vinkius.com):

```typescript
import { McpServer } from "@vinkius/vurb";

const server = new McpServer({ name: "my-plugin", version: "1.0.0" });

server.tool("greet", { name: "string" }, async ({ name }) => {
  return { content: [{ type: "text", text: `Hello, ${name}!` }] };
});

server.start();
```

Deploy to the [Vinkius AI Gateway](https://vinkius.com) and share the SSE URL with anyone.

---

## All Plugins

This page lists the most popular plugins. The [Vinkius AI Gateway](https://vinkius.com) offers **2,600+ MCP servers** that work as Claude Code plugins.

Browse the full catalog: [vinkius.com/en/categories](https://vinkius.com/en/categories)

---

## License

MIT — [Vinkius Labs](https://vinkius.com)
