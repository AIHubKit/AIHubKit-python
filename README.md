# AIHubKit

**AIHubKit** is an open-source Python library designed to streamline the integration of various large language models (LLMs) into applications. Its primary goal is to provide a unified client SDK that simplifies interactions with different LLM providers, such as OpenAI, Anthropic, and HuggingFace.

## Key Features

- **Unified API Interface**  
  Interact with multiple LLMs through a consistent and simple API, reducing the complexity of learning provider-specific SDKs.

- **Modular Design**  
  Each LLM integration is encapsulated in its own module, enabling seamless addition of new models or providers.

- **Configuration Management**  
  Centralized management of API keys and model-specific settings through a flexible configuration system.

- **Error Handling and Logging**  
  Built-in utilities for error handling and logging help streamline development and debugging.

- **Extensibility**  
  Easily extendable to support new models or customize functionality based on specific project requirements.

## Use Cases

- **Conversational AI**: Build chatbots or virtual assistants powered by multiple LLMs.  
- **Document Analysis**: Use LLMs for tasks like summarization, sentiment analysis, or question-answering on text documents.  
- **Multi-Model AI Systems**: Leverage the strengths of different models for specialized tasks, such as translation, content generation, or information retrieval.

## Goals

AIHubKit aims to lower the barrier for developers and researchers to leverage LLMs by providing a simplified, consistent, and extensible integration framework.

## Example Usage

Here’s a simple example to demonstrate how AIHubKit might be used:

```python
from aihubkit import OpenAIClient, AnthropicClient

# Initialize OpenAI client
openai_client = OpenAIClient(api_key="your-openai-key")
response = openai_client.generate_text(prompt="Explain quantum computing")
print(response)

# Switch to Anthropic client
anthropic_client = AnthropicClient(api_key="your-anthropic-key")
response = anthropic_client.generate_text(prompt="Explain quantum computing")
print(response)
