# AI Test Case Generator using n8n + Groq

An n8n workflow that turns a feature requirement into structured test cases using an AI Agent.

![Workflow](Testcases_using_AI_Agent.png)

## How it works
Chat Trigger → AI Agent (Groq Chat Model) → Convert to File (HTML)

1. Paste a requirement or user story into the chat.
2. The AI Agent generates test cases (ID, Title, Preconditions, Steps, Expected Result).
3. The output is saved as an HTML file.

## Sample output
See [File.html](File.html) for generated test cases for an account balance feature.

## Setup
1. Install n8n and open the editor.
2. Import `testcase-agent.json` (Workflows → Import from File).
3. Add your own Groq API credentials to the Groq Chat Model node.
4. Open the chat and send a requirement.

## Tech stack
n8n, Groq LLM, AI Agent, HTML export