# AI Visibility Glossary

> A developer-oriented glossary of the concepts, terminology, metrics, and technical processes behind **AI Visibility**.

## Overview

AI Visibility is the ability of a brand, company, product, website, organization, person, or source to be **discovered, understood, mentioned, cited, represented, and recommended by AI-powered search and answer systems**.

Traditional SEO primarily asks:

> “Where does this page rank in a search engine?”

AI Visibility asks a broader question:

> “When someone asks an AI system a relevant question, does the system know who we are, understand what we offer, consider our information, mention us, cite us, or recommend us?”

For developers, this creates an interesting technical problem.

AI Visibility sits at the intersection of:

* Information Retrieval
* Search
* Entity Understanding
* Content Architecture
* Knowledge Bases
* Semantic Search
* Retrieval-Augmented Generation
* Source Selection
* Ranking
* Citations
* Recommendations
* Brand Representation
* Measurement and monitoring

This glossary is designed to provide a common vocabulary for understanding that ecosystem.

---

## Why an AI Visibility Glossary?

AI search systems introduce concepts that do not map perfectly to traditional SEO terminology.

A website can have excellent traditional search rankings and still have weak visibility in AI-generated answers.

For example, imagine a user asks:

> “What are the best project management platforms for a 20-person remote agency?”

An AI system may need to:

1. Understand the user's intent.
2. Identify the relevant entities.
3. Interpret “20-person” and “remote agency”.
4. Retrieve relevant information.
5. Generate a candidate set of sources.
6. Evaluate those sources.
7. Apply contextual or eligibility constraints.
8. Select useful information.
9. Generate an answer.
10. Mention specific products.
11. Cite supporting sources.
12. Recommend one or more products.

Each step creates potential visibility opportunities or failure points.

The purpose of this glossary is to give developers and practitioners precise language for those processes.

---

# Core AI Visibility Concepts

## AI Visibility

The degree to which an entity is discovered, understood, mentioned, cited, represented, or recommended by AI-powered search and answer systems.

AI Visibility is the overall outcome.

It can be measured through signals such as:

* Brand mentions
* Citations
* Recommendations
* Brand position
* Query coverage
* Citation share
* Recommendation visibility
* Competitor visibility
* Brand representation
* Information accuracy

---

## Generative Engine Optimization (GEO)

The practice of improving a brand's information ecosystem so AI-powered search and answer systems can discover, understand, mention, cite, and recommend it.

GEO is generally considered an optimization discipline.

AI Visibility is the outcome being measured.

---

## Answer Engine Optimization (AEO)

The practice of structuring information so answer engines can understand and use it when responding to questions.

AEO focuses heavily on:

* Direct answers
* Question-based content
* Clear definitions
* Structured information
* Entity relationships
* Retrievable passages
* Useful supporting evidence

---

# Search and Retrieval

## AI Search

A search experience that uses AI to understand queries, retrieve information, synthesize answers, and potentially provide citations or recommendations.

Unlike traditional search, the output may be a generated response rather than simply a ranked list of URLs.

---

## Information Retrieval

The process of finding information relevant to a user's question.

A simplified AI search pipeline might look like:

```text
User Query
    ↓
Query Understanding
    ↓
Information Retrieval
    ↓
Candidate Generation
    ↓
Ranking / Re-Ranking
    ↓
Source Selection
    ↓
Answer Generation
    ↓
Citations / Recommendations
```

For AI Visibility, retrieval is critical because information that is never discovered has little opportunity to influence the final answer.

---

## Semantic Search

Search based on meaning and intent rather than exact keyword matching.

For example:

```text
"project management for distributed teams"
```

may be related to:

```text
"remote team collaboration software"
```

even though the wording is different.

This means AI Visibility cannot depend exclusively on exact keyword matching.

---

## Query Understanding

The process of interpreting what the user actually wants from a question.

This can include:

* Intent
* Topic
* Entities
* Audience
* Geography
* Industry
* Requirements
* Use case
* Constraints

For developers, query understanding is important because the same brand may be highly relevant for one interpretation of a query and irrelevant for another.

---

## Query Expansion

The process of broadening a query using related terms, concepts, entities, or context.

For example:

```text
"CRM for freelancers"
```

may be expanded conceptually toward:

