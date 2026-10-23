# AI Email Customer Support with RAG

An AI-powered customer support automation that receives customer
emails through Gmail, understands the request using an AI agent,
retrieves relevant information from a knowledge base using RAG,
and automatically sends a contextual response.

## Architecture

Gmail
   ↓
Gmail Trigger
   ↓
AI Agent
   ↓
RAG Knowledge Base
   ↓
LLM
   ↓
Generate Response
   ↓
Gmail Reply

## Tech Stack

- n8n
- Gmail
- RAG (Retrieval-Augmented Generation)
- Groq LLM
- Google Gemini Embeddings
- Vector Database
- AI Agent

## Features

- Automatically reads incoming customer emails
- Understands customer questions
- Retrieves relevant information from the knowledge base
- Generates context-aware responses
- Automatically replies to the customer
- Reduces manual customer-support work

## Workflow

1. Customer sends an email.
2. Gmail Trigger receives the message.
3. The AI Agent analyzes the customer's request.
4. The RAG system searches the knowledge base.
5. Relevant information is provided to the AI Agent.
6. The LLM generates a response.
7. n8n sends the response back through Gmail.

## Example

Customer:

"Hi, I want to book an appointment with a doctor."

The AI agent understands the request and uses the available
knowledge/context to provide the appropriate response.

## Setup

1. Import `workflow/customer-support-rag.json` into n8n.
2. Configure your Gmail credentials.
3. Configure your LLM credentials.
4. Configure the embedding model.
5. Configure the vector database/knowledge base.
6. Update the system prompt.
7. Activate the workflow.

## Security

API keys, credentials, customer emails, and private documents
are not included in this repository.

## Future Improvements

- Human handoff for complex queries
- Ticket creation
- Conversation memory
- Multi-language support
- Customer sentiment detection
- Support analytics
