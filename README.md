# Claude Code Plugins

A curated directory of plugins, skills, and MCP integrations for [Claude Code](https://claude.ai/code). Extend your AI coding assistant with persistent memory, live data access, and production-grade developer workflows.

Claude Code is the most powerful agentic coding tool available. These plugins make it unstoppable.

[![Plugins](https://img.shields.io/badge/Plugins-340%2B-brightgreen)](https://vinkius.com)
[![Total Available](https://img.shields.io/badge/Total_Available-2%2C600%2B-blue)](https://vinkius.com/en/categories)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## Contents

- [Getting Started](#getting-started)
- [Memory and Context](#memory-and-context)
- [AI and LLM Providers](#ai-and-llm-providers)
- [Developer Productivity](#developer-productivity)
- [Database Access](#database-access)
- [Cloud and Infrastructure](#cloud-and-infrastructure)
- [DevOps and CI/CD](#devops-and-cicd)
- [Communication](#communication)
- [CRM and Sales](#crm-and-sales)
- [Marketing and Email](#marketing-and-email)
- [Advertising Platforms](#advertising-platforms)
- [Analytics and Customer Data](#analytics-and-customer-data)
- [Monitoring and Observability](#monitoring-and-observability)
- [Security and Compliance](#security-and-compliance)
- [Finance and Payments](#finance-and-payments)
- [E-commerce](#e-commerce)
- [Customer Support](#customer-support)
- [Project Management](#project-management)
- [Productivity and Documents](#productivity-and-documents)
- [Design and Media](#design-and-media)
- [Video and Audio](#video-and-audio)
- [Social Media](#social-media)
- [Search and Web Scraping](#search-and-web-scraping)
- [File Storage](#file-storage)
- [Calendar and Scheduling](#calendar-and-scheduling)
- [Forms and Surveys](#forms-and-surveys)
- [Signatures and Documents](#signatures-and-documents)
- [Translation](#translation)
- [SMS and Notifications](#sms-and-notifications)
- [Telephony and VoIP](#telephony-and-voip)
- [ERP and Business Operations](#erp-and-business-operations)
- [HR and Recruiting](#hr-and-recruiting)
- [Legal and Compliance](#legal-and-compliance)
- [Real Estate](#real-estate)
- [Logistics and Shipping](#logistics-and-shipping)
- [Events and Webinars](#events-and-webinars)
- [Automation Platforms](#automation-platforms)
- [Crypto and Blockchain](#crypto-and-blockchain)
- [Stock Market and Fintech](#stock-market-and-fintech)
- [Government Data](#government-data)
- [NASA and Space](#nasa-and-space)
- [Weather and Climate](#weather-and-climate)
- [Healthcare and Public Health](#healthcare-and-public-health)
- [Gaming and Esports](#gaming-and-esports)
- [Music and Audio Platforms](#music-and-audio-platforms)
- [Sports and Fitness](#sports-and-fitness)
- [Food and Restaurants](#food-and-restaurants)
- [Education](#education)
- [IoT and Smart Home](#iot-and-smart-home)
- [Secrets Management](#secrets-management)
- [Testing and QA](#testing-and-qa)
- [How to Install a Plugin](#how-to-install-a-plugin)

---

## Getting Started

Claude Code loads MCP servers from a `.mcp.json` file in your project root. Each entry is a plugin — a live connection to an external tool.

```bash
# Add memory to Claude Code in 10 seconds
echo '{"mcpServers":{"memory":{"url":"YOUR_MEM0_URL"}}}' > .mcp.json
claude
/mcp  # verify connection
```

All plugins below are available as managed MCP servers on the [Vinkius AI Gateway](https://vinkius.com) — deploy in one click, get an SSE endpoint URL, paste it into your `.mcp.json`.

---

## Memory and Context

Give Claude Code long-term memory across sessions.

| Plugin | What It Does | Deploy |
|---|---|---|
| [Mem0](https://vinkius.com/en/apps/mem0-mcp) | Persistent memory — store and recall learnings, decisions, preferences | [Deploy →](https://vinkius.com/en/apps/mem0-mcp) |
| [Context7](https://vinkius.com/en/apps/context7-mcp) | Session context management — carry context between conversations | [Deploy →](https://vinkius.com/en/apps/context7-mcp) |
| [Qdrant](https://vinkius.com/en/apps/qdrant-mcp) | Vector search — semantic retrieval of past code and docs | [Deploy →](https://vinkius.com/en/apps/qdrant-mcp) |
| [Pinecone](https://vinkius.com/en/apps/pinecone-mcp) | Managed vector database — high-performance similarity search | [Deploy →](https://vinkius.com/en/apps/pinecone-mcp) |
| [Chroma](https://vinkius.com/en/apps/chroma-vector-db-mcp) | Local-first vector DB — lightweight embedding storage | [Deploy →](https://vinkius.com/en/apps/chroma-vector-db-mcp) |

**Recommendation:** Start with **Mem0** for general memory. Add **Qdrant** for semantic code search.

---

## AI and LLM Providers

Connect Claude Code to other AI models and services.

| Plugin | What It Does | Deploy |
|---|---|---|
| [OpenAI](https://vinkius.com/en/apps/openai-mcp) | GPT, DALL-E, Whisper, embeddings | [Deploy →](https://vinkius.com/en/apps/openai-mcp) |
| [Anthropic](https://vinkius.com/en/apps/anthropic-mcp) | Claude models API access | [Deploy →](https://vinkius.com/en/apps/anthropic-mcp) |
| [Mistral AI](https://vinkius.com/en/apps/mistral-ai-mcp) | Frontier LLMs and embeddings | [Deploy →](https://vinkius.com/en/apps/mistral-ai-mcp) |
| [Groq](https://vinkius.com/en/apps/groq-mcp) | Ultra-fast inference | [Deploy →](https://vinkius.com/en/apps/groq-mcp) |
| [Cohere](https://vinkius.com/en/apps/cohere-mcp) | AI platform, embed, rerank | [Deploy →](https://vinkius.com/en/apps/cohere-mcp) |
| [Together AI](https://vinkius.com/en/apps/together-ai-mcp) | Open-source model inference | [Deploy →](https://vinkius.com/en/apps/together-ai-mcp) |
| [Replicate](https://vinkius.com/en/apps/replicate-mcp) | Run any ML model via API | [Deploy →](https://vinkius.com/en/apps/replicate-mcp) |
| [Hugging Face](https://vinkius.com/en/apps/hugging-face-mcp) | Models, datasets, inference | [Deploy →](https://vinkius.com/en/apps/hugging-face-mcp) |
| [Hugging Face Audio](https://vinkius.com/en/apps/hugging-face-audio-mcp) | Speech and audio models | [Deploy →](https://vinkius.com/en/apps/hugging-face-audio-mcp) |
| [Hugging Face Vision](https://vinkius.com/en/apps/hugging-face-vision-mcp) | Image and vision models | [Deploy →](https://vinkius.com/en/apps/hugging-face-vision-mcp) |
| [Fireworks AI](https://vinkius.com/en/apps/fireworks-ai-mcp) | Fast inference for open models | [Deploy →](https://vinkius.com/en/apps/fireworks-ai-mcp) |
| [Perplexity AI](https://vinkius.com/en/apps/perplexity-ai-mcp) | AI-powered web research | [Deploy →](https://vinkius.com/en/apps/perplexity-ai-mcp) |
| [Cohere Embed](https://vinkius.com/en/apps/cohere-embed-rerank-mcp) | Embedding and reranking | [Deploy →](https://vinkius.com/en/apps/cohere-embed-rerank-mcp) |
| [Anyscale](https://vinkius.com/en/apps/anyscale-mcp) | Scalable AI endpoints | [Deploy →](https://vinkius.com/en/apps/anyscale-mcp) |

---

## Developer Productivity

Connect Claude Code to your development workflow.

| Plugin | What It Does | Deploy |
|---|---|---|
| [GitHub](https://vinkius.com/en/apps/github-mcp) | Repos, issues, PRs, Actions, code search | [Deploy →](https://vinkius.com/en/apps/github-mcp) |
| [GitLab](https://vinkius.com/en/apps/gitlab-mcp) | Repos, CI/CD, merge requests | [Deploy →](https://vinkius.com/en/apps/gitlab-mcp) |
| [Linear](https://vinkius.com/en/apps/linear-mcp) | Issues, projects, cycles | [Deploy →](https://vinkius.com/en/apps/linear-mcp) |
| [Jira Cloud](https://vinkius.com/en/apps/jira-cloud-mcp) | Tickets, sprints, boards, epics | [Deploy →](https://vinkius.com/en/apps/jira-cloud-mcp) |
| [Jira Service Management](https://vinkius.com/en/apps/jira-service-management-jsm-mcp) | IT service desk and ITSM | [Deploy →](https://vinkius.com/en/apps/jira-service-management-jsm-mcp) |
| [Sentry](https://vinkius.com/en/apps/sentry-mcp) | Error tracking, crash reporting | [Deploy →](https://vinkius.com/en/apps/sentry-mcp) |
| [Figma](https://vinkius.com/en/apps/figma-mcp) | Design files, components, tokens | [Deploy →](https://vinkius.com/en/apps/figma-mcp) |
| [Postman](https://vinkius.com/en/apps/postman-mcp) | API collections, test endpoints | [Deploy →](https://vinkius.com/en/apps/postman-mcp) |
| [npm Registry](https://vinkius.com/en/apps/npm-registry-mcp) | Package search, versions, deps | [Deploy →](https://vinkius.com/en/apps/npm-registry-mcp) |
| [SonarQube](https://vinkius.com/en/apps/sonarqube-sonarcloud-mcp) | Code quality, bugs, vulnerabilities | [Deploy →](https://vinkius.com/en/apps/sonarqube-sonarcloud-mcp) |
| [Shortcut](https://vinkius.com/en/apps/shortcut-mcp) | Project management for software teams | [Deploy →](https://vinkius.com/en/apps/shortcut-mcp) |
| [Plane](https://vinkius.com/en/apps/plane-mcp) | Open-source project management | [Deploy →](https://vinkius.com/en/apps/plane-mcp) |
| [ZenHub](https://vinkius.com/en/apps/zenhub-mcp) | Agile project management for GitHub | [Deploy →](https://vinkius.com/en/apps/zenhub-mcp) |
| [Height](https://vinkius.com/en/apps/height-project-management-mcp) | AI-native project management | [Deploy →](https://vinkius.com/en/apps/height-project-management-mcp) |

---

## Database Access

Let Claude Code query your databases directly.

| Plugin | What It Does | Deploy |
|---|---|---|
| [PostgreSQL](https://vinkius.com/en/apps/postgresql-mcp) | SQL queries, schema, migrations | [Deploy →](https://vinkius.com/en/apps/postgresql-mcp) |
| [MySQL](https://vinkius.com/en/apps/mysql-mcp) | SQL queries, schema inspection | [Deploy →](https://vinkius.com/en/apps/mysql-mcp) |
| [MongoDB](https://vinkius.com/en/apps/mongodb-mcp) | Documents, aggregations, indexes | [Deploy →](https://vinkius.com/en/apps/mongodb-mcp) |
| [Redis](https://vinkius.com/en/apps/redis-mcp) | Key-value, caching, pub/sub | [Deploy →](https://vinkius.com/en/apps/redis-mcp) |
| [Supabase](https://vinkius.com/en/apps/supabase-mcp) | PostgreSQL + Auth + Storage + Realtime | [Deploy →](https://vinkius.com/en/apps/supabase-mcp) |
| [PlanetScale](https://vinkius.com/en/apps/planetscale-mcp) | Serverless MySQL | [Deploy →](https://vinkius.com/en/apps/planetscale-mcp) |
| [Airtable](https://vinkius.com/en/apps/airtable-mcp) | Spreadsheet-database hybrid | [Deploy →](https://vinkius.com/en/apps/airtable-mcp) |
| [Snowflake](https://vinkius.com/en/apps/snowflake-mcp) | Cloud data warehouse | [Deploy →](https://vinkius.com/en/apps/snowflake-mcp) |
| [BigQuery](https://vinkius.com/en/apps/bigquery-mcp) | Serverless SQL analytics | [Deploy →](https://vinkius.com/en/apps/bigquery-mcp) |

---

## Cloud and Infrastructure

| Plugin | What It Does | Deploy |
|---|---|---|
| [AWS S3](https://vinkius.com/en/apps/aws-s3-mcp) | Buckets, objects, presigned URLs | [Deploy →](https://vinkius.com/en/apps/aws-s3-mcp) |
| [Cloudflare](https://vinkius.com/en/apps/cloudflare-mcp) | DNS, Workers, R2, Pages | [Deploy →](https://vinkius.com/en/apps/cloudflare-mcp) |
| [Vercel](https://vinkius.com/en/apps/vercel-mcp) | Deployments, domains, env vars | [Deploy →](https://vinkius.com/en/apps/vercel-mcp) |
| [Terraform](https://vinkius.com/en/apps/terraform-mcp) | Infrastructure as code | [Deploy →](https://vinkius.com/en/apps/terraform-mcp) |
| [Pulumi](https://vinkius.com/en/apps/pulumi-mcp) | IaC with real programming languages | [Deploy →](https://vinkius.com/en/apps/pulumi-mcp) |
| [Docker Hub](https://vinkius.com/en/apps/docker-hub-mcp) | Images, tags, vulnerabilities | [Deploy →](https://vinkius.com/en/apps/docker-hub-mcp) |
| [Kong](https://vinkius.com/en/apps/kong-ai-api-gateway-mcp) | AI API gateway | [Deploy →](https://vinkius.com/en/apps/kong-ai-api-gateway-mcp) |
| [Traefik Hub](https://vinkius.com/en/apps/traefik-hub-mcp) | Cloud-native API gateway | [Deploy →](https://vinkius.com/en/apps/traefik-hub-mcp) |

---

## DevOps and CI/CD

| Plugin | What It Does | Deploy |
|---|---|---|
| [CircleCI](https://vinkius.com/en/apps/circleci-mcp) | CI/CD pipelines and workflows | [Deploy →](https://vinkius.com/en/apps/circleci-mcp) |
| [Grafana](https://vinkius.com/en/apps/grafana-mcp) | Dashboards, metrics visualization | [Deploy →](https://vinkius.com/en/apps/grafana-mcp) |
| [Grafana k6](https://vinkius.com/en/apps/grafana-k6-cloud-load-testing-mcp) | Cloud load testing | [Deploy →](https://vinkius.com/en/apps/grafana-k6-cloud-load-testing-mcp) |
| [Envoy](https://vinkius.com/en/apps/envoy-mcp) | Service mesh proxy | [Deploy →](https://vinkius.com/en/apps/envoy-mcp) |

---

## Communication

| Plugin | What It Does | Deploy |
|---|---|---|
| [Slack](https://vinkius.com/en/apps/slack-mcp) | Messages, channels, search | [Deploy →](https://vinkius.com/en/apps/slack-mcp) |
| [Discord](https://vinkius.com/en/apps/discord-mcp) | Servers, channels, messages | [Deploy →](https://vinkius.com/en/apps/discord-mcp) |
| [Telegram](https://vinkius.com/en/apps/telegram-mcp) | Messages, bots, groups | [Deploy →](https://vinkius.com/en/apps/telegram-mcp) |
| [Microsoft Teams](https://vinkius.com/en/apps/microsoft-teams-mcp) | Chat, channels, meetings | [Deploy →](https://vinkius.com/en/apps/microsoft-teams-mcp) |
| [WeCom](https://vinkius.com/en/apps/wecom-mcp) | Enterprise WeChat | [Deploy →](https://vinkius.com/en/apps/wecom-mcp) |
| [DingTalk](https://vinkius.com/en/apps/dingtalk-mcp) | Alibaba enterprise messaging | [Deploy →](https://vinkius.com/en/apps/dingtalk-mcp) |

---

## CRM and Sales

| Plugin | What It Does | Deploy |
|---|---|---|
| [HubSpot CRM](https://vinkius.com/en/apps/hubspot-crm-full-mcp) | Contacts, deals, companies, pipelines | [Deploy →](https://vinkius.com/en/apps/hubspot-crm-full-mcp) |
| [HubSpot Sales Hub](https://vinkius.com/en/apps/hubspot-sales-hub-mcp) | Sequences, meetings, quotes | [Deploy →](https://vinkius.com/en/apps/hubspot-sales-hub-mcp) |
| [HubSpot Marketing Hub](https://vinkius.com/en/apps/hubspot-marketing-hub-mcp) | Campaigns, landing pages, forms | [Deploy →](https://vinkius.com/en/apps/hubspot-marketing-hub-mcp) |
| [HubSpot Service Hub](https://vinkius.com/en/apps/hubspot-service-hub-mcp) | Tickets, knowledge base | [Deploy →](https://vinkius.com/en/apps/hubspot-service-hub-mcp) |
| [HubSpot Analytics](https://vinkius.com/en/apps/hubspot-analytics-mcp) | Reports, dashboards | [Deploy →](https://vinkius.com/en/apps/hubspot-analytics-mcp) |
| [Salesforce](https://vinkius.com/en/apps/salesforce-mcp) | Leads, opportunities, reports | [Deploy →](https://vinkius.com/en/apps/salesforce-mcp) |
| [Pipedrive](https://vinkius.com/en/apps/pipedrive-crm-full-mcp) | Deals, contacts, activities | [Deploy →](https://vinkius.com/en/apps/pipedrive-crm-full-mcp) |
| [Zoho CRM](https://vinkius.com/en/apps/zoho-crm-full-mcp) | Complete CRM platform | [Deploy →](https://vinkius.com/en/apps/zoho-crm-full-mcp) |
| [Zoho CRM Sales](https://vinkius.com/en/apps/zoho-crm-sales-mcp) | Sales pipeline focus | [Deploy →](https://vinkius.com/en/apps/zoho-crm-sales-mcp) |
| [Zoho CRM Contacts](https://vinkius.com/en/apps/zoho-crm-contacts-mcp) | Contact management | [Deploy →](https://vinkius.com/en/apps/zoho-crm-contacts-mcp) |
| [Zoho CRM Analytics](https://vinkius.com/en/apps/zoho-crm-analytics-mcp) | CRM analytics and reports | [Deploy →](https://vinkius.com/en/apps/zoho-crm-analytics-mcp) |
| [Monday.com](https://vinkius.com/en/apps/mondaycom-work-management-crm-mcp) | Work management and CRM | [Deploy →](https://vinkius.com/en/apps/mondaycom-work-management-crm-mcp) |
| [Apollo.io](https://vinkius.com/en/apps/apolloio-mcp) | Sales intelligence, prospecting | [Deploy →](https://vinkius.com/en/apps/apolloio-mcp) |
| [Hunter](https://vinkius.com/en/apps/hunter-mcp) | Email finder and verification | [Deploy →](https://vinkius.com/en/apps/hunter-mcp) |
| [Clearbit](https://vinkius.com/en/apps/clearbit-hubspot-mcp) | Company and contact enrichment | [Deploy →](https://vinkius.com/en/apps/clearbit-hubspot-mcp) |
| [Microsoft Dynamics 365](https://vinkius.com/en/apps/microsoft-dynamics-365-mcp) | Enterprise CRM and ERP | [Deploy →](https://vinkius.com/en/apps/microsoft-dynamics-365-mcp) |

---

## Marketing and Email

| Plugin | What It Does | Deploy |
|---|---|---|
| [Mailchimp](https://vinkius.com/en/apps/mailchimp-mcp) | Campaign management, audiences | [Deploy →](https://vinkius.com/en/apps/mailchimp-mcp) |
| [SendGrid](https://vinkius.com/en/apps/twilio-sendgrid-mcp) | Transactional and marketing email | [Deploy →](https://vinkius.com/en/apps/twilio-sendgrid-mcp) |
| [Klaviyo](https://vinkius.com/en/apps/klaviyo-marketing-automation-mcp) | E-commerce email automation | [Deploy →](https://vinkius.com/en/apps/klaviyo-marketing-automation-mcp) |
| [ActiveCampaign](https://vinkius.com/en/apps/activecampaign-mcp) | Email + CRM automation | [Deploy →](https://vinkius.com/en/apps/activecampaign-mcp) |
| [ConvertKit](https://vinkius.com/en/apps/kit-convertkit-mcp) | Creator-focused email | [Deploy →](https://vinkius.com/en/apps/kit-convertkit-mcp) |
| [Brevo](https://vinkius.com/en/apps/brevo-mcp) | Email, SMS, chat marketing | [Deploy →](https://vinkius.com/en/apps/brevo-mcp) |
| [MailerLite](https://vinkius.com/en/apps/mailerlite-mcp) | Email marketing | [Deploy →](https://vinkius.com/en/apps/mailerlite-mcp) |
| [Mailgun](https://vinkius.com/en/apps/mailgun-transactional-email-domains-mcp) | Transactional email API | [Deploy →](https://vinkius.com/en/apps/mailgun-transactional-email-domains-mcp) |
| [Postmark](https://vinkius.com/en/apps/postmark-mcp) | Fast transactional email | [Deploy →](https://vinkius.com/en/apps/postmark-mcp) |
| [Resend](https://vinkius.com/en/apps/resend-mcp) | Modern email API for developers | [Deploy →](https://vinkius.com/en/apps/resend-mcp) |
| [Mailjet](https://vinkius.com/en/apps/mailjet-mcp) | Collaborative email platform | [Deploy →](https://vinkius.com/en/apps/mailjet-mcp) |
| [SparkPost](https://vinkius.com/en/apps/sparkpost-mcp) | Enterprise email delivery | [Deploy →](https://vinkius.com/en/apps/sparkpost-mcp) |
| [Drip](https://vinkius.com/en/apps/drip-mcp) | E-commerce CRM | [Deploy →](https://vinkius.com/en/apps/drip-mcp) |
| [Constant Contact](https://vinkius.com/en/apps/constant-contact-mcp) | Email marketing for SMBs | [Deploy →](https://vinkius.com/en/apps/constant-contact-mcp) |
| [Beehiiv](https://vinkius.com/en/apps/beehiiv-mcp) | Newsletter platform | [Deploy →](https://vinkius.com/en/apps/beehiiv-mcp) |
| [Substack](https://vinkius.com/en/apps/substack-mcp) | Newsletter and publishing | [Deploy →](https://vinkius.com/en/apps/substack-mcp) |
| [Marketo](https://vinkius.com/en/apps/marketo-mcp) | Enterprise marketing automation | [Deploy →](https://vinkius.com/en/apps/marketo-mcp) |
| [Buffer](https://vinkius.com/en/apps/buffer-mcp) | Social media scheduling | [Deploy →](https://vinkius.com/en/apps/buffer-mcp) |
| [Hootsuite](https://vinkius.com/en/apps/hootsuite-social-media-management-mcp) | Social media management | [Deploy →](https://vinkius.com/en/apps/hootsuite-social-media-management-mcp) |
| [Sprout Social](https://vinkius.com/en/apps/sprout-social-mcp) | Social media analytics | [Deploy →](https://vinkius.com/en/apps/sprout-social-mcp) |

---

## Advertising Platforms

| Plugin | What It Does | Deploy |
|---|---|---|
| [Google Ads](https://vinkius.com/en/apps/google-ads-mcp) | Search, display, video campaigns | [Deploy →](https://vinkius.com/en/apps/google-ads-mcp) |
| [Facebook Ads](https://vinkius.com/en/apps/facebook-ads-mcp) | Meta advertising platform | [Deploy →](https://vinkius.com/en/apps/facebook-ads-mcp) |
| [TikTok Ads](https://vinkius.com/en/apps/tiktok-ads-mcp) | TikTok advertising | [Deploy →](https://vinkius.com/en/apps/tiktok-ads-mcp) |
| [LinkedIn Ads](https://vinkius.com/en/apps/linkedin-ads-mcp) | B2B advertising | [Deploy →](https://vinkius.com/en/apps/linkedin-ads-mcp) |
| [Pinterest Ads](https://vinkius.com/en/apps/pinterest-ads-mcp) | Visual discovery advertising | [Deploy →](https://vinkius.com/en/apps/pinterest-ads-mcp) |
| [Reddit Ads](https://vinkius.com/en/apps/reddit-ads-mcp) | Community-based advertising | [Deploy →](https://vinkius.com/en/apps/reddit-ads-mcp) |
| [X/Twitter Ads](https://vinkius.com/en/apps/x-ads-twitter-mcp) | Twitter advertising platform | [Deploy →](https://vinkius.com/en/apps/x-ads-twitter-mcp) |
| [Snapchat Ads](https://vinkius.com/en/apps/snapchat-ads-mcp) | Snapchat advertising | [Deploy →](https://vinkius.com/en/apps/snapchat-ads-mcp) |
| [Microsoft Ads](https://vinkius.com/en/apps/microsoft-ads-mcp) | Bing search advertising | [Deploy →](https://vinkius.com/en/apps/microsoft-ads-mcp) |
| [Amazon Ads](https://vinkius.com/en/apps/amazon-ads-mcp) | Amazon PPC advertising | [Deploy →](https://vinkius.com/en/apps/amazon-ads-mcp) |

---

## Analytics and Customer Data

| Plugin | What It Does | Deploy |
|---|---|---|
| [Google Analytics](https://vinkius.com/en/apps/google-analytics-mcp) | Traffic, events, audiences | [Deploy →](https://vinkius.com/en/apps/google-analytics-mcp) |
| [Mixpanel](https://vinkius.com/en/apps/mixpanel-mcp) | Product analytics, funnels | [Deploy →](https://vinkius.com/en/apps/mixpanel-mcp) |
| [PostHog](https://vinkius.com/en/apps/posthog-mcp) | Events, feature flags, session replay | [Deploy →](https://vinkius.com/en/apps/posthog-mcp) |
| [Amplitude](https://vinkius.com/en/apps/amplitude-mcp) | Product intelligence | [Deploy →](https://vinkius.com/en/apps/amplitude-mcp) |
| [Segment](https://vinkius.com/en/apps/segment-mcp) | Customer data platform | [Deploy →](https://vinkius.com/en/apps/segment-mcp) |
| [Heap](https://vinkius.com/en/apps/heap-mcp) | Auto-capture analytics | [Deploy →](https://vinkius.com/en/apps/heap-mcp) |
| [FullStory](https://vinkius.com/en/apps/fullstory-mcp) | Digital experience analytics | [Deploy →](https://vinkius.com/en/apps/fullstory-mcp) |
| [Hotjar](https://vinkius.com/en/apps/hotjar-behavior-analytics-mcp) | Heatmaps and behavior analytics | [Deploy →](https://vinkius.com/en/apps/hotjar-behavior-analytics-mcp) |
| [RudderStack](https://vinkius.com/en/apps/rudderstack-mcp) | Open-source customer data pipeline | [Deploy →](https://vinkius.com/en/apps/rudderstack-mcp) |
| [SimilarWeb](https://vinkius.com/en/apps/similarweb-analytics-mcp) | Website traffic intelligence | [Deploy →](https://vinkius.com/en/apps/similarweb-analytics-mcp) |

---

## Monitoring and Observability

| Plugin | What It Does | Deploy |
|---|---|---|
| [Datadog](https://vinkius.com/en/apps/datadog-mcp) | Metrics, logs, traces, APM | [Deploy →](https://vinkius.com/en/apps/datadog-mcp) |
| [PagerDuty](https://vinkius.com/en/apps/pagerduty-mcp) | Incidents, schedules, escalations | [Deploy →](https://vinkius.com/en/apps/pagerduty-mcp) |
| [Grafana](https://vinkius.com/en/apps/grafana-mcp) | Dashboards and visualization | [Deploy →](https://vinkius.com/en/apps/grafana-mcp) |

---

## Security and Compliance

| Plugin | What It Does | Deploy |
|---|---|---|
| [Snyk](https://vinkius.com/en/apps/snyk-mcp) | Vulnerability scanning | [Deploy →](https://vinkius.com/en/apps/snyk-mcp) |
| [CrowdStrike Falcon](https://vinkius.com/en/apps/crowdstrike-falcon-mcp) | Endpoint security | [Deploy →](https://vinkius.com/en/apps/crowdstrike-falcon-mcp) |
| [Tenable](https://vinkius.com/en/apps/tenable-mcp) | Vulnerability management | [Deploy →](https://vinkius.com/en/apps/tenable-mcp) |
| [Semgrep](https://vinkius.com/en/apps/semgrep-mcp) | Static code analysis | [Deploy →](https://vinkius.com/en/apps/semgrep-mcp) |
| [Checkmarx](https://vinkius.com/en/apps/checkmarx-mcp) | Application security testing | [Deploy →](https://vinkius.com/en/apps/checkmarx-mcp) |
| [Veracode](https://vinkius.com/en/apps/veracode-mcp) | Software security verification | [Deploy →](https://vinkius.com/en/apps/veracode-mcp) |
| [NIST NVD](https://vinkius.com/en/apps/nist-nvd-mcp) | National vulnerability database | [Deploy →](https://vinkius.com/en/apps/nist-nvd-mcp) |

---

## Finance and Payments

| Plugin | What It Does | Deploy |
|---|---|---|
| [Stripe](https://vinkius.com/en/apps/stripe-mcp) | Payments, subscriptions, invoices | [Deploy →](https://vinkius.com/en/apps/stripe-mcp) |
| [PayPal](https://vinkius.com/en/apps/paypal-mcp) | Global payments | [Deploy →](https://vinkius.com/en/apps/paypal-mcp) |
| [QuickBooks](https://vinkius.com/en/apps/quickbooks-mcp) | Accounting and bookkeeping | [Deploy →](https://vinkius.com/en/apps/quickbooks-mcp) |
| [Xero](https://vinkius.com/en/apps/xero-mcp) | Cloud accounting | [Deploy →](https://vinkius.com/en/apps/xero-mcp) |
| [FreshBooks](https://vinkius.com/en/apps/freshbooks-mcp) | Invoicing and accounting | [Deploy →](https://vinkius.com/en/apps/freshbooks-mcp) |
| [Wave](https://vinkius.com/en/apps/wave-financial-mcp) | Free accounting software | [Deploy →](https://vinkius.com/en/apps/wave-financial-mcp) |
| [Plaid](https://vinkius.com/en/apps/plaid-mcp) | Bank connections, transactions | [Deploy →](https://vinkius.com/en/apps/plaid-mcp) |
| [Chargebee](https://vinkius.com/en/apps/chargebee-mcp) | Subscription billing | [Deploy →](https://vinkius.com/en/apps/chargebee-mcp) |
| [Paddle](https://vinkius.com/en/apps/paddle-mcp) | SaaS billing and tax | [Deploy →](https://vinkius.com/en/apps/paddle-mcp) |
| [Recurly](https://vinkius.com/en/apps/recurly-mcp) | Subscription management | [Deploy →](https://vinkius.com/en/apps/recurly-mcp) |
| [Zoho Books](https://vinkius.com/en/apps/zoho-books-mcp) | Online accounting | [Deploy →](https://vinkius.com/en/apps/zoho-books-mcp) |
| [Zoho Invoice](https://vinkius.com/en/apps/zoho-invoice-mcp) | Invoicing solution | [Deploy →](https://vinkius.com/en/apps/zoho-invoice-mcp) |

---

## E-commerce

| Plugin | What It Does | Deploy |
|---|---|---|
| [Shopify](https://vinkius.com/en/apps/shopify-mcp) | Products, orders, customers | [Deploy →](https://vinkius.com/en/apps/shopify-mcp) |
| [BigCommerce](https://vinkius.com/en/apps/bigcommerce-mcp) | Enterprise e-commerce | [Deploy →](https://vinkius.com/en/apps/bigcommerce-mcp) |
| [Magento](https://vinkius.com/en/apps/magento-adobe-commerce-mcp) | Adobe Commerce | [Deploy →](https://vinkius.com/en/apps/magento-adobe-commerce-mcp) |
| [WooCommerce](https://vinkius.com/en/apps/woocommerce-mcp) | WordPress e-commerce | [Deploy →](https://vinkius.com/en/apps/woocommerce-mcp) |
| [Squarespace](https://vinkius.com/en/apps/squarespace-commerce-mcp) | Website + store builder | [Deploy →](https://vinkius.com/en/apps/squarespace-commerce-mcp) |
| [Ecwid](https://vinkius.com/en/apps/ecwid-mcp) | Embeddable online store | [Deploy →](https://vinkius.com/en/apps/ecwid-mcp) |
| [Gumroad](https://vinkius.com/en/apps/gumroad-mcp) | Creator commerce | [Deploy →](https://vinkius.com/en/apps/gumroad-mcp) |
| [Odoo eCommerce](https://vinkius.com/en/apps/odoo-ecommerce-mcp) | Open-source e-commerce | [Deploy →](https://vinkius.com/en/apps/odoo-ecommerce-mcp) |

---

## Customer Support

| Plugin | What It Does | Deploy |
|---|---|---|
| [Zendesk](https://vinkius.com/en/apps/zendesk-mcp) | Ticketing, help desk | [Deploy →](https://vinkius.com/en/apps/zendesk-mcp) |
| [Intercom](https://vinkius.com/en/apps/intercom-mcp) | Conversational support | [Deploy →](https://vinkius.com/en/apps/intercom-mcp) |
| [Freshdesk](https://vinkius.com/en/apps/freshdesk-mcp) | Customer support platform | [Deploy →](https://vinkius.com/en/apps/freshdesk-mcp) |
| [FreshService](https://vinkius.com/en/apps/freshservice-mcp) | IT service management | [Deploy →](https://vinkius.com/en/apps/freshservice-mcp) |
| [ServiceNow](https://vinkius.com/en/apps/servicenow-mcp) | Enterprise ITSM | [Deploy →](https://vinkius.com/en/apps/servicenow-mcp) |
| [Help Scout](https://vinkius.com/en/apps/help-scout-mcp) | Shared inbox for support | [Deploy →](https://vinkius.com/en/apps/help-scout-mcp) |
| [Front](https://vinkius.com/en/apps/front-mcp) | Shared inbox collaboration | [Deploy →](https://vinkius.com/en/apps/front-mcp) |
| [Groove](https://vinkius.com/en/apps/groove-mcp) | Simple helpdesk for SMBs | [Deploy →](https://vinkius.com/en/apps/groove-mcp) |
| [Drift](https://vinkius.com/en/apps/drift-mcp) | Conversational marketing | [Deploy →](https://vinkius.com/en/apps/drift-mcp) |
| [Zoho Desk](https://vinkius.com/en/apps/zoho-desk-mcp) | Help desk software | [Deploy →](https://vinkius.com/en/apps/zoho-desk-mcp) |
| [Odoo Helpdesk](https://vinkius.com/en/apps/odoo-helpdesk-mcp) | Open-source helpdesk | [Deploy →](https://vinkius.com/en/apps/odoo-helpdesk-mcp) |

---

## Project Management

| Plugin | What It Does | Deploy |
|---|---|---|
| [Jira](https://vinkius.com/en/apps/jira-cloud-mcp) | Enterprise project management | [Deploy →](https://vinkius.com/en/apps/jira-cloud-mcp) |
| [Linear](https://vinkius.com/en/apps/linear-mcp) | Modern issue tracking | [Deploy →](https://vinkius.com/en/apps/linear-mcp) |
| [Asana](https://vinkius.com/en/apps/asana-mcp) | Work management platform | [Deploy →](https://vinkius.com/en/apps/asana-mcp) |
| [Trello](https://vinkius.com/en/apps/trello-mcp) | Kanban boards | [Deploy →](https://vinkius.com/en/apps/trello-mcp) |
| [ClickUp](https://vinkius.com/en/apps/clickup-mcp) | Productivity platform | [Deploy →](https://vinkius.com/en/apps/clickup-mcp) |
| [Basecamp](https://vinkius.com/en/apps/basecamp-mcp) | Team project management | [Deploy →](https://vinkius.com/en/apps/basecamp-mcp) |
| [Wrike](https://vinkius.com/en/apps/wrike-mcp) | Enterprise work management | [Deploy →](https://vinkius.com/en/apps/wrike-mcp) |
| [Confluence](https://vinkius.com/en/apps/confluence-mcp) | Team wiki and documentation | [Deploy →](https://vinkius.com/en/apps/confluence-mcp) |
| [Zoho Projects](https://vinkius.com/en/apps/zoho-projects-mcp) | Online project management | [Deploy →](https://vinkius.com/en/apps/zoho-projects-mcp) |
| [Odoo Project](https://vinkius.com/en/apps/odoo-project-mcp) | Open-source project management | [Deploy →](https://vinkius.com/en/apps/odoo-project-mcp) |

---

## Productivity and Documents

| Plugin | What It Does | Deploy |
|---|---|---|
| [Notion](https://vinkius.com/en/apps/notion-mcp) | Pages, databases, blocks | [Deploy →](https://vinkius.com/en/apps/notion-mcp) |
| [Google Drive](https://vinkius.com/en/apps/google-drive-mcp) | Files, folders, sharing | [Deploy →](https://vinkius.com/en/apps/google-drive-mcp) |
| [Google Sheets](https://vinkius.com/en/apps/google-sheets-mcp) | Spreadsheets, ranges, formulas | [Deploy →](https://vinkius.com/en/apps/google-sheets-mcp) |
| [Google Calendar](https://vinkius.com/en/apps/google-calendar-mcp) | Events, scheduling | [Deploy →](https://vinkius.com/en/apps/google-calendar-mcp) |
| [Todoist](https://vinkius.com/en/apps/todoist-mcp) | Task management | [Deploy →](https://vinkius.com/en/apps/todoist-mcp) |
| [Zoho Notebook](https://vinkius.com/en/apps/zoho-notebook-mcp) | Note-taking | [Deploy →](https://vinkius.com/en/apps/zoho-notebook-mcp) |
| [Logseq](https://vinkius.com/en/apps/logseq-knowledge-management-mcp) | Knowledge management | [Deploy →](https://vinkius.com/en/apps/logseq-knowledge-management-mcp) |
| [Obsidian Publish](https://vinkius.com/en/apps/obsidian-publish-mcp) | Published notes and wikis | [Deploy →](https://vinkius.com/en/apps/obsidian-publish-mcp) |

---

## Video and Audio

| Plugin | What It Does | Deploy |
|---|---|---|
| [Vimeo](https://vinkius.com/en/apps/vimeo-mcp) | Video hosting and analytics | [Deploy →](https://vinkius.com/en/apps/vimeo-mcp) |
| [Mux](https://vinkius.com/en/apps/mux-mcp) | Video streaming infrastructure | [Deploy →](https://vinkius.com/en/apps/mux-mcp) |
| [Wistia](https://vinkius.com/en/apps/wistia-mcp) | Business video hosting | [Deploy →](https://vinkius.com/en/apps/wistia-mcp) |
| [Loom](https://vinkius.com/en/apps/loom-async-video-messaging-mcp) | Async video messaging | [Deploy →](https://vinkius.com/en/apps/loom-async-video-messaging-mcp) |
| [ElevenLabs](https://vinkius.com/en/apps/elevenlabs-mcp) | AI voice generation | [Deploy →](https://vinkius.com/en/apps/elevenlabs-mcp) |
| [HeyGen](https://vinkius.com/en/apps/heygen-mcp) | AI video avatars | [Deploy →](https://vinkius.com/en/apps/heygen-mcp) |
| [Synthesia](https://vinkius.com/en/apps/synthesia-mcp) | AI video generation | [Deploy →](https://vinkius.com/en/apps/synthesia-mcp) |
| [Runway ML](https://vinkius.com/en/apps/runway-ml-mcp) | AI video editing | [Deploy →](https://vinkius.com/en/apps/runway-ml-mcp) |
| [Descript](https://vinkius.com/en/apps/descript-mcp) | Video and podcast editing | [Deploy →](https://vinkius.com/en/apps/descript-mcp) |
| [YouTube](https://vinkius.com/en/apps/youtube-mcp) | Video platform | [Deploy →](https://vinkius.com/en/apps/youtube-mcp) |

---

## Social Media

| Plugin | What It Does | Deploy |
|---|---|---|
| [X/Twitter](https://vinkius.com/en/apps/x-twitter-mcp) | Posts, timelines, search | [Deploy →](https://vinkius.com/en/apps/x-twitter-mcp) |
| [LinkedIn](https://vinkius.com/en/apps/linkedin-mcp) | Profiles, posts, company pages | [Deploy →](https://vinkius.com/en/apps/linkedin-mcp) |
| [LinkedIn Pages](https://vinkius.com/en/apps/linkedin-page-management-mcp) | Company page management | [Deploy →](https://vinkius.com/en/apps/linkedin-page-management-mcp) |
| [Facebook Pages](https://vinkius.com/en/apps/facebook-pages-mcp) | Page management | [Deploy →](https://vinkius.com/en/apps/facebook-pages-mcp) |
| [Instagram](https://vinkius.com/en/apps/instagram-social-media-business-mcp) | Business account management | [Deploy →](https://vinkius.com/en/apps/instagram-social-media-business-mcp) |
| [Pinterest](https://vinkius.com/en/apps/pinterest-mcp) | Pins, boards, analytics | [Deploy →](https://vinkius.com/en/apps/pinterest-mcp) |
| [Reddit](https://vinkius.com/en/apps/reddit-mcp) | Subreddits, posts, comments | [Deploy →](https://vinkius.com/en/apps/reddit-mcp) |

---

## Search and Web Scraping

| Plugin | What It Does | Deploy |
|---|---|---|
| [Exa AI](https://vinkius.com/en/apps/exa-ai-mcp) | Neural web search for AI | [Deploy →](https://vinkius.com/en/apps/exa-ai-mcp) |
| [Serper](https://vinkius.com/en/apps/serper-mcp) | Google SERP API | [Deploy →](https://vinkius.com/en/apps/serper-mcp) |
| [Firecrawl](https://vinkius.com/en/apps/firecrawl-mcp) | Web scraping to markdown | [Deploy →](https://vinkius.com/en/apps/firecrawl-mcp) |
| [Algolia](https://vinkius.com/en/apps/algolia-mcp) | Search-as-a-service | [Deploy →](https://vinkius.com/en/apps/algolia-mcp) |

---

## File Storage

| Plugin | What It Does | Deploy |
|---|---|---|
| [Dropbox](https://vinkius.com/en/apps/dropbox-mcp) | File storage and sharing | [Deploy →](https://vinkius.com/en/apps/dropbox-mcp) |
| [Box](https://vinkius.com/en/apps/box-mcp) | Enterprise content management | [Deploy →](https://vinkius.com/en/apps/box-mcp) |
| [Cloudinary](https://vinkius.com/en/apps/cloudinary-mcp) | Image/video management | [Deploy →](https://vinkius.com/en/apps/cloudinary-mcp) |
| [Backblaze B2](https://vinkius.com/en/apps/backblaze-b2-mcp) | Affordable cloud storage | [Deploy →](https://vinkius.com/en/apps/backblaze-b2-mcp) |
| [Wasabi](https://vinkius.com/en/apps/wasabi-mcp) | Hot cloud storage | [Deploy →](https://vinkius.com/en/apps/wasabi-mcp) |

---

## Calendar and Scheduling

| Plugin | What It Does | Deploy |
|---|---|---|
| [Calendly](https://vinkius.com/en/apps/calendly-mcp) | Meeting scheduling | [Deploy →](https://vinkius.com/en/apps/calendly-mcp) |
| [SavvyCal](https://vinkius.com/en/apps/savvycal-mcp) | Smart scheduling | [Deploy →](https://vinkius.com/en/apps/savvycal-mcp) |
| [Reclaim.ai](https://vinkius.com/en/apps/reclaimai-mcp) | AI calendar assistant | [Deploy →](https://vinkius.com/en/apps/reclaimai-mcp) |
| [Motion](https://vinkius.com/en/apps/motion-ai-calendar-task-management-mcp) | AI-powered calendar | [Deploy →](https://vinkius.com/en/apps/motion-ai-calendar-task-management-mcp) |
| [Clockwise](https://vinkius.com/en/apps/clockwise-mcp) | Time optimization | [Deploy →](https://vinkius.com/en/apps/clockwise-mcp) |
| [Acuity Scheduling](https://vinkius.com/en/apps/acuity-scheduling-mcp) | Appointment scheduling | [Deploy →](https://vinkius.com/en/apps/acuity-scheduling-mcp) |

---

## Forms and Surveys

| Plugin | What It Does | Deploy |
|---|---|---|
| [Typeform](https://vinkius.com/en/apps/typeform-mcp) | Conversational forms | [Deploy →](https://vinkius.com/en/apps/typeform-mcp) |
| [JotForm](https://vinkius.com/en/apps/jotform-mcp) | Online form builder | [Deploy →](https://vinkius.com/en/apps/jotform-mcp) |
| [Tally](https://vinkius.com/en/apps/tally-mcp) | Free form builder | [Deploy →](https://vinkius.com/en/apps/tally-mcp) |
| [Google Forms](https://vinkius.com/en/apps/google-forms-mcp) | Simple form creation | [Deploy →](https://vinkius.com/en/apps/google-forms-mcp) |
| [PaperForm](https://vinkius.com/en/apps/paperform-mcp) | Beautiful online forms | [Deploy →](https://vinkius.com/en/apps/paperform-mcp) |

---

## Signatures and Documents

| Plugin | What It Does | Deploy |
|---|---|---|
| [DocuSign](https://vinkius.com/en/apps/docusign-mcp) | Electronic signatures | [Deploy →](https://vinkius.com/en/apps/docusign-mcp) |
| [PandaDoc](https://vinkius.com/en/apps/pandadoc-mcp) | Proposals and e-signatures | [Deploy →](https://vinkius.com/en/apps/pandadoc-mcp) |
| [Adobe Acrobat Sign](https://vinkius.com/en/apps/adobe-acrobat-sign-mcp) | Adobe e-signatures | [Deploy →](https://vinkius.com/en/apps/adobe-acrobat-sign-mcp) |
| [Dropbox Sign](https://vinkius.com/en/apps/dropbox-sign-mcp) | Dropbox e-signatures | [Deploy →](https://vinkius.com/en/apps/dropbox-sign-mcp) |
| [YouSign](https://vinkius.com/en/apps/yousign-mcp) | European e-signatures | [Deploy →](https://vinkius.com/en/apps/yousign-mcp) |

---

## Translation

| Plugin | What It Does | Deploy |
|---|---|---|
| [DeepL](https://vinkius.com/en/apps/deepl-mcp) | Premium AI translation | [Deploy →](https://vinkius.com/en/apps/deepl-mcp) |
| [LibreTranslate](https://vinkius.com/en/apps/libretranslate-api-mcp) | Open-source translation | [Deploy →](https://vinkius.com/en/apps/libretranslate-api-mcp) |

---

## SMS and Notifications

| Plugin | What It Does | Deploy |
|---|---|---|
| [Twilio](https://vinkius.com/en/apps/twilio-mcp) | SMS, voice, video | [Deploy →](https://vinkius.com/en/apps/twilio-mcp) |
| [Vonage](https://vinkius.com/en/apps/vonage-mcp) | Communication APIs | [Deploy →](https://vinkius.com/en/apps/vonage-mcp) |
| [MessageBird](https://vinkius.com/en/apps/messagebird-mcp) | Omnichannel messaging | [Deploy →](https://vinkius.com/en/apps/messagebird-mcp) |
| [Plivo](https://vinkius.com/en/apps/plivo-mcp) | Cloud communications | [Deploy →](https://vinkius.com/en/apps/plivo-mcp) |
| [Sinch](https://vinkius.com/en/apps/sinch-mcp) | Cloud messaging | [Deploy →](https://vinkius.com/en/apps/sinch-mcp) |
| [OneSignal](https://vinkius.com/en/apps/onesignal-mcp) | Push notifications | [Deploy →](https://vinkius.com/en/apps/onesignal-mcp) |

---

## Telephony and VoIP

| Plugin | What It Does | Deploy |
|---|---|---|
| [Aircall](https://vinkius.com/en/apps/aircall-mcp) | Cloud phone system | [Deploy →](https://vinkius.com/en/apps/aircall-mcp) |
| [Dialpad](https://vinkius.com/en/apps/dialpad-mcp) | AI-powered communications | [Deploy →](https://vinkius.com/en/apps/dialpad-mcp) |
| [Five9](https://vinkius.com/en/apps/five9-mcp) | Contact center platform | [Deploy →](https://vinkius.com/en/apps/five9-mcp) |
| [JustCall](https://vinkius.com/en/apps/justcall-mcp) | Business phone system | [Deploy →](https://vinkius.com/en/apps/justcall-mcp) |

---

## ERP and Business Operations

| Plugin | What It Does | Deploy |
|---|---|---|
| [Odoo ERP](https://vinkius.com/en/apps/odoo-erp-full-mcp) | Complete open-source ERP | [Deploy →](https://vinkius.com/en/apps/odoo-erp-full-mcp) |
| [Odoo Sales](https://vinkius.com/en/apps/odoo-sales-mcp) | Sales management | [Deploy →](https://vinkius.com/en/apps/odoo-sales-mcp) |
| [Odoo Inventory](https://vinkius.com/en/apps/odoo-inventory-mcp) | Warehouse management | [Deploy →](https://vinkius.com/en/apps/odoo-inventory-mcp) |
| [Odoo Manufacturing](https://vinkius.com/en/apps/odoo-manufacturing-mcp) | Production planning | [Deploy →](https://vinkius.com/en/apps/odoo-manufacturing-mcp) |
| [Odoo HR](https://vinkius.com/en/apps/odoo-hr-mcp) | Human resources | [Deploy →](https://vinkius.com/en/apps/odoo-hr-mcp) |
| [Odoo Accounting](https://vinkius.com/en/apps/odoo-accounting-mcp) | Accounting module | [Deploy →](https://vinkius.com/en/apps/odoo-accounting-mcp) |
| [Odoo Purchase](https://vinkius.com/en/apps/odoo-purchase-mcp) | Procurement management | [Deploy →](https://vinkius.com/en/apps/odoo-purchase-mcp) |
| [SAP S/4HANA](https://vinkius.com/en/apps/sap-s4hana-mcp) | Enterprise ERP | [Deploy →](https://vinkius.com/en/apps/sap-s4hana-mcp) |
| [SAP Concur](https://vinkius.com/en/apps/sap-concur-mcp) | Travel and expense | [Deploy →](https://vinkius.com/en/apps/sap-concur-mcp) |
| [Oracle NetSuite](https://vinkius.com/en/apps/oracle-netsuite-mcp) | Cloud ERP | [Deploy →](https://vinkius.com/en/apps/oracle-netsuite-mcp) |
| [Workday](https://vinkius.com/en/apps/workday-mcp) | Enterprise HR and finance | [Deploy →](https://vinkius.com/en/apps/workday-mcp) |
| [Dynamics 365 Finance](https://vinkius.com/en/apps/dynamics-365-finance-operations-mcp) | Microsoft finance operations | [Deploy →](https://vinkius.com/en/apps/dynamics-365-finance-operations-mcp) |
| [Zoho Inventory](https://vinkius.com/en/apps/zoho-inventory-mcp) | Inventory management | [Deploy →](https://vinkius.com/en/apps/zoho-inventory-mcp) |

---

## Legal and Compliance

| Plugin | What It Does | Deploy |
|---|---|---|
| [Clio](https://vinkius.com/en/apps/clio-mcp) | Legal practice management | [Deploy →](https://vinkius.com/en/apps/clio-mcp) |
| [Bloomberg Law](https://vinkius.com/en/apps/bloomberg-law-mcp) | Legal research and analytics | [Deploy →](https://vinkius.com/en/apps/bloomberg-law-mcp) |
| [CourtListener](https://vinkius.com/en/apps/courtlistener-mcp) | Free legal opinions database | [Deploy →](https://vinkius.com/en/apps/courtlistener-mcp) |
| [Justia](https://vinkius.com/en/apps/justia-legal-intelligence-mcp) | Legal intelligence | [Deploy →](https://vinkius.com/en/apps/justia-legal-intelligence-mcp) |
| [CloudLex](https://vinkius.com/en/apps/cloudlex-legal-mcp) | Legal case management | [Deploy →](https://vinkius.com/en/apps/cloudlex-legal-mcp) |
| [MyCase](https://vinkius.com/en/apps/mycase-legal-mcp) | Legal practice software | [Deploy →](https://vinkius.com/en/apps/mycase-legal-mcp) |
| [OpenLaws](https://vinkius.com/en/apps/openlaws-mcp) | Open legal data access | [Deploy →](https://vinkius.com/en/apps/openlaws-mcp) |
| [BCLaws](https://vinkius.com/en/apps/bclaws-api-mcp) | BC legislation database | [Deploy →](https://vinkius.com/en/apps/bclaws-api-mcp) |

---

## Logistics and Shipping

| Plugin | What It Does | Deploy |
|---|---|---|
| [FedEx](https://vinkius.com/en/apps/fedex-mcp) | Shipping and tracking | [Deploy →](https://vinkius.com/en/apps/fedex-mcp) |
| [DHL](https://vinkius.com/en/apps/dhl-mcp) | International shipping | [Deploy →](https://vinkius.com/en/apps/dhl-mcp) |
| [USPS](https://vinkius.com/en/apps/usps-developer-portal-mcp) | US postal service | [Deploy →](https://vinkius.com/en/apps/usps-developer-portal-mcp) |
| [EasyPost](https://vinkius.com/en/apps/easypost-mcp) | Multi-carrier shipping | [Deploy →](https://vinkius.com/en/apps/easypost-mcp) |
| [AfterShip](https://vinkius.com/en/apps/aftership-tracking-mcp) | Package tracking | [Deploy →](https://vinkius.com/en/apps/aftership-tracking-mcp) |
| [AfterShip Returns](https://vinkius.com/en/apps/aftership-returns-mcp) | Returns management | [Deploy →](https://vinkius.com/en/apps/aftership-returns-mcp) |

---

## Events and Webinars

| Plugin | What It Does | Deploy |
|---|---|---|
| [Eventbrite](https://vinkius.com/en/apps/eventbrite-mcp) | Event management | [Deploy →](https://vinkius.com/en/apps/eventbrite-mcp) |
| [Meetup](https://vinkius.com/en/apps/meetup-mcp) | Community events | [Deploy →](https://vinkius.com/en/apps/meetup-mcp) |
| [Zoom](https://vinkius.com/en/apps/zoom-mcp) | Video conferencing | [Deploy →](https://vinkius.com/en/apps/zoom-mcp) |
| [Webex](https://vinkius.com/en/apps/webex-mcp) | Cisco video meetings | [Deploy →](https://vinkius.com/en/apps/webex-mcp) |
| [Airmeet](https://vinkius.com/en/apps/airmeet-mcp) | Virtual events platform | [Deploy →](https://vinkius.com/en/apps/airmeet-mcp) |

---

## Automation Platforms

| Plugin | What It Does | Deploy |
|---|---|---|
| [Zapier](https://vinkius.com/en/apps/zapier-mcp) | No-code automation | [Deploy →](https://vinkius.com/en/apps/zapier-mcp) |
| [Make](https://vinkius.com/en/apps/make-workflow-automation-mcp) | Visual workflow automation | [Deploy →](https://vinkius.com/en/apps/make-workflow-automation-mcp) |
| [n8n](https://vinkius.com/en/apps/n8n-ai-workflow-automation-mcp) | Open-source workflow automation | [Deploy →](https://vinkius.com/en/apps/n8n-ai-workflow-automation-mcp) |
| [Pipedream](https://vinkius.com/en/apps/pipedream-mcp) | Developer-first workflows | [Deploy →](https://vinkius.com/en/apps/pipedream-mcp) |
| [Workato](https://vinkius.com/en/apps/workato-mcp) | Enterprise iPaaS | [Deploy →](https://vinkius.com/en/apps/workato-mcp) |

---

## Crypto and Blockchain

| Plugin | What It Does | Deploy |
|---|---|---|
| [CoinGecko](https://vinkius.com/en/apps/coingecko-mcp) | Crypto prices, market data | [Deploy →](https://vinkius.com/en/apps/coingecko-mcp) |
| [CoinMarketCap](https://vinkius.com/en/apps/coinmarketcap-mcp) | Market cap rankings | [Deploy →](https://vinkius.com/en/apps/coinmarketcap-mcp) |
| [Etherscan](https://vinkius.com/en/apps/etherscan-mcp) | Ethereum blockchain explorer | [Deploy →](https://vinkius.com/en/apps/etherscan-mcp) |
| [Binance](https://vinkius.com/en/apps/binance-mcp) | Crypto exchange | [Deploy →](https://vinkius.com/en/apps/binance-mcp) |
| [Coinbase](https://vinkius.com/en/apps/coinbase-mcp) | Crypto exchange | [Deploy →](https://vinkius.com/en/apps/coinbase-mcp) |
| [Kraken](https://vinkius.com/en/apps/kraken-mcp) | Crypto exchange | [Deploy →](https://vinkius.com/en/apps/kraken-mcp) |
| [Alchemy](https://vinkius.com/en/apps/alchemy-mcp) | Web3 development platform | [Deploy →](https://vinkius.com/en/apps/alchemy-mcp) |
| [CoinDesk BPI](https://vinkius.com/en/apps/coindesk-bitcoin-price-index-mcp) | Bitcoin price index | [Deploy →](https://vinkius.com/en/apps/coindesk-bitcoin-price-index-mcp) |
| [CoinMarketCal](https://vinkius.com/en/apps/coinmarketcal-mcp) | Crypto events calendar | [Deploy →](https://vinkius.com/en/apps/coinmarketcal-mcp) |

---

## Stock Market and Fintech

| Plugin | What It Does | Deploy |
|---|---|---|
| [Alpha Vantage](https://vinkius.com/en/apps/alpha-vantage-mcp) | Stock and forex data | [Deploy →](https://vinkius.com/en/apps/alpha-vantage-mcp) |
| [Finnhub](https://vinkius.com/en/apps/finnhub-mcp) | Real-time financial data | [Deploy →](https://vinkius.com/en/apps/finnhub-mcp) |
| [Twelve Data](https://vinkius.com/en/apps/twelve-data-mcp) | Stock and crypto API | [Deploy →](https://vinkius.com/en/apps/twelve-data-mcp) |
| [SEC EDGAR Full](https://vinkius.com/en/apps/sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents-mcp) | SEC filings — the free Bloomberg alternative | [Deploy →](https://vinkius.com/en/apps/sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents-mcp) |
| [SEC EDGAR Filings](https://vinkius.com/en/apps/sec-edgar-filings-10-k-10-q-8-k-insider-trades-full-text-search-mcp) | 10-K, 10-Q, insider trades | [Deploy →](https://vinkius.com/en/apps/sec-edgar-filings-10-k-10-q-8-k-insider-trades-full-text-search-mcp) |
| [SEC EDGAR Financials](https://vinkius.com/en/apps/sec-edgar-financials-revenue-income-assets-eps-industry-comparison-mcp) | Revenue, income, EPS comparison | [Deploy →](https://vinkius.com/en/apps/sec-edgar-financials-revenue-income-assets-eps-industry-comparison-mcp) |

---

## Government Data

See [awesome-mcp-servers](https://github.com/vinkius-labs/awesome-mcp-servers) for the full list of 90+ government data MCPs including FRED, BLS, ECB, Eurostat, UK ONS, US Census, US Treasury, World Bank, NOAA, NASA, USDA, EPA, FDA, CDC, FEMA, EIA, DOT, NIST, and BCB (Brazil).

---

## NASA and Space

| Plugin | What It Does | Deploy |
|---|---|---|
| [NASA Full](https://vinkius.com/en/apps/nasa-full-ultimate-space-intelligence-mcp) | Complete NASA data access | [Deploy →](https://vinkius.com/en/apps/nasa-full-ultimate-space-intelligence-mcp) |
| [NASA Asteroids](https://vinkius.com/en/apps/nasa-asteroids-near-earth-objects-planetary-defense-mcp) | Near-Earth objects | [Deploy →](https://vinkius.com/en/apps/nasa-asteroids-near-earth-objects-planetary-defense-mcp) |
| [NASA Mars Rover](https://vinkius.com/en/apps/nasa-mars-rover-photos-from-the-red-planet-mcp) | Mars photos | [Deploy →](https://vinkius.com/en/apps/nasa-mars-rover-photos-from-the-red-planet-mcp) |
| [NASA Exoplanets](https://vinkius.com/en/apps/nasa-exoplanets-worlds-beyond-our-solar-system-mcp) | Exoplanet data | [Deploy →](https://vinkius.com/en/apps/nasa-exoplanets-worlds-beyond-our-solar-system-mcp) |
| [NASA Space Weather](https://vinkius.com/en/apps/nasa-donki-space-weather-intelligence-mcp) | Solar storms, CMEs | [Deploy →](https://vinkius.com/en/apps/nasa-donki-space-weather-intelligence-mcp) |
| [NASA APOD](https://vinkius.com/en/apps/nasa-apod-astronomy-picture-of-the-day-mcp) | Astronomy Picture of the Day | [Deploy →](https://vinkius.com/en/apps/nasa-apod-astronomy-picture-of-the-day-mcp) |
| [NASA Earth](https://vinkius.com/en/apps/nasa-earth-full-disk-imagery-natural-events-mcp) | Earth imagery and events | [Deploy →](https://vinkius.com/en/apps/nasa-earth-full-disk-imagery-natural-events-mcp) |

---

## Gaming and Esports

| Plugin | What It Does | Deploy |
|---|---|---|
| [Steam Hype](https://vinkius.com/en/apps/steam-platform-hype-intelligence-mcp) | Trending games, wishlists | [Deploy →](https://vinkius.com/en/apps/steam-platform-hype-intelligence-mcp) |
| [Steam Economy](https://vinkius.com/en/apps/steam-economy-market-intelligence-mcp) | Market items, trading | [Deploy →](https://vinkius.com/en/apps/steam-economy-market-intelligence-mcp) |
| [Steam Scouting](https://vinkius.com/en/apps/steam-performance-scouting-intelligence-mcp) | Player stats, reviews | [Deploy →](https://vinkius.com/en/apps/steam-performance-scouting-intelligence-mcp) |
| [Roblox Discovery](https://vinkius.com/en/apps/roblox-experience-discovery-mcp) | Experience discovery | [Deploy →](https://vinkius.com/en/apps/roblox-experience-discovery-mcp) |
| [Roblox Social](https://vinkius.com/en/apps/roblox-social-group-intelligence-mcp) | Social and groups | [Deploy →](https://vinkius.com/en/apps/roblox-social-group-intelligence-mcp) |
| [Roblox Avatar](https://vinkius.com/en/apps/roblox-avatar-catalog-intelligence-mcp) | Avatar catalog | [Deploy →](https://vinkius.com/en/apps/roblox-avatar-catalog-intelligence-mcp) |
| [Epic Games Store](https://vinkius.com/en/apps/epic-games-store-intelligence-mcp) | Store intelligence | [Deploy →](https://vinkius.com/en/apps/epic-games-store-intelligence-mcp) |
| [Fortnite Stats](https://vinkius.com/en/apps/fortnite-player-stats-news-intelligence-mcp) | Player stats | [Deploy →](https://vinkius.com/en/apps/fortnite-player-stats-news-intelligence-mcp) |
| [Fortnite Cosmetics](https://vinkius.com/en/apps/fortnite-cosmetics-item-shop-mcp) | Item shop | [Deploy →](https://vinkius.com/en/apps/fortnite-cosmetics-item-shop-mcp) |
| [Fortnite Map](https://vinkius.com/en/apps/fortnite-map-playlists-engine-intelligence-mcp) | Maps and playlists | [Deploy →](https://vinkius.com/en/apps/fortnite-map-playlists-engine-intelligence-mcp) |
| [Riot Games](https://vinkius.com/en/apps/riot-games-mcp) | LoL, Valorant, TFT | [Deploy →](https://vinkius.com/en/apps/riot-games-mcp) |
| [Twitch](https://vinkius.com/en/apps/twitch-mcp) | Streams, channels, clips | [Deploy →](https://vinkius.com/en/apps/twitch-mcp) |
| [IGDB](https://vinkius.com/en/apps/igdb-global-gaming-database-mcp) | Game database | [Deploy →](https://vinkius.com/en/apps/igdb-global-gaming-database-mcp) |
| [RAWG](https://vinkius.com/en/apps/rawg-video-games-database-mcp) | Video games database | [Deploy →](https://vinkius.com/en/apps/rawg-video-games-database-mcp) |
| [PandaScore](https://vinkius.com/en/apps/pandascore-mcp) | Esports data | [Deploy →](https://vinkius.com/en/apps/pandascore-mcp) |
| [Chess.com](https://vinkius.com/en/apps/chesscom-global-intelligence-mcp) | Chess intelligence | [Deploy →](https://vinkius.com/en/apps/chesscom-global-intelligence-mcp) |
| [Lichess](https://vinkius.com/en/apps/lichessorg-open-chess-intelligence-mcp) | Open chess data | [Deploy →](https://vinkius.com/en/apps/lichessorg-open-chess-intelligence-mcp) |
| [GamerPower](https://vinkius.com/en/apps/gamerpower-gaming-giveaways-mcp) | Gaming giveaways | [Deploy →](https://vinkius.com/en/apps/gamerpower-gaming-giveaways-mcp) |

---

## Music and Audio Platforms

| Plugin | What It Does | Deploy |
|---|---|---|
| [Spotify](https://vinkius.com/en/apps/spotify-music-mcp) | Music streaming, playlists | [Deploy →](https://vinkius.com/en/apps/spotify-music-mcp) |
| [SoundCloud](https://vinkius.com/en/apps/soundcloud-mcp) | Audio platform | [Deploy →](https://vinkius.com/en/apps/soundcloud-mcp) |
| [Deezer](https://vinkius.com/en/apps/deezer-mcp) | Music streaming | [Deploy →](https://vinkius.com/en/apps/deezer-mcp) |
| [TIDAL](https://vinkius.com/en/apps/tidal-developer-api-mcp) | Hi-fi music streaming | [Deploy →](https://vinkius.com/en/apps/tidal-developer-api-mcp) |
| [MusicBrainz](https://vinkius.com/en/apps/musicbrainz-mcp) | Open music database | [Deploy →](https://vinkius.com/en/apps/musicbrainz-mcp) |
| [Last.fm](https://vinkius.com/en/apps/lastfm-mcp) | Music scrobbling and stats | [Deploy →](https://vinkius.com/en/apps/lastfm-mcp) |
| [Genius](https://vinkius.com/en/apps/genius-mcp) | Song lyrics and annotations | [Deploy →](https://vinkius.com/en/apps/genius-mcp) |
| [Musixmatch](https://vinkius.com/en/apps/musixmatch-mcp) | Lyrics database | [Deploy →](https://vinkius.com/en/apps/musixmatch-mcp) |
| [Discogs](https://vinkius.com/en/apps/discogs-mcp) | Music catalog and marketplace | [Deploy →](https://vinkius.com/en/apps/discogs-mcp) |
| [Bandcamp](https://vinkius.com/en/apps/bandcamp-mcp) | Independent music platform | [Deploy →](https://vinkius.com/en/apps/bandcamp-mcp) |

---

## Sports and Fitness

| Plugin | What It Does | Deploy |
|---|---|---|
| [Strava Training](https://vinkius.com/en/apps/strava-training-mcp) | Training data and analytics | [Deploy →](https://vinkius.com/en/apps/strava-training-mcp) |
| [Strava Social](https://vinkius.com/en/apps/strava-social-mcp) | Social fitness features | [Deploy →](https://vinkius.com/en/apps/strava-social-mcp) |
| [Strava Planning](https://vinkius.com/en/apps/strava-planning-mcp) | Route planning | [Deploy →](https://vinkius.com/en/apps/strava-planning-mcp) |
| [Fitbit](https://vinkius.com/en/apps/fitbit-mcp) | Activity and health tracking | [Deploy →](https://vinkius.com/en/apps/fitbit-mcp) |
| [WHOOP](https://vinkius.com/en/apps/whoop-mcp) | Recovery and strain | [Deploy →](https://vinkius.com/en/apps/whoop-mcp) |
| [Withings](https://vinkius.com/en/apps/withings-mcp) | Health devices data | [Deploy →](https://vinkius.com/en/apps/withings-mcp) |
| [OpenF1](https://vinkius.com/en/apps/openf1-live-data-telemetry-mcp) | Formula 1 live telemetry | [Deploy →](https://vinkius.com/en/apps/openf1-live-data-telemetry-mcp) |
| [Hyprace F1](https://vinkius.com/en/apps/hyprace-f1-data-mcp) | F1 historical data | [Deploy →](https://vinkius.com/en/apps/hyprace-f1-data-mcp) |
| [API Football](https://vinkius.com/en/apps/api-football-mcp) | Global football data | [Deploy →](https://vinkius.com/en/apps/api-football-mcp) |
| [TheSportsDB](https://vinkius.com/en/apps/thesportsdb-global-sports-database-mcp) | Global sports database | [Deploy →](https://vinkius.com/en/apps/thesportsdb-global-sports-database-mcp) |
| [FantasyData](https://vinkius.com/en/apps/fantasydata-sportsdataio-mcp) | Fantasy sports data | [Deploy →](https://vinkius.com/en/apps/fantasydata-sportsdataio-mcp) |
| [Cartola FC](https://vinkius.com/en/apps/cartola-fc-fantasy-football-mcp) | Brazilian fantasy football | [Deploy →](https://vinkius.com/en/apps/cartola-fc-fantasy-football-mcp) |
| [API Futebol](https://vinkius.com/en/apps/api-futebol-brazilian-football-mcp) | Brazilian football leagues | [Deploy →](https://vinkius.com/en/apps/api-futebol-brazilian-football-mcp) |

---

## Food and Restaurants

| Plugin | What It Does | Deploy |
|---|---|---|
| [DoorDash](https://vinkius.com/en/apps/doordash-drive-mcp) | Delivery logistics | [Deploy →](https://vinkius.com/en/apps/doordash-drive-mcp) |
| [Uber Eats](https://vinkius.com/en/apps/uber-eats-mcp) | Food delivery | [Deploy →](https://vinkius.com/en/apps/uber-eats-mcp) |
| [iFood](https://vinkius.com/en/apps/ifood-mcp) | Brazilian food delivery | [Deploy →](https://vinkius.com/en/apps/ifood-mcp) |
| [Rappi](https://vinkius.com/en/apps/rappi-api-mcp) | LATAM delivery platform | [Deploy →](https://vinkius.com/en/apps/rappi-api-mcp) |
| [Tock](https://vinkius.com/en/apps/tock-reservations-mcp) | Restaurant reservations | [Deploy →](https://vinkius.com/en/apps/tock-reservations-mcp) |

---

## Education

| Plugin | What It Does | Deploy |
|---|---|---|
| [Moodle](https://vinkius.com/en/apps/moodle-mcp) | Learning management system | [Deploy →](https://vinkius.com/en/apps/moodle-mcp) |
| [Udemy](https://vinkius.com/en/apps/udemy-mcp) | Online courses marketplace | [Deploy →](https://vinkius.com/en/apps/udemy-mcp) |
| [edX](https://vinkius.com/en/apps/edx-mcp) | University courses platform | [Deploy →](https://vinkius.com/en/apps/edx-mcp) |
| [Duolingo](https://vinkius.com/en/apps/duolingo-mcp) | Language learning | [Deploy →](https://vinkius.com/en/apps/duolingo-mcp) |

---

## Real Estate

| Plugin | What It Does | Deploy |
|---|---|---|
| [Zillow](https://vinkius.com/en/apps/zillow-mcp) | US property listings | [Deploy →](https://vinkius.com/en/apps/zillow-mcp) |
| [Idealista](https://vinkius.com/en/apps/idealista-real-estate-mcp) | European real estate | [Deploy →](https://vinkius.com/en/apps/idealista-real-estate-mcp) |

---

## IoT and Smart Home

| Plugin | What It Does | Deploy |
|---|---|---|
| [Home Assistant](https://vinkius.com/en/apps/home-assistant-mcp) | Smart home automation | [Deploy →](https://vinkius.com/en/apps/home-assistant-mcp) |
| [Particle IoT](https://vinkius.com/en/apps/particle-iot-mcp) | IoT device management | [Deploy →](https://vinkius.com/en/apps/particle-iot-mcp) |

---

## Secrets Management

| Plugin | What It Does | Deploy |
|---|---|---|
| [Doppler](https://vinkius.com/en/apps/doppler-mcp) | Secrets management platform | [Deploy →](https://vinkius.com/en/apps/doppler-mcp) |
| [Infisical](https://vinkius.com/en/apps/infisical-mcp) | Open-source secrets manager | [Deploy →](https://vinkius.com/en/apps/infisical-mcp) |

---

## Testing and QA

| Plugin | What It Does | Deploy |
|---|---|---|
| [BrowserStack](https://vinkius.com/en/apps/browserstack-mcp) | Cross-browser testing | [Deploy →](https://vinkius.com/en/apps/browserstack-mcp) |
| [Cypress Cloud](https://vinkius.com/en/apps/cypress-cloud-mcp) | E2E testing | [Deploy →](https://vinkius.com/en/apps/cypress-cloud-mcp) |
| [Percy](https://vinkius.com/en/apps/percy-mcp) | Visual testing | [Deploy →](https://vinkius.com/en/apps/percy-mcp) |

---

## How to Install a Plugin

### Step 1: Deploy the MCP server

Go to [vinkius.com](https://vinkius.com), find the server, and deploy it. You receive an SSE endpoint URL.

### Step 2: Add to `.mcp.json`

```json
{
  "mcpServers": {
    "plugin-name": { "url": "https://edge.vinkius.com/vk_live_xxx/mcp" }
  }
}
```

### Step 3: Start Claude Code

```bash
claude
/mcp  # verify connection
```

---

This directory lists **200+ plugins** from the Vinkius catalog. Browse all **2,600+ MCP servers**: [vinkius.com/en/categories](https://vinkius.com/en/categories)

## License

MIT — [Vinkius Labs](https://vinkius.com)
