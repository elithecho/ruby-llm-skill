---
name: ruby-llm
description: "Ruby gem providing a unified API for interacting with multiple AI providers (OpenAI, Anthropic, Google Gemini, Ollama, and more). Use when working with Ruby applications that need chat conversations, embeddings, image generation, audio transcription, content moderation, tool/function calling, Rails integration, or async operations."
---

# RubyLLM

## Quick Start

```ruby
# Simple chat
chat = RubyLLM.chat
response = chat.ask "What is Ruby?"
puts response.content

# With a specific model
chat = RubyLLM.chat(model: 'claude-sonnet-4-5')
response = chat.ask "Explain Ruby metaprogramming"

# Generate images
image = RubyLLM.paint("A sunset over mountains")

# Create embeddings
embedding = RubyLLM.embed("Ruby is elegant and expressive")
```

## Installation

```ruby
bundle add ruby_llm
```

## Configuration

```ruby
RubyLLM.configure do |config|
  config.openai_api_key = ENV['OPENAI_API_KEY']
  config.anthropic_api_key = ENV['ANTHROPIC_API_KEY']
end
```

## Core Features

- **Chat**: Conversational AI interactions with message history
- **Tools**: Let AI models call your Ruby code
- **Streaming**: Real-time response streaming
- **Embeddings**: Text vectorization for similarity search
- **Image Generation**: AI image creation (DALL-E, etc.)
- **Audio Transcription**: Speech to text
- **Moderation**: Content safety checking
- **Extended Thinking**: Reasoning models

## Supported Providers

OpenAI, Anthropic, Google Gemini, AWS Bedrock, DeepSeek, Mistral, Ollama (local), OpenRouter, Perplexity, xAI (Grok), Azure AI, GPUStack

## Reference Documentation

For detailed information on each feature, see the reference files:

- **Getting Started**: [getting-started.md](getting-started.md) - Quick start guide
- **Configuration**: [configuration.md](configuration.md) - API keys, defaults, and settings
- **Chat**: [chat.md](chat.md) - Conversational AI interactions
- **Tools**: [tools.md](tools.md) - Function calling and tool definitions
- **Streaming**: [streaming.md](streaming.md) - Real-time response streaming
- **Embeddings**: [embeddings.md](embeddings.md) - Text vectorization
- **Image Generation**: [image-generation.md](image-generation.md) - AI image creation
- **Audio Transcription**: [audio-transcription.md](audio-transcription.md) - Speech to text
- **Moderation**: [moderation.md](moderation.md) - Content safety checking
- **Extended Thinking**: [thinking.md](thinking.md) - Reasoning models
- **Rails Integration**: [rails.md](rails.md) - ActiveRecord persistence
- **Async**: [async.md](async.md) - Concurrent operations
- **Error Handling**: [error-handling.md](error-handling.md) - Graceful error management
- **Model Registry**: [models.md](models.md) - Model discovery and capabilities
- **Agentic Workflows**: [agentic-workflows.md](agentic-workflows.md) - Orchestrating multiple agents
