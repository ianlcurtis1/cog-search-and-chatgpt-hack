# Cognitive Search & ChatGPT Hack

--THIS IS A WORKING DOCUMENT AND IS (VERY) INCOMPLETE--

# Hack Purpose
Customers are confused as to where Azure Cognitive Search (ACS) comes into the picture when using ChatGPT with their data. The hack is to crystalise the capabilities and value offering that ACS gives (in combination with GPT models) in the minds of CSAs and others so that they can have an informed customer conversation. Benefits include:
1. Data ingestion from many sources
2. Data enrichment
3. Vector search
4. Fast indexed data store
5. ...

This hack builds a subset of the architecture in this repo - https://techcommunity.microsoft.com/t5/azure-ai-services-blog/revolutionize-your-enterprise-data-with-chatgpt-next-gen-apps-w/ba-p/3762087 - which is a very common and simple pattern for this scenario. 
The idea of the hack is to produce the search and generative parts of this solution by hand, in the portal or via CLR - i.e. not via a script. You learn how to create the resources, ingest and enrich data, query the data, and understand what the different capabilities actually bring in practice. After the hack you can use the scripts in the repo above to deploy the more fully featured and demonstrable example, in the smug knowledge that you now know how it all works.

![Imgur](https://github.com/ianlcurtis1/cog-search-and-chatgpt-hack/blob/main/Architecture.png)

# Hack Away!
`Prerequisites`
- OpenAI service enabled on your subscription.
- ..

The hack will not build a UI, hackers will query the data via AI Studio.

`TASK 1` Create the base infrastructure
1. Log into the portal, https://portal.azure.com
2. Create a Cognitive Search service: eastus, standard tier, ...
3. Create a storage account and blob storage container: LRS, ...
4. Upload data files to your blob container
5. Create an OpenAI service
6. Create a deployment of `GPT 3.5 Turbo`

`TASK 2` Run a prompt against ChatGPT grounded in raw data ingested into ACS 
1. ...
2. 

`TASK 3` Run the same prompt against ChatGPT grounded in data ingested and enriched into ACS
Indexes
GPT 3.5 Turbo
1. ...
2. 

`TASK 4` Run the same prompt against ChatGPT grounded in data ingested and enriched into ACS, using vector search
1. ...
2. 

# Stretch Goals
`TASK 5` - Filter search results based on AD roles
1. Filtered search https://github.com/jometzg/openai-chat-rest-examples/blob/main/filtered-search-with-embeddings.md
2. ...

# Cleanup
⚠️ To avoid unnecessary costs, remember to take down your app if it's no longer in use by deleting the resource group.

# Helpful links
...