```text
CRM for independent professionals
CRM for solo businesses
client management software
customer relationship management for freelancers
```

This increases the possible information that can be retrieved.

---

## Query Decomposition

Breaking a complex question into smaller information requirements.

For example:

> “What is the best CRM for a 10-person European B2B agency that needs email automation, reporting, and API access?”

could involve separate requirements:

```text
CRM category
+
10-person company
+
B2B
+
agency
+
Europe
+
email automation
+
reporting
+
API
```

A brand may satisfy some requirements but not others.

---

## Query Routing

The process of determining where or how a query should be handled.

Different questions may require different sources or retrieval mechanisms.

For example:

```text
"What does your product do?"
        → product information

"What is your current pricing?"
        → current pricing source

"What are the best alternatives?"
        → comparison/recommendation sources
```

---

# Entities and Knowledge

## Entity

A distinct, identifiable thing that an AI system can understand.

Examples include:

* Companies
* Brands
* Products
* People
* Organizations
* Locations
* Publications
* Services
* Events

For AI Visibility, entity clarity is fundamental.

---

## Entity Understanding

The ability of an AI system to correctly identify and understand an entity and its associated information.

A system should ideally understand:

```text
Company
 ├── Products
 ├── Services
 ├── Industry
 ├── Customers
 ├── Locations
 ├── Competitors
 └── Relationships
```

Poor entity understanding can result in incorrect recommendations, incorrect descriptions, or confusion between similarly named entities.

---

## Entity Relationship

A connection between identifiable entities.

Examples:

```text
Company → Product
Brand → Parent Company
Person → Organization
Product → Category
Company → Location
Company → Competitor
```

Entity relationships provide context that helps AI systems understand what a brand actually represents.

---

## Knowledge Base

An organized collection of information that can be used to understand entities, products, services, topics, and relationships.

A knowledge base might contain:

* Company information
* Product descriptions
* Services
* Documentation
* Pricing
* Locations
* Industries
* Customers
* Integrations
* Relationships
* FAQs

From an AI Visibility perspective, the goal is not simply to have information somewhere.

The information needs to be **clear, accurate, connected, and retrievable**.

---

# Retrieval Architecture

## Retrieval-Augmented Generation (RAG)

A system architecture in which relevant external information is retrieved and provided to a generative AI system before it produces an answer.

A simplified implementation looks like:

```text
User Question
      ↓
Query Processing
      ↓
Retriever
      ↓
Relevant Documents
      ↓
Context
      ↓
LLM
      ↓
Generated Answer
```

RAG matters to AI Visibility because a source generally needs to become available to the retrieval process before it can influence the generated answer.

---

## Embeddings

Numerical representations of text or other information that can be used to compare semantic meaning.

In AI Visibility systems, embeddings are commonly associated with semantic retrieval.

For example, two pieces of text may use different words but represent similar concepts.

Embeddings can therefore help systems discover information based on meaning rather than exact wording.

---

## Vector Search

A retrieval method that searches for information based on vector representations.

A simplified flow is:

```text
Query
  ↓
Embedding
  ↓
Vector Search
  ↓
Relevant Content
```

Vector search is particularly useful when users express an idea differently from the wording used in the source material.

---

## Hybrid Retrieval

A retrieval approach that combines multiple retrieval methods.

A common combination is:

```text
Keyword Retrieval
        +
Semantic Retrieval
        ↓
Combined Candidate Set
        ↓
Ranking
```

This can be valuable because exact terminology remains important for entities, product names, technical terms, and regulations, while semantic retrieval helps discover conceptually related information.

---

## Passage Retrieval

The process of finding specific sections of a document rather than retrieving an entire document.

For example, an AI system may retrieve only:

```text
"Enterprise plans support up to 5,000 users."
```

from a long pricing document.

This makes content structure important for AI Visibility.

---

## Chunking

Dividing larger documents into smaller meaningful pieces that can be retrieved independently.

Good chunks should retain enough context to make sense when retrieved separately.

For example:

```text
## CRM for Small Agencies

Our CRM is designed for agencies with 5–50 employees.

### Email Automation

The platform supports automated follow-up sequences...
```

is generally more useful than arbitrary text fragments with no identifiable context.

---

## Contextual Retrieval

