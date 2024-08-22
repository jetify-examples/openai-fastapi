# openai-fastapi

This repo is an example that sets up a devbox environment with Python and pip. It uses Fast API to set up API endpoints listed below and calls OpenAI API to allow interactions with ChatGPT.

## Setup

### Prerequisites

To setup this repo make sure to have [devbox](https://www.jetify.com/devbox/docs/installing_devbox/) installed and have access to your OpenAI's [API key](https://help.openai.com/en/articles/4936850-where-do-i-find-my-openai-api-key).

### Steps

1. Clone this repo `git clone https://github.com/jetify-examples/openai-fastapi.git`.
2. `cd openai-fastapi` and then run `devbox run install`
3. Copy your OpenAI's API key in devbox.json's `"env"` section.
4. run `devbox run start`
