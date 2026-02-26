# LLM Android Clean Architecture

## Overview
A production-grade Android LLM integration should follow Clean Architecture principles to ensure scalability, testability, and maintainability.

## Architecture Layers

### 1. Presentation Layer
- Jetpack Compose UI
- ViewModel
- UI state management
- Streaming token rendering

### 2. Domain Layer
- Use cases (SendMessageUseCase)
- Business rules
- Conversation management
- Tool invocation orchestration

### 3. Data Layer
- Repository pattern
- Remote LLM datasource
- Local cache datasource
- DTO → Domain mapping

## Flow
UI → ViewModel → UseCase → Repository → RemoteDatasource → Backend Proxy → LLM

## Key Benefits
- Separation of concerns
- Replaceable LLM provider
- Testable domain logic
- Stable UI