Retrieval that preserves enough surrounding information for the retrieved content to be interpreted correctly.

Consider:

> “It supports up to 50 users.”

Without context, “it” is ambiguous.

A clearer version is:

> “Acme CRM supports teams of up to 50 users.”

Explicit context improves the chance that retrieved information is associated with the correct entity.

---

# Ranking and Selection

## Candidate Generation

The process of creating an initial set of potentially relevant sources.

Potential candidates may include:

* Company websites
* Product pages
* Documentation
* Research
* Industry publications
* Reviews
* Comparison websites
* Professional organizations
* Expert articles

Candidate generation is important because a source that never enters the candidate set has little opportunity to be selected later.

---

## Top-k Retrieval

Selecting a limited number of the most relevant results from a larger candidate pool.

If a system retrieves the top 10 sources, a source ranked outside that set may have substantially less opportunity to influence the final response.

---

## First-Stage Retrieval

The initial retrieval process used to find a broad set of potentially relevant information.

Its goal is generally discovery rather than final selection.

---

## Second-Stage Retrieval

A deeper evaluation or retrieval stage applied to information already identified as potentially relevant.

The exact architecture differs between systems, but the general idea is:

```text
Broad Discovery
      ↓
Deeper Evaluation
      ↓
Final Candidate Set
```

---

## Re-Ranking

The process of evaluating retrieved results again and changing their order according to additional relevance signals.

Potential signals include:

* Query relevance
* Context
* Entity relationships
* Source authority
* Specificity
* Recency
* Evidence
* Audience fit
* Geographic relevance
* Product suitability

---

## Document Ranking

The process of ordering documents according to their relevance or usefulness for a particular query.

A document may rank differently for different questions.

For example, a pricing page may be highly relevant for:

> “How much does Product X cost?”

but much less relevant for:

> “What are the best project management tools for remote teams?”

---

## Metadata Filtering

Using descriptive information about a source to narrow the available information.

Metadata can include:

* Date
* Author
* Language
* Geography
* Content type
* Product category
* Organization
* Topic

Metadata can help systems identify which information is appropriate for a particular query.

---

## Pre-Filtering

Removing information before deeper retrieval or ranking takes place.

For example, a query asking for:

> “Cybersecurity providers in the Netherlands”

may require geographic filtering before more detailed relevance evaluation.

---

## Post-Filtering

Applying additional requirements after potentially relevant information has already been retrieved.

For example:

```text
Retrieve project management tools
        ↓
Check European availability
        ↓
Check mobile application
        ↓
Check time tracking
        ↓
Final candidates
```

---

# Sources and Citations

## Source Selection

The process of deciding which discovered sources should actually contribute to an answer.

Being discoverable does not guarantee selection.

A system may discover ten sources but use only three.

---

## Source Authority

The degree to which a source is considered credible, knowledgeable, trustworthy, and useful for a particular subject.

Authority is contextual.

For example:

* A government source may be authoritative for regulations.
* A vendor may be authoritative about its own product specifications.
* An academic publication may be authoritative for scientific research.

---

## Citation Quality

The overall usefulness and reliability of a source citation.

Factors can include:

* Relevance
* Authority
* Accuracy
* Specificity
* Evidence
* Context
* Freshness

Citation quantity alone is not sufficient.

---

## Citation Relevance

The degree to which a cited source actually relates to the question or claim being answered.

A highly authoritative source can still be a poor citation if it does not address the specific question.

---

## Citation Accuracy

The degree to which an AI-generated statement correctly represents the information contained in the cited source.

For example, if a source states:

> “The standard plan supports up to 50 users.”

an AI answer claiming:

> “The product supports unlimited users.”

would represent a citation accuracy problem.

---

## Citation Coverage

The breadth with which a brand's relevant sources are cited across important queries and topics.

Possible query groups include:

* Product
* Category
* Comparison
* Recommendation
* Industry
* Geography
* Customer type
* Use case
* Pricing
* Features

---

## Citation Share

The proportion of citation visibility associated with a brand compared with competitors within a defined query set.

For example:

```text
Brand A: 40%
Brand B: 30%
Brand C: 20%
Other:   10%
```

The methodology and query set must always be defined.

---

## Citation Position

