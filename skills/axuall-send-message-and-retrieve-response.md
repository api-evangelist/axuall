---
name: axuall-send-message-and-retrieve-response
description: Send a message to an agent and retrieve the conversation messages.
api: openapi/axuall-openapi.json
operations:
- agent_chat_v2_agent_chat_post
- get_agent_conversation_messages_v2_agent_conversations__conversation_id__messages_get
generated: '2026-09-27'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/axuall-openapi.json ; every operationId checked against the contract
---

# axuall-send-message-and-retrieve-response

Send a message to an agent and retrieve the conversation messages.

## Steps

1. 1. Call `agent_chat_v2_agent_chat_post` with the request body fields `agent_id`, `message`, and optional `metadata`.
2. 2. Call `get_agent_conversation_messages_v2_agent_conversations__conversation_id__messages_get` with the path parameter `conversation_id` returned from the chat response to fetch the messages.

## Rules

- Auth: Include an `Authorization: Bearer <token>` header as defined by the HTTPBearer scheme.
