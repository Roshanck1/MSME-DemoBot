User (Web Browser)
      ↓
Frontend UI (HTML/React)  ←→  FastAPI Backend (OpenAI API)

Backend: FastAPI server that connects to OpenAI and handles logic
A frontend chat interface (HTML/JavaScript or React)

uvicorn
What it is: A lightning-fast ASGI server used to serve FastAPI apps.
Why it’s used: Runs your app so it can accept web traffic (like user messages or browser requests).

openai
What it is: The official Python SDK to communicate with OpenAI’s API (e.g., GPT-3.5, GPT-4).
Why it’s used: Send prompts, receive completions, build chatbot logic.

python-dotenv
What it is: A helper library to load environment variables from a .env file into os.environ.
Why it’s used: Keeps your API keys and secrets out of your main code.

jinja2
What it is: A templating engine used by FastAPI (and Flask) to render HTML pages.
Why it’s used: Allows you to generate chatbot UIs, result pages, etc., dynamically.

| Package         | Role              | Why It’s Needed                            |
| --------------- | ----------------- | ------------------------------------------ |
| `fastapi`       | Web API framework | Handles routes and logic for chat requests |
| `uvicorn`       | ASGI server       | Runs the FastAPI app                       |
| `openai`        | OpenAI API SDK    | Talks to ChatGPT/GPT-4/other models        |
| `python-dotenv` | Config management | Loads your secrets (.env) into the app     |
| `jinja2`        | Template engine   | Renders HTML pages dynamically             |
