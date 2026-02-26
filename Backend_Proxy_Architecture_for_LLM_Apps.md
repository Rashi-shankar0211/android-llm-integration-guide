
# Backend Proxy Architecture for LLM Apps

## Why Proxy?
- Protect API keys
- Add authentication
- Prompt control
- Rate limiting
- Logging
- Cost monitoring

## Architecture
Android → Auth Layer → LLM Service → Provider

## Responsibilities

### Auth Layer
- JWT validation
- User identity
- Session control

### LLM Service
- Prompt enrichment
- System prompt injection
- Tool schema
- Token limit control

### Observability
- Prompt logs
- Response logs
- Latency metrics
- Cost metrics

## Recommended Stack
- Node.js / FastAPI
- Redis cache
- Vector DB (optional)
