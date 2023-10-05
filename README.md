# LLM Data Backend - Powered By Meltano

This Meltano project is an example of the project described in this [blog post](https://meltano.com/blog/llm-apps-are-mostly-data-pipelines/).

## Prereqs
- An OpenAI account and API key
- A Pinecone account and API key
- You can optionally create an index in Pinecone but this project is currently configured to delete and recreate the index

## Run
To run the project do the following:

1. Copy the `.env_template` file to `.env` and replace the sample values with your OpenAI and Pinecone values
2. Run `meltano install`
3. Run `meltano run reload_pinecone`
4. Run the demo app `meltano invoke streamlit_app:demo_ui`