The prominence of a citation within an AI-generated response or citation set.

A citation appearing prominently in an answer may have greater visibility than one appearing much later.

Citation position should not be confused with traditional search-engine ranking.

---

## Citation Persistence

The degree to which a source continues to be cited across repeated queries, query variations, and time.

A citation that appears once is not necessarily evidence of stable AI Visibility.

---

## Citation Diversity

The variety of sources and source types that contribute citations for a brand or topic.

A healthy citation ecosystem might include:

```text
Company documentation
Industry publication
Independent review
Research report
Professional organization
Customer case study
```

rather than relying exclusively on one source.

---

# Brand Visibility

## Brand Mention

A direct appearance of a brand, company, product, organization, or person in an AI-generated answer.

A mention does not necessarily mean recommendation.

---

## Brand Representation in AI

How an AI system describes, positions, and contextualizes a brand.

This can include:

* What the company does
* Products
* Target customers
* Industries
* Strengths
* Weaknesses
* Pricing position
* Competitors
* Geographic coverage
* Use cases

AI Visibility therefore requires more than simply appearing in an answer.

The information must also be represented accurately.

---

## Brand Authority

The degree to which a brand is recognized as credible, knowledgeable, and relevant within a particular market or subject.

Brand authority can be influenced by:

* Expertise
* Original research
* Industry recognition
* Independent coverage
* Customer evidence
* Consistent information

---

## Brand Reputation

The broader perception of a brand across information sources, reviews, publications, communities, customers, and other references.

Reputation can influence how AI systems describe and evaluate a company.

---

## Information Consistency

The degree to which important facts remain aligned across the sources AI systems may encounter.

For example:

```text
Company website: 50 users
Documentation:   50 users
Directory:       100 users
Review site:     100 users
```

Conflicting information can make entity understanding and accurate representation more difficult.

---

## Information Accuracy

The degree to which information about a brand, product, service, person, or topic is factually correct and current.

Accuracy is particularly important for:

* Pricing
* Product features
* Integrations
* Availability
* Ownership
* Locations
* Plans
* Regulations
* Product limits

---

# Recommendations

## AI Recommendation Visibility

The degree to which a brand or product appears as a recommendation in AI-generated answers.

This is different from simply being mentioned.

For example:

> “Brand X is one of several companies in this category.”

is different from:

> “For a 10-person remote agency, Brand X would be a strong choice.”

The second represents recommendation visibility.

---

## Recommendation Context

The specific situation surrounding an AI recommendation.

Context may include:

* User type
* Company size
* Industry
* Geography
* Budget
* Use case
* Required features
* Technical requirements

---

## Recommendation Criteria

The characteristics or requirements used to determine which options are suitable.

For example:

```text
Customer: small agency
Location: Europe
Feature: API
Feature: email automation
Budget: moderate
```

---

## Recommendation Eligibility

Whether a product or service satisfies the basic conditions necessary to be considered.

A product unavailable in a user's country may fail eligibility even if it is otherwise highly relevant.

---

## Recommendation Relevance

How well a recommendation matches the user's actual needs and context.

A product can be factually suitable for the broad category but still be a poor recommendation for a specific user.

---

## Recommendation Accuracy

Whether the recommendation is based on correct information and correctly matches the product to the user's requirements.

AI Visibility should not be optimized simply for more recommendations.

The goal should be **accurate recommendations to appropriate audiences**.

---

## Recommendation Evidence

Information supporting why a brand or product should be considered.

Examples include:

* Product documentation
* Case studies
* Original research
* Customer evidence
* Independent reviews
* Technical analysis
* Industry reports
* Demonstrated capabilities

Marketing claims alone are not necessarily strong recommendation evidence.

---

# Measurement

## Query Coverage

The percentage or breadth of relevant questions across which a brand becomes visible.

A useful query set might include:

```text
Category queries
Recommendation queries
Comparison queries
Alternative queries
Industry queries
Customer-type queries
Geographic queries
Feature queries
Use-case queries
Problem-solving queries
```

---

## Brand Mention Rate

The percentage of tested relevant AI answers in which a particular brand appears.

Example:

```text
100 relevant queries tested
65 contain Brand A

Brand Mention Rate = 65%
```

The query methodology must be defined.

---

## Brand Mention Share

