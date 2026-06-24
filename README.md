# ai-openai

OpenAI driver for the togo `ai` plugin — a unified LLM interface (chat + embeddings) for togo apps.

## Install
```bash
togo install togo-framework/ai-openai
```

## Configure
Set `AI_DRIVER=openai` and:
```env
OPENAI_API_KEY=...
# optional: OPENAI_BASE_URL=https://api.openai.com/v1
```

Then the `ai` plugin routes `Chat`/`Embed` through OpenAI. Token usage is reported via `ai.Usage` (for the billing plugin).

MIT © ToGO
