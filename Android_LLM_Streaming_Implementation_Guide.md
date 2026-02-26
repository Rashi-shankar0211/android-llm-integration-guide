# Android LLM Streaming Implementation Guide

## Why Streaming?
- Better UX
- Faster perceived response
- ChatGPT-like experience

## Transport Options
- SSE (recommended)
- WebSocket
- Chunked HTTP

## Android Implementation

### Network
- OkHttp streaming
- Ktor streaming

### Coroutine Flow
Stream tokens via Flow

### UI
- Append tokens progressively
- Typing indicator
- Cancel support

## Backend Requirement
Proxy must forward streaming tokens from provider.

## UX Tips
- Smooth scrolling
- Partial markdown rendering
- Retry on disconnect