The percentage of relevant brand mentions belonging to a specific brand within a defined competitive query set.

This differs from Brand Mention Rate because the denominator is the total number of relevant brand mentions rather than the number of queries.

---

## Brand Position in AI Answers

The relative prominence of a brand within an AI-generated response.

For example:

```text
1. Brand A
2. Brand B
3. Brand C
```

Position should always be interpreted in context.

---

## Competitor Visibility in AI

The visibility of competing brands across the same AI query landscape.

Competitive measurement can reveal:

* Queries where competitors appear
* Queries where the brand is absent
* Industries where competitors dominate
* Use cases where competitors are recommended
* Citation gaps
* Geographic gaps

---

## AI Visibility Share

The proportion of relevant AI visibility associated with a brand compared with competitors.

A methodology may combine:

* Mentions
* Recommendations
* Citations
* Position
* Query coverage
* Product appearances

There is no universal formula, so the measurement methodology should always be documented.

---

## AI Visibility Gap

An area where a brand has weaker or missing AI visibility compared with expectations or competitors.

Examples:

```text
Strong visibility:
General category queries

Weak visibility:
Healthcare queries

No visibility:
European healthcare queries
```

A visibility gap does not automatically mean more content is needed.

The underlying reason should be investigated first.

---

## AI Visibility Opportunity

A specific situation where a brand has a realistic opportunity to improve AI Visibility.

For example:

```text
Competitors are frequently recommended
for "CRM for small European agencies"

The product actually supports this audience
but the website does not clearly communicate it.

Opportunity:
Improve audience + geography + use-case information.
```

---

## AI Visibility Benchmark

A defined baseline used to compare AI Visibility over time or against competitors.

A benchmark should define:

* Query set
* Query groups
* Competitors
* AI platforms
* Metrics
* Measurement rules
* Date
* Segmentation

Consistency is critical.

---

## AI Visibility Trend

The direction of AI Visibility over time.

Possible trends include:

* Increasing
* Decreasing
* Stable
* Expanding into new query groups
* Losing visibility to competitors
* Becoming more concentrated

A trend should be interpreted alongside accuracy and quality.

---

## AI Visibility Volatility

The degree to which AI Visibility changes across repeated queries, query variations, or time.

High volatility can appear as:

```text
Query A → Brand mentioned
Query B → Brand absent
Query C → Brand recommended
Query D → Competitor recommended
```

Some variation is normal. The goal is to distinguish normal contextual variation from meaningful instability.

---

# Monitoring

## AI Visibility Monitoring

The ongoing process of tracking how a brand appears across AI-generated answers.

Monitoring can include:

* Mentions
* Citations
* Recommendations
* Brand position
* Competitor visibility
* Brand representation
* Accuracy
* Source changes

---

## AI Search Monitoring

A broader practice covering the AI search environment itself.

It can include monitoring:

* Brands
* Competitors
* Sources
* Citations
* Recommendations
* Query behavior
* Representation
* Changes in AI search results

---

## AI Visibility Alert

A notification triggered when a meaningful change occurs.

Examples:

```text
Brand mention rate drops 15%
```

```text
Primary product disappears from recommendations
```

```text
Competitor becomes dominant for a strategic query group
```

```text
AI begins describing a product incorrectly
```

An alert should provide enough context to investigate the underlying cause.

---

# Trust and Authority

## Trust Signals

Information or evidence that helps demonstrate credibility and reliability.

Examples include:

* Independent reviews
* Expert commentary
* Original research
* Case studies
* Clear company information
* Author expertise
* Technical documentation
* Customer evidence
* Professional recognition

---

## Third-Party Recognition

Independent references or acknowledgment of a company, product, person, or area of expertise.

Examples:

* Industry publications
* Professional organizations
* Research
* Expert interviews
* Independent reviews
* Industry reports
* Conferences
* Credible directories

Quality and relevance matter more than raw mention volume.

---

## Expertise Signals

Evidence demonstrating genuine knowledge, experience, or specialization.

Examples:

* Professional experience
* Research
* Technical documentation
* Expert authorship
* Case studies
* Specialized products
* First-hand data
* Industry contributions

---

## Original Research

New data, analysis, findings, or information produced directly by an organization or expert.

Examples:

