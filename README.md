# Cognitive Search & ChatGPT Hack

--THIS IS A WORKING DOCUMENT AND IS (VERY) INCOMPLETE--

# Hack Purpose
Customers are confused as to where Azure Cognitive Search (ACS) comes into the picture when using ChatGPT with their data. The hack is to crystalise the capabilities and value offering that ACS gives in the minds of CSAs and others so that they can have a customer conversation. Benefits include:
1. Data ingestion from many sources
2. Data enrichment
3. Vector search
4. Fast indexed data store

# Content
This repo is the basis - https://techcommunity.microsoft.com/t5/azure-ai-services-blog/revolutionize-your-enterprise-data-with-chatgpt-next-gen-apps-w/ba-p/3762087. It is a very common and simple pattern for this scenario.

The idea of the hack is to produce the search and generative parts of this solution by hand, in the portal or via CLR - i.e. not via a script. The hackers learn how to create the resources, ingest and enrich data, query the data, and understand what the different capabilities actually bring in practice.

![Imgur](https://github.com/ianlcurtis1/cog-search-and-chatgpt-hack/blob/main/Architecture.png)

# Hack Away!
The hack will not build a UI, hackers will query the data via AI Studio.

Hands on creation of the:
1. Blob storage
  - Uploaded data files
2. Cognitive Search
  - Indexes
3. OpenAI
  - GPT-4

Hackers will show comparative quality in response
- Demonstrate what the different aspects of Cognitive Search bring
- Run the prompt against data grounded against ChatGPT model (no Cognitive Search)
- Run the same prompt against Cog Search with Indexes and enrichment
- Run the same prompt against Cog Search with vectors (similarity)

# Stretch
Filtered search https://github.com/jometzg/openai-chat-rest-examples/blob/main/filtered-search-with-embeddings.md
