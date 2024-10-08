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

## Usage

Once the server is setup and running, you can access to static page by visiting `localhost:8080`

### API

The app also makes an API endpoint available to interact with OpenAI's ChatGPT. The endpoint responds to POST requests to `/api/prompt`. Below is an example request and response:

Example request:

```bash
curl --location 'http://127.0.0.1:8080/api/prompt' \
--header 'Content-Type: application/json' \
--data '{
    "prompt": "What is the circumference of Earth?"
}'
```

Example response:

```json
{
  "message": {
    "content": "The circumference of Earth is approximately 24,901 miles (40,075 kilometers).",
    "refusal": null,
    "role": "assistant",
    "function_call": null,
    "tool_calls": null
  }
}
```

## Development

To use this project as a skeleton and develop on it, you can utilize the references for Fast API [docs](https://fastapi.tiangolo.com/#create-it), more specifically, routes and handlers. As well as OpenAI's [Python SDK](https://pypi.org/project/openai/).
