<img src="logo.png" alt="Intelegence Logo" width="200" />

# Intelegence

A simple TypeScript framework for building AI-powered applications with support for language models, image generation, and persistent storage.

## Features

-   🤖 **Language Models**: Integrate with various language models (like OpenAI) with built-in caching
-   🎨 **Image Generation**: Generate images using AI models with automatic storage and caching
-   💾 **Storage System**: Flexible storage interface with implementations for various backends
-   🔄 **Caching**: Automatic caching of model responses for improved performance
-   🎯 **Type Safety**: Full TypeScript support with well-defined interfaces
-   🔌 **Extensible**: Easy to implement custom models and storage backends

## Installation

```bash
npm install @aerrobert/intelligence
```

## Quick Start

```typescript
const AI = new Intelegence({
    language: new OpenAIChatBasedLLM({
        storage: new LocalDataStorage({
            storagePath: './storage',
        }),
    }),
});

const result = await AI.ask({
    question: 'What is the capital of France?',
});
```
