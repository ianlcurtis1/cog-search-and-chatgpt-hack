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

`TASK 1` Create a vanilla GPT deployment
1. In Azure, create an OpenAI service.
2. From AI Studio create a deployment of `GPT 3.5 Turbo`.

Note the `Chat` and `Completions` blades in AI Studio. 
- You can ask ChatGPT a question or 2.
- Have a play with the settings in the right-hand blade of the Chat and Completions pages and note the effect on the response received. Tip: it's best to change one setting at a time.
- You can deploy the model as a Web App or PVA by using the dropdown in the top-right corner, if you like.

Now we need to add our own data.

`TASK 2` Create search service deployment
1. Create a Cognitive Search service: eastus, standard tier, ...
2. Create a storage account and blob storage container: LRS, ...
3. Upload data files found [???] to your blob container

`TASK 3` Run a prompt against ChatGPT grounded in raw data ingested into ACS

You can quickly ground ChatGPT with your data by using the 'Add your data' tab in the Chat Playground. 
1. Add your uploaded data as a data source for your GPT model.
2. Write a prompt to find out x and display it as y...

`TASK 4` Run the same prompt against ChatGPT grounded in data ingested and enriched into ACS
Indexes
GPT 3.5 Turbo
1. ...
2. 

`TASK 5` Run the same prompt against ChatGPT grounded in data ingested and enriched into ACS, using vector search
1. ...
2. 

`TASK 6` Prompt engineering to get a better response
1. ...
2. 

`TASK 7` Protect your model's endpoint
1. ...
2. 

# Stretch Goals
`TASK 8` - Filter search results based on AD roles
1. Filtered search https://github.com/jometzg/openai-chat-rest-examples/blob/main/filtered-search-with-embeddings.md
2. ...

`TASK 9` - Investigate Prompt Flow
1. ...
2. 

# Cleanup
⚠️ To avoid unnecessary costs, remember to take down your app if it's no longer in use by deleting the resource group.

# Helpful links
...
