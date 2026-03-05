# RubyLLM Skill

A Claude Code skill for working with [RubyLLM](https://rubyllm.com/) - a Ruby gem providing a unified API for interacting with multiple AI providers.

## What This Skill Provides

Reference documentation and guidance for building AI-powered Ruby applications with RubyLLM:

- **Chat** - Conversational AI interactions
- **Tools** - Function calling to let AI call your Ruby code
- **Streaming** - Real-time response streaming
- **Embeddings** - Text vectorization
- **Image Generation** - AI image creation
- **Audio Transcription** - Speech to text
- **Moderation** - Content safety checking
- **Rails Integration** - ActiveRecord persistence
- **Async** - Concurrent operations

## Supported Providers

OpenAI, Anthropic, Google Gemini, AWS Bedrock, DeepSeek, Mistral, Ollama, OpenRouter, Perplexity, xAI, Azure AI, GPUStack

## Installation

This skill can be loaded into Claude Code when working with RubyLLM projects.

## Quick Start

```ruby
# Configure
RubyLLM.configure do |config|
  config.openai_api_key = ENV['OPENAI_API_KEY']
end

# Chat
chat = RubyLLM.chat
response = chat.ask "What is Ruby?"

# Images
image = RubyLLM.paint("A sunset")

# Embeddings
embedding = RubyLLM.embed("Ruby is elegant")
```

## Usage

When working on a Ruby project that needs AI functionality, this skill provides:

- Quick reference for common patterns
- Detailed documentation in `references/`
- Code examples for all features

## See Also

- [RubyLLM Documentation](https://docs.rubyllm.com/)
- [RubyLLM GitHub](https://github.com/crmne/ruby_llm)