* Surveys
* Market studies
* Proprietary datasets
* Experiments
* Benchmarks
* Technical investigations
* Customer research

Original research can create both direct citation opportunities and third-party recognition.

---

## Content Authority

The credibility, usefulness, expertise, and evidence associated with a specific piece of content.

Content authority is page- or resource-specific.

---

## Topical Authority

The degree to which a brand or source is recognized as knowledgeable and comprehensive within a particular subject.

Topical authority is broader than the authority of one individual article.

---

## Content Trustworthiness

The degree to which information is accurate, reliable, transparent, and dependable.

Trustworthiness is especially important when AI systems encounter conflicting information.

---

# Content and Information Architecture

AI Visibility is not simply a content-volume problem.

A technically strong AI Visibility strategy requires information to be:

```text
Discoverable
      ↓
Understandable
      ↓
Contextualized
      ↓
Retrievable
      ↓
Relevant
      ↓
Trustworthy
      ↓
Selectable
      ↓
Citable / Usable
```

Developers therefore have an important role.

Technical implementation can affect:

* Content accessibility
* Page structure
* Metadata
* Internal relationships
* Structured information
* Documentation
* URLs
* Content hierarchy
* Product/entity relationships
* Freshness
* API and machine-readable information

---

# A Developer's AI Visibility Checklist

When developing a website intended to perform well in AI search environments, consider the following.

## 1. Make entities explicit

Clearly identify:

```text
Company
Product
Service
Industry
Audience
Location
Parent company
Related products
Competitors
```

Avoid forcing AI systems to infer basic relationships from vague language.

---

## 2. Create clear content boundaries

A page should have a recognizable purpose.

For example:

```text
/products/crm
/pricing
/integrations
/industries/healthcare
/use-cases/remote-agencies
/resources/research
/documentation/api
```

Clear information architecture can make retrieval and interpretation easier.

---

## 3. Write self-contained sections

Important information should remain understandable when retrieved independently.

Prefer:

> “Acme CRM supports teams of up to 50 users.”

over:

> “It supports up to 50 users.”

---

## 4. Document limitations

AI systems need to understand not only what a product does, but also what it does not do.

Useful information includes:

* Limitations
* Availability
* Supported countries
* Plan restrictions
* Feature requirements
* Integration requirements
* Customer-size limitations

This can improve recommendation accuracy.

---

## 5. Maintain information consistency

Check important facts across:

```text
Website
Documentation
Product pages
Business profiles
Directories
Reviews
Publications
Partner pages
Knowledge bases
```

Conflicting information can create entity and representation problems.

---

## 6. Build evidence

Support important claims with:

* Research
* Data
* Documentation
* Case studies
* Independent sources
* Expert analysis
* Customer evidence

Do not rely exclusively on promotional statements.

---

## 7. Test real questions

Do not evaluate AI Visibility using only keywords.

Build query sets based on realistic user questions.

For example:

```text
What is the best CRM for a small agency?

What CRM is good for a remote agency?

What CRM has strong API support?

What are alternatives to Brand X?

What CRM works well for European agencies?
```

---

# Example AI Visibility Measurement Model

A simple internal data model could look like:

```json
{
  "query": "best CRM for small European agencies",
  "platform": "ai-search",
  "brand": "Example CRM",
  "mentioned": true,
  "recommended": true,
  "brand_position": 2,
  "citation_present": true,
  "citation_position": 1,
  "representation_accurate": true,
  "recommendation_relevant": true,
  "competitors": [
    "Competitor A",
    "Competitor B"
  ]
}
```

Aggregating these observations can produce higher-level metrics such as:

```text
Brand Mention Rate
Query Coverage
Citation Coverage
Citation Share
Recommendation Visibility
Recommendation Position
AI Visibility Share
Competitor Visibility
AI Visibility Trend
AI Visibility Gap
```

---

# AI Visibility as an Engineering Problem

AI Visibility should not be treated exclusively as a marketing problem.

It can also be viewed as an information systems problem.

A simplified model is:

```text
                ┌──────────────────┐
                │   User Question  │
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │ Query Understanding│
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │    Retrieval     │
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │ Candidate Sources│
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │ Ranking / Filters│
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │ Source Selection │
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │ Answer Generation│
                └────────┬─────────┘
                         ↓
             ┌───────────┴───────────┐
             ↓                       ↓
        Citations               Recommendations
             ↓                       ↓
       Brand Visibility       Brand Visibility
```

