# ai-openai — documentation

OpenAI LLM driver for togo ai

## Overview

Package openai is a OpenAI driver for togo ai (OpenAI-compatible API).
Blank-import it and set AI_DRIVER=openai + OPENAI_API_KEY.

## Install

```bash
togo install togo-framework/ai-openai
```

Set `AI_DRIVER=openai`.

## Configuration

Environment variables read by this plugin (extracted from the source — see the gateway/provider docs for each value):

| Env var |
|---|
| `OPENAI_BASE_URL"` |

## Usage

```go
provider := ai.FromKernel(k)
resp, err := provider.Chat(ctx, []ai.Message{{Role: "user", Content: "Hello"}}, ai.Options{})
// streaming + provider.Embed(ctx, texts) for vectors; resp.Usage carries token counts
```

## Links

- Marketplace: https://to-go.dev/marketplace
- Source: https://github.com/togo-framework/ai-openai
- Full README: ../README.md
