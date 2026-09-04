# AI Tools Categories

**English** · [العربية](README.ar.md)

> A two-level taxonomy of AI tool categories with stable slugs, parents, aliases, and
> descriptions, ready to drop into a directory or a dataset.

<!-- counts:start -->
![Categories](https://img.shields.io/badge/categories-182-informational)
<!-- counts:end -->
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen)
[![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-lightgrey)](LICENSE)

20 top-level categories and 162 subcategories, as JSON and CSV. Every node has a stable
slug, a parent, a one-line description, and the other names it commonly goes by. It is the
part of a directory nobody wants to design from scratch and everybody ends up designing
badly.

The top level is deliberately the same twenty categories used by the TiorAI AI tools dataset,
so the two fit together: adopt the top level alone and stay compatible with published data, or
adopt both levels and get the detail. A competing second top level would have made two TiorAI
repositories disagree with each other in public.

Maintained by [TiorAI](https://tiorai.com/), which catalogues AI tools for a living.

<!-- last-reviewed:start -->
**Last reviewed:** 2026-09-04
<!-- last-reviewed:end -->

## Contents

- [What's in the dataset](#whats-in-the-dataset)
- [The categories](#the-categories)
- [Writing and content](#writing-and-content)
- [Image generation and editing](#image-generation-and-editing)
- [Video](#video)
- [Audio, music, and voice](#audio-music-and-voice)
- [Coding and development](#coding-and-development)
- [Developer infrastructure and models](#developer-infrastructure-and-models)
- [Chatbots and assistants](#chatbots-and-assistants)
- [Automation and agents](#automation-and-agents)
- [Productivity and workflow](#productivity-and-workflow)
- [Presentations and documents](#presentations-and-documents)
- [Design and creative](#design-and-creative)
- [Marketing and advertising](#marketing-and-advertising)
- [SEO and search](#seo-and-search)
- [Sales and CRM](#sales-and-crm)
- [Customer support](#customer-support)
- [Data and analytics](#data-and-analytics)
- [Research and knowledge](#research-and-knowledge)
- [Education and learning](#education-and-learning)
- [Business and finance](#business-and-finance)
- [Health and lifestyle](#health-and-lifestyle)
- [Schema](#schema)
- [How categories are selected](#how-categories-are-selected)
- [Using the data](#using-the-data)
- [Known limitations](#known-limitations)
- [Suggest a category](#suggest-a-category)
- [Contributing](#contributing)
- [Disclaimer](#disclaimer)
- [License](#license)
- [About TiorAI](#about-tiorai)

## What's in the dataset

```text
data/
├── categories.json        all 182 nodes, typed, with parents and children
├── categories-flat.csv    the same 182 nodes, one row each
├── categories.csv         the 20 top-level categories with a subcategory count
└── schema.json            JSON Schema for categories.json
```

## The categories

All 182 categories, grouped by top-level parent and sorted by name inside each group. Position carries no meaning.

This section is generated from `data/categories.json`, so it cannot disagree with the data files. They are the source; this is a view of them, and [`data/categories-flat.csv`](data/categories-flat.csv) stays the faster way to search, sort, or filter all of it at once.

| Category | Slug | Subcategories |
|---|---|---:|
| [Writing and content](#writing-and-content) | `writing-and-content` | 9 |
| [Image generation and editing](#image-generation-and-editing) | `image-generation-and-editing` | 8 |
| [Video](#video) | `video` | 8 |
| [Audio, music, and voice](#audio-music-and-voice) | `audio-music-and-voice` | 9 |
| [Coding and development](#coding-and-development) | `coding-and-development` | 12 |
| [Developer infrastructure and models](#developer-infrastructure-and-models) | `developer-infrastructure-and-models` | 12 |
| [Chatbots and assistants](#chatbots-and-assistants) | `chatbots-and-assistants` | 7 |
| [Automation and agents](#automation-and-agents) | `automation-and-agents` | 7 |
| [Productivity and workflow](#productivity-and-workflow) | `productivity-and-workflow` | 8 |
| [Presentations and documents](#presentations-and-documents) | `presentations-and-documents` | 6 |
| [Design and creative](#design-and-creative) | `design-and-creative` | 7 |
| [Marketing and advertising](#marketing-and-advertising) | `marketing-and-advertising` | 10 |
| [SEO and search](#seo-and-search) | `seo-and-search` | 10 |
| [Sales and CRM](#sales-and-crm) | `sales-and-crm` | 7 |
| [Customer support](#customer-support) | `customer-support` | 6 |
| [Data and analytics](#data-and-analytics) | `data-and-analytics` | 7 |
| [Research and knowledge](#research-and-knowledge) | `research-and-knowledge` | 8 |
| [Education and learning](#education-and-learning) | `education-and-learning` | 7 |
| [Business and finance](#business-and-finance) | `business-and-finance` | 8 |
| [Health and lifestyle](#health-and-lifestyle) | `health-and-lifestyle` | 6 |

## Writing and content

Drafting, editing, and producing written material.

- **Academic and technical writing** — Papers, documentation, and other writing with citation or precision demands. `academic-and-technical-writing`
- **AI content detection** — Estimating whether a passage was machine written. `ai-content-detection`
- **Copywriting** — Short persuasive text for ads, landing pages, product pages, and email. `copywriting`
- **Grammar and style checking** — Correcting mechanics and enforcing a consistent house style. `grammar-and-style-checking`
- **Long-form writing** — Drafting articles, reports, books, and other extended pieces. `long-form-writing`
- **Paraphrasing and rewriting** — Restating existing text at a different length, register, or reading level. `paraphrasing-and-rewriting`
- **Scriptwriting** — Writing for video, podcast, and spoken delivery. `scriptwriting`
- **Summarisation** — Condensing documents, transcripts, or threads into their substance. `summarisation`
- **Translation and localisation** — Moving text between languages and adapting it for a local audience. `translation-and-localisation`

## Image generation and editing

Creating and altering still images.

- **Background removal** — Separating a subject from its background. `background-removal`
- **Headshots and avatars** — Generating portraits of a person from supplied photographs. `headshots-and-avatars`
- **Image APIs** — Programmatic access to generation and editing models. `image-apis`
- **Image editing** — Altering an existing image, including inpainting and object removal. `image-editing`
- **Logo and brand assets** — Marks, icons, and vector assets for an identity. `logo-and-brand-assets`
- **Product photography** — Producing or improving catalogue and ecommerce imagery. `product-photography`
- **Text to image** — Generating an image from a written description. `text-to-image`
- **Upscaling and restoration** — Raising resolution and repairing damaged or low-quality images. `upscaling-and-restoration`

## Video

Producing, editing, and repurposing moving pictures.

- **AI avatars and presenters** — Synthetic on-camera presenters delivering a script. `ai-avatars-and-presenters`
- **Animation and motion** — Animating stills, characters, and motion graphics. `animation-and-motion`
- **Clipping and repurposing** — Cutting long footage into short vertical pieces. `clipping-and-repurposing`
- **Dubbing and subtitling** — Translating spoken audio and matching it to the picture. `dubbing-and-subtitling`
- **Text to video** — Generating footage from a written description. `text-to-video`
- **Video APIs** — Programmatic access to video generation and processing. `video-apis`
- **Video editing** — Cutting, assembling, and correcting existing footage. `video-editing`
- **Video enhancement** — Upscaling, stabilising, denoising, and interpolating footage. `video-enhancement`

## Audio, music, and voice

Speech, sound, music, and everything else heard rather than read.

- **Audio editing and mastering** — Assembling, balancing, and finishing audio. `audio-editing-and-mastering`
- **Audio enhancement** — Removing noise, echo, and artefacts from recordings. `audio-enhancement`
- **Music generation** — Composing or producing music and sound beds. `music-generation`
- **Podcast production** — Recording, editing, and publishing spoken-word shows. `podcast-production`
- **Speech APIs** — Programmatic access to speech recognition and synthesis. `speech-apis`
- **Speech to text** — Turning spoken audio into written text. `speech-to-text`
- **Text to speech** — Turning written text into spoken audio. `text-to-speech`
- **Voice agents** — Systems that hold a spoken conversation and take action. `voice-agents`
- **Voice cloning** — Recreating a specific voice from a sample. `voice-cloning`

## Coding and development

Writing, reviewing, testing, and shipping software.

- **AI code editors** — Editors and IDEs built around a model. `ai-code-editors`
- **Application security** — Finding and fixing vulnerabilities in code and dependencies. `application-security`
- **Code completion** — Suggesting the next lines as a developer types. `code-completion`
- **Code review** — Automated review of changes before they merge. `code-review`
- **Coding agents** — Systems that carry out a coding task across several files. `coding-agents`
- **Database and SQL** — Writing queries, designing schemas, and explaining plans. `database-and-sql`
- **Debugging** — Locating and explaining defects in running software. `debugging`
- **DevOps and infrastructure** — CI/CD, infrastructure as code, incidents, and operations. `devops-and-infrastructure`
- **Documentation** — Generating and maintaining developer documentation. `documentation`
- **Frontend and UI generation** — Producing interface code from a design or a description. `frontend-and-ui-generation`
- **Terminal assistants** — Model-backed tools driven from a command line. `terminal-assistants`
- **Testing and QA** — Generating, maintaining, and running tests. `testing-and-qa`

## Developer infrastructure and models

What an AI application is built on.

- **Agent frameworks** — Libraries for building systems that plan and use tools. `agent-frameworks`
- **Evaluation platforms** — Measuring output quality against datasets and rubrics. `evaluation-platforms`
- **Fine-tuning platforms** — Adapting a base model to a task or a house style. `fine-tuning-platforms`
- **Guardrails and moderation** — Constraining what goes into and out of a model. `guardrails-and-moderation`
- **LLM gateways** — A single endpoint in front of several model providers. `llm-gateways`
- **Model APIs** — Hosted access to language, image, speech, and embedding models. `model-apis`
- **Model hosting and serving** — Running models on managed or self-operated infrastructure. `model-hosting-and-serving`
- **Observability and tracing** — Recording prompts, tool calls, cost, and latency per request. `observability-and-tracing`
- **Prompt management** — Versioning, testing, and deploying prompts as artefacts. `prompt-management`
- **RAG frameworks** — Libraries for retrieval-augmented generation pipelines. `rag-frameworks`
- **Synthetic data** — Generating training and evaluation data. `synthetic-data`
- **Vector databases** — Storage and nearest-neighbour search over embeddings. `vector-databases`

## Chatbots and assistants

General conversational systems, and the interfaces people meet a model through.

- **Answer engines** — Search that returns a written answer with sources. `answer-engines`
- **Browser assistants** — Assistants that work inside the web browser. `browser-assistants`
- **Character and roleplay** — Persona-driven conversation and interactive fiction. `character-and-roleplay`
- **Custom assistant builders** — No-code tools for building a branded assistant. `custom-assistant-builders`
- **General assistants** — Broad conversational products for everyday use. `general-assistants`
- **Local and private assistants** — Assistants running on the user's own hardware. `local-and-private-assistants`
- **Multi-model platforms** — Interfaces offering several providers' models side by side. `multi-model-platforms`

## Automation and agents

Work that runs without a person driving each step.

- **Browser and web automation** — Driving a browser to gather data or complete tasks. `browser-and-web-automation`
- **Document and data entry automation** — Extracting structured data from documents into systems. `document-and-data-entry-automation`
- **Email automation** — Triage, drafting, and routing of inbox work. `email-automation`
- **Internal tools and app builders** — Building internal interfaces over existing data. `internal-tools-and-app-builders`
- **Robotic process automation** — Automating work across desktop and enterprise applications. `robotic-process-automation`
- **Task and research agents** — Agents that pursue a goal across several tools. `task-and-research-agents`
- **Workflow automation** — Connecting applications so a trigger causes a sequence of actions. `workflow-automation`

## Productivity and workflow

Getting personal and team work done: notes, meetings, mail, tasks, and time.

- **Calendar and scheduling** — Arranging time and coordinating availability. `calendar-and-scheduling`
- **Email assistants** — Drafting, summarising, and prioritising mail. `email-assistants`
- **Knowledge management** — Connecting notes, documents, and references into something searchable. `knowledge-management`
- **Meeting assistants** — Recording, transcribing, and summarising meetings. `meeting-assistants`
- **Note taking** — Capturing and organising written notes. `note-taking`
- **Personal automation** — Small automations for an individual's own routine. `personal-automation`
- **Task and project management** — Planning, assigning, and tracking work. `task-and-project-management`
- **Workplace search** — Searching across the applications an organisation uses. `workplace-search`

## Presentations and documents

Producing and working with documents.

- **Contract review** — Reading agreements for terms, risks, and deviations. `contract-review`
- **Diagrams and whiteboards** — Producing charts, diagrams, and visual thinking surfaces. `diagrams-and-whiteboards`
- **Document extraction** — Pulling structured fields out of forms, invoices, and contracts. `document-extraction`
- **Document generation** — Assembling documents from templates and data. `document-generation`
- **PDF and document chat** — Asking questions of a document and getting cited answers. `pdf-and-document-chat`
- **Presentation generation** — Building slide decks from an outline or a document. `presentation-generation`

## Design and creative

Visual and product design work.

- **3D and modelling** — Generating and editing three-dimensional assets. `3d-and-modelling`
- **Branding** — Identity systems, naming, and brand guidelines. `branding`
- **Design collaboration** — Reviewing, handing off, and versioning design work. `design-collaboration`
- **Graphic design** — Layout and composition for print and screen. `graphic-design`
- **Interior and architecture** — Spaces, rendering, and architectural visualisation. `interior-and-architecture`
- **Prototyping** — Turning an idea into something clickable quickly. `prototyping`
- **UI and UX design** — Interface layout, components, and interaction design. `ui-and-ux-design`

## Marketing and advertising

Reaching and converting an audience.

- **Advertising** — Creating, targeting, and optimising paid campaigns. `advertising`
- **Audience research** — Understanding who the audience is and what they want. `audience-research`
- **Competitive intelligence** — Tracking what competitors publish, price, and launch. `competitive-intelligence`
- **Content marketing** — Planning and producing content that earns attention. `content-marketing`
- **Conversion optimisation** — Improving the rate at which visitors take an action. `conversion-optimisation`
- **Email marketing** — Campaigns, sequences, and lifecycle messaging. `email-marketing`
- **Influencer and affiliate** — Finding and managing third-party promotion. `influencer-and-affiliate`
- **Marketing analytics** — Attribution, reporting, and channel measurement. `marketing-analytics`
- **Personalisation** — Varying content and offers by visitor. `personalisation`
- **Social media management** — Scheduling, publishing, and responding across social platforms. `social-media-management`

## SEO and search

Being found in search, classic and generative.

- **AI search visibility** — Appearing in generative answers and AI assistants. `ai-search-visibility`
- **Backlinks and digital PR** — Earning and monitoring links from other sites. `backlinks-and-digital-pr`
- **Content optimisation** — Shaping a page to match what a query needs. `content-optimisation`
- **Internal linking** — Connecting pages so authority and readers flow between them. `internal-linking`
- **Keyword research** — Finding what an audience searches for and how often. `keyword-research`
- **Local SEO** — Visibility in maps, local packs, and location queries. `local-seo`
- **Programmatic SEO** — Generating and maintaining pages at scale from data. `programmatic-seo`
- **Rank tracking** — Monitoring position for tracked queries over time. `rank-tracking`
- **Structured data** — Marking pages up so machines can read their meaning. `structured-data`
- **Technical SEO** — Crawling, indexing, structure, and page performance. `technical-seo`

## Sales and CRM

Finding, working, and closing revenue.

- **Conversation intelligence** — Recording and analysing sales calls. `conversation-intelligence`
- **CRM assistants** — Keeping the customer record current and useful. `crm-assistants`
- **Data enrichment** — Filling in missing detail on people and companies. `data-enrichment`
- **Proposals and quoting** — Producing quotes, proposals, and pricing documents. `proposals-and-quoting`
- **Prospecting and lead generation** — Identifying and reaching potential buyers. `prospecting-and-lead-generation`
- **Revenue forecasting** — Predicting pipeline outcomes and quota attainment. `revenue-forecasting`
- **Sales engagement** — Sequencing and managing outbound contact. `sales-engagement`

## Customer support

Answering and resolving customer problems.

- **Customer feedback analysis** — Finding themes across reviews, tickets, and surveys. `customer-feedback-analysis`
- **Helpdesk assistants** — Drafting, summarising, and routing inside a ticketing system. `helpdesk-assistants`
- **Knowledge base tools** — Writing and maintaining the articles support answers from. `knowledge-base-tools`
- **Quality assurance** — Scoring conversations against a rubric. `quality-assurance`
- **Support chatbots** — Automated answering of customer questions. `support-chatbots`
- **Voice support** — Handling inbound and outbound calls. `voice-support`

## Data and analytics

Turning data into answers, from preparation through analysis to a chart.

- **Business intelligence** — Dashboards, metrics, and self-serve reporting. `business-intelligence`
- **Conversational analytics** — Asking questions of a dataset in plain language. `conversational-analytics`
- **Data preparation** — Cleaning, joining, and reshaping data for use. `data-preparation`
- **Data visualisation** — Charting and presenting quantitative findings. `data-visualisation`
- **Predictive modelling** — Forecasting and scoring from historical data. `predictive-modelling`
- **Spreadsheets** — Formula help, analysis, and automation inside a sheet. `spreadsheets`
- **Web and product analytics** — Measuring behaviour in a site or product. `web-and-product-analytics`

## Research and knowledge

Finding, reading, and synthesising sources.

- **Academic search** — Searching the scholarly literature by paper, author, and citation. `academic-search`
- **Citation management** — Collecting references and formatting them. `citation-management`
- **Deep research agents** — Multi-step research producing a cited report. `deep-research-agents`
- **Fact checking** — Verifying claims against sources and flagging the ones that do not hold. `fact-checking`
- **Literature review** — Screening and synthesising evidence across many papers. `literature-review`
- **Market research** — Sizing, segmenting, and understanding a market. `market-research`
- **Paper reading** — Explaining and interrogating a single document. `paper-reading`
- **Survey and qualitative research** — Designing studies and analysing open-ended responses. `survey-and-qualitative-research`

## Education and learning

Teaching, studying, and training, in classrooms and at work.

- **Assessment and marking** — Setting and grading work against criteria. `assessment-and-marking`
- **Corporate training** — Onboarding, compliance, and skills development at work. `corporate-training`
- **Course creation** — Building lessons, curricula, and learning materials. `course-creation`
- **Language learning** — Practising a language with feedback. `language-learning`
- **Lesson planning** — Preparing what happens in a class. `lesson-planning`
- **Study tools** — Flashcards, revision plans, and practice questions. `study-tools`
- **Tutoring and explanation** — Working through a subject with a learner. `tutoring-and-explanation`

## Business and finance

Running the organisation: money, people, contracts, and obligations.

- **Accounting and bookkeeping** — Recording, reconciling, and reporting on money. `accounting-and-bookkeeping`
- **Compliance and risk** — Meeting obligations and evidencing that you did. `compliance-and-risk`
- **Ecommerce operations** — Catalogue, merchandising, fulfilment, and returns. `ecommerce-operations`
- **Financial analysis** — Modelling, forecasting, and interpreting financial data. `financial-analysis`
- **Human resources** — Hiring, onboarding, and people operations. `human-resources`
- **Invoicing and payments** — Billing customers, chasing payment, and reconciling what arrives. `invoicing-and-payments`
- **Legal work** — Drafting, reviewing, and researching legal material. `legal-work`
- **Procurement and vendors** — Sourcing, contracting, and managing suppliers. `procurement-and-vendors`

## Health and lifestyle

Personal wellbeing and daily life.

- **Accessibility** — Captioning, description, and adaptation for disabled users. `accessibility`
- **Clinical documentation** — Producing notes and records from a consultation. `clinical-documentation`
- **Fitness and nutrition** — Training plans, food logging, and coaching. `fitness-and-nutrition`
- **Home and personal life** — Cooking, shopping, admin, and household organisation. `home-and-personal-life`
- **Mental wellbeing** — Journalling, reflection, and supportive conversation. `mental-wellbeing`
- **Travel planning** — Itineraries, booking, and destination research. `travel-planning`

## Schema

One record per category, at either level. The machine-readable version is
[`data/schema.json`](data/schema.json).

| Field | Type | Notes |
|---|---|---|
| `name` | string | Display name, sentence case |
| `slug` | string | Stable identifier, unique across both levels. Derived from the name, but it does not change when the name does |
| `parent` | string or null | Slug of the level-1 parent. `null` at level 1 |
| `level` | integer | `1` or `2`. There is no level 3, on purpose |
| `description` | string | One sentence, 5 to 22 words |
| `aliases` | array of strings | Other names for the same category, including American spellings and common abbreviations |
| `children` | array of strings | Slugs of the level-2 children. Empty at level 2 |
| `last_reviewed` | string | ISO `YYYY-MM-DD` |

The tree is checked before release: every `parent` resolves, every `children` entry
resolves, no name appears twice anywhere in the tree, and no level-2 node has children of
its own.

## How categories are selected

A category earns a place when it answers a question a person actually arrives with. "Text to
image" is a category because people search for it. "Generative visual synthesis" is not,
because nobody does.

The rules the tree is built to:

- **Two levels, never three.** A third level is where taxonomies go to die: it produces
  nodes with one member, and it forces a judgement call on every new tool.
- **Six to twelve children per top-level category.** Below six, the level is not carrying its
  weight and the children belong one level up. Above twelve, the category is really two.
- **Named by the job, not the technology.** `Meeting assistants`, not `Multimodal
  transcription and summarisation`.
- **Aliases carry the variants.** `personalization`, `tts`, `cro`, and `localization` are
  aliases rather than separate nodes, so a lookup succeeds whichever a user types.
- **No vendor-specific nodes.** A category named after one product is a product page.

What is deliberately absent: a third level, categories that exist only as a marketing
phrase, industry verticals (a taxonomy of tools is not a taxonomy of customers), and any node
that could not hold at least a handful of distinct products.

## Using the data

Build the tree:

```python
import json

nodes = json.load(open("data/categories.json"))
by_slug = {n["slug"]: n for n in nodes}
for top in (n for n in nodes if n["level"] == 1):
    print(top["name"])
    for c in top["children"]:
        print("   ", by_slug[c]["name"])
```

Resolve whatever a user typed, aliases included:

```python
def resolve(q, nodes):
    q = q.strip().lower()
    for n in nodes:
        if n["slug"] == q or n["name"].lower() == q:
            return n
        if q in [a.lower() for a in n["aliases"]]:
            return n
    return None
```

Roll a level-2 slug up to its top-level category:

```python
def top_level(slug, by_slug):
    n = by_slug[slug]
    return by_slug[n["parent"]] if n["parent"] else n
```

Validate before you depend on it:

```bash
pip install check-jsonschema
check-jsonschema --schemafile data/schema.json data/categories.json
```

Slugs are the contract. Names get edited for clarity; slugs do not change, so anything you
key on them keeps working across releases.

## Known limitations

- **A taxonomy is an opinion.** This one is shaped by what people search for and what a
  directory has to file. Another defensible tree would put document extraction under
  automation rather than documents, and would not be wrong.
- **Some tools belong in several places.** The taxonomy does not solve that; it gives you
  stable nodes to file against, and the decision of whether to allow multiple assignments is
  yours.
- **No vertical categories.** Healthcare, legal, and education appear as work, not as
  industries. A tool sold to hospitals is still a transcription tool.
- **Two levels means some nodes are broad.** `Workflow automation` covers a great deal. That
  is the cost of refusing a third level, and it is a cost worth paying.

## Suggest a category

- [Suggest a category](../../issues/new?template=suggest-a-category.yml) — a form, two
  minutes.
- [Report a broken link](../../issues/new?template=report-a-broken-link.yml) — for anything
  here that points somewhere it should not.

The most useful suggestions are the ones with evidence behind them: a category you needed and
could not find a node for, and the tools that would sit in it. A proposal for a node with two
plausible members will be turned down, politely and with the reason.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md). One category per pull request, name it by the job it
does, and say which existing node it would be taken out of.

## Disclaimer

This is an editorial taxonomy, not a standard. It is published because a usable shared tree is
more valuable than a perfect private one, and it will change as the field does. Nothing here
is an endorsement of any product, and no product is named in the dataset at all.

## License

[CC BY 4.0](LICENSE). Use it in a commercial directory, adapt it, extend it, as long as you
credit TiorAI and say what you changed.

The licence covers the category names, descriptions, and structure. It does not cover the
TiorAI name or logo.

## About TiorAI

[TiorAI](https://tiorai.com/) is an AI tools directory. Filing several thousand products means
having a tree to file them in; this is that tree, published separately so other people do not
have to invent their own.

- [AI tools directory](https://tiorai.com/tools/)