At each stage, there are different opportunities for a brand to become visible—or disappear.

---

# Building an AI Visibility Testing System

A developer building an AI Visibility monitoring system could structure the workflow as follows:

```text
1. Define target entities
2. Define competitors
3. Build representative query sets
4. Group queries by intent/context
5. Execute queries
6. Store raw AI responses
7. Extract brand mentions
8. Extract citations
9. Extract recommendations
10. Determine positions
11. Evaluate representation
12. Compare competitors
13. Calculate metrics
14. Detect changes
15. Investigate causes
16. Report opportunities
```

A database might contain entities such as:

```text
queries
brands
competitors
responses
mentions
citations
recommendations
sources
positions
query_groups
measurements
alerts
```

This creates the foundation for an AI Visibility analytics platform.

---

# Important Principle

The most important principle in AI Visibility is:

> **Do not optimize only for being mentioned. Optimize for being correctly understood, relevantly retrieved, accurately represented, appropriately recommended, and supported by trustworthy information.**

A brand that appears frequently but is misunderstood can have poor AI Visibility quality.

A brand that is cited frequently but for irrelevant queries may have poor strategic visibility.

A brand that is recommended to the wrong audience may have high visibility but poor recommendation accuracy.

Therefore, AI Visibility should be treated as a multidimensional system.

---

# Glossary Categories

The glossary can be organized into the following major categories:

1. **AI Visibility Fundamentals**
2. **GEO & AI Visibility**
3. **AI Search & Discovery**
4. **Entities & Citations**
5. **AI Retrieval & Ranking**
6. **Brand Visibility in AI**
7. **AI Recommendations**
8. **AI Search Measurement**
9. **AI Visibility Optimization**
10. **Content & Information Architecture**
11. **AI Search Platforms**
12. **AI Visibility Strategy**
13. **AI Visibility Analytics**
14. **Trust, Authority & Reputation**
15. **AI Search Monitoring**

Each term should belong to a clearly defined category so the glossary remains focused on AI Visibility rather than becoming a general AI or machine-learning dictionary.

---

# Scope

This glossary intentionally focuses on concepts that directly contribute to understanding, measuring, improving, or practicing AI Visibility.

It does **not** attempt to become a general machine-learning glossary.

For example, low-level concepts such as:

* Transformer architecture
* Backpropagation
* Gradient descent
* Activation functions
* Optimizers
* Epochs
* Batch sizes

are generally outside the scope unless they directly contribute to an AI Visibility concept.

The goal is not to document how an AI model is trained.

The goal is to document **how information becomes visible to AI systems and how developers can understand, measure, and improve that visibility.**

---

# Contributing

Contributions are welcome.

When proposing a new glossary term, ask:

### Does this term directly relate to AI Visibility?

It should help explain at least one of the following:

* How AI discovers information
* How AI understands entities
* How AI retrieves information
* How AI selects sources
* How AI cites information
* How AI recommends products or brands
* How brands are represented
* How AI Visibility is measured
* How AI Visibility can be monitored
* How AI Visibility can be improved
* How developers can structure information for AI systems

Avoid adding generic AI or machine-learning terminology that does not have a meaningful connection to AI Visibility.

---

# Goal

The long-term goal of this project is to build a comprehensive **AI Visibility Glossary** containing hundreds of focused terms.

The first milestone is:

> **300 useful AI Visibility terms.**

The priority, however, is relevance and quality—not reaching an arbitrary number.

A smaller glossary containing highly relevant concepts is more valuable than a large glossary filled with generic AI terminology.

---

# License

Add the project's preferred license here, for example:

```text
MIT License
```

or replace this section with the license used by the repository.

---

## Final Thought

AI Visibility is becoming an important layer between traditional web content and AI-generated answers.

For developers, the central challenge is no longer simply:

> “Can a search engine find my page?”

It is increasingly:

> **“Can an AI system discover the right information, understand what it means, connect it to the right entity, trust it, retrieve it for the right question, and use it accurately in an answer?”**

That is the problem this glossary is designed to help define.
