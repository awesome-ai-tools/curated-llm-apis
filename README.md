<p align="center">
  <img src="assets/banner.svg" alt="Curated LLM APIs" width="800"/>
</p>

<h1 align="center">Curated LLM APIs</h1>

<p align="center">
  <strong>A curated comparison of LLM API providers &mdash; pricing, models, features, and SDKs</strong>
</p>

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome"></a>
  <a href="https://github.com/awesome-ai-tools/curated-llm-apis/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
  <a href="https://github.com/awesome-ai-tools/curated-llm-apis/actions/workflows/link-checker.yml"><img src="https://github.com/awesome-ai-tools/curated-llm-apis/actions/workflows/link-checker.yml/badge.svg" alt="Link Check"></a>
  <a href="https://github.com/awesome-ai-tools/curated-llm-apis/stargazers"><img src="https://img.shields.io/github/stars/awesome-ai-tools/curated-llm-apis?style=flat" alt="Stars"></a>
  <a href="#pricing-comparison"><img src="https://img.shields.io/badge/pricing-updated_Mar_2026-brightgreen" alt="Pricing Updated"></a>
</p>

<p align="center">
  <a href="#major-providers">Major Providers</a> &bull;
  <a href="#open-source-model-hosting">Open Source Hosting</a> &bull;
  <a href="#specialized-apis">Specialized APIs</a> &bull;
  <a href="#pricing-comparison">Pricing Table</a> &bull;
  <a href="https://awesome-ai-tools.github.io/curated-llm-apis/">Searchable Directory</a>
</p>

---

## Featured: Ssemble AI Clipping

> **[Ssemble](https://www.ssemble.com)** &mdash; AI-powered video clipping via MCP (Model Context Protocol). Automatically extract the best short-form clips from long videos using AI. Available as an MCP server for integration with Claude, Cursor, and other AI tools.
>
> **[`@ssemble/mcp-server` on npm](https://www.npmjs.com/package/@ssemble/mcp-server)** | **[ssemble.com](https://www.ssemble.com)**

---

## Contents

- [Major Providers](#major-providers)
- [Open Source Model Hosting](#open-source-model-hosting)
- [Specialized APIs](#specialized-apis)
- [Embedding APIs](#embedding-apis)
- [API Gateways & Routers](#api-gateways--routers)
- [LLM SDKs & Libraries](#llm-sdks--libraries)
- [Evaluation & Testing](#evaluation--testing)
- [Rate Limiting & Cost Management](#rate-limiting--cost-management)
- [Pricing Comparison](#pricing-comparison)
- [Recently Added](#recently-added)
- [Related Lists](#related-lists)
- [Contributing](#contributing)

---

## Major Providers

Full-service LLM API providers with proprietary frontier models.

- [OpenAI](https://platform.openai.com/) - Creator of the GPT series. Flagship models include GPT-4o ($2.50/$10.00 per 1M tokens) and the newer GPT-4.1 family. 128K context window. Industry-leading function calling and structured outputs.
- [Anthropic](https://www.anthropic.com/api) - Maker of the Claude family. Current lineup: Claude Haiku 3.5 ($0.80/$4.00), Sonnet 4 ($3/$15), and Opus 4 ($15/$75). Up to 200K context window. Strong at coding, analysis, and safety.
- [Google Gemini](https://ai.google.dev/) - Google's multimodal AI. Gemini 2.5 Pro ($1.25/$10.00 under 200K context), Gemini 2.0 Flash ($0.10/$0.40). Native multimodal input (text, image, audio, video). Up to 1M token context.
- [Amazon Bedrock](https://aws.amazon.com/bedrock/) - Managed service providing access to foundation models from Anthropic, Meta, Mistral, Cohere, AI21, and Amazon's own Titan models via a unified API. Pay-per-use with no upfront commitment.
- [Azure OpenAI Service](https://azure.microsoft.com/en-us/products/ai-services/openai-service) - Microsoft's enterprise deployment of OpenAI models with Azure security, compliance, and regional availability. Same models as OpenAI with enterprise SLAs.
- [Cohere](https://cohere.com/) - Enterprise-focused NLP platform. Command R+ for RAG workloads, Command A ($2.50/$10.00 per 1M tokens) for agents. Strong multilingual support and embedding models.
- [AI21 Labs](https://www.ai21.com/) - Creator of the Jamba model family. Jamba 1.5 offers a 256K context window. Specializes in enterprise language understanding and generation.
- [Mistral AI](https://mistral.ai/) - European AI lab. Mistral Large ($2/$6 per 1M tokens), Mistral Medium 3 ($0.40/$2.00), and Mistral Small. Open-weight models available. Strong multilingual performance.
- [xAI (Grok)](https://docs.x.ai/) - Elon Musk's AI company. Grok-3 models with real-time X (Twitter) data access. Grok 3 Mini ($0.30/$0.50 per 1M tokens). Up to 131K context window.
- [DeepSeek](https://platform.deepseek.com/) - Chinese AI lab offering highly cost-effective models. DeepSeek V3 ($0.27/$1.10 per 1M tokens). Automatic context caching reduces costs by up to 90%. Open-weight.
- [Meta Llama (via API partners)](https://llama.meta.com/) - Meta's open-source Llama 3.1 models (8B, 70B, 405B parameters) available through various hosting providers. Free weights with commercial license.
- [Reka AI](https://www.reka.ai/) - Multimodal models with vision, audio, and text understanding. Reka Core, Flash, and Edge models for various deployment sizes.

## Open Source Model Hosting

Platforms that host and serve open-source and open-weight models via API.

- [Together AI](https://www.together.ai/) - Host for 100+ open-source models including Llama 3.1, Mixtral, and Qwen. Inference, fine-tuning, and custom model deployment. Llama 3.1 70B from $0.88/1M tokens.
- [Fireworks AI](https://fireworks.ai/) - High-performance inference for open models. Llama 3.1 70B at $0.90/1M tokens. On-demand and serverless deployment options. Custom model support.
- [Groq](https://groq.com/) - Ultra-fast inference on custom LPU hardware. Llama 3.1 70B at $0.59/$0.79 per 1M tokens. Sub-second latency. Focused on speed with throughput up to 500+ tokens/sec.
- [Anyscale](https://www.anyscale.com/) - Scalable LLM serving built on Ray. Supports fine-tuning and hosting of open models. Enterprise-grade deployment with auto-scaling.
- [Replicate](https://replicate.com/) - Run open-source models in the cloud with a simple API. Pay per second of compute. Supports Llama, Stable Diffusion, Whisper, and thousands more.
- [Modal](https://modal.com/) - Serverless cloud for AI/ML. Run any model with GPU access. Pay-per-second billing. Great for batch jobs and custom inference pipelines.
- [Perplexity API](https://docs.perplexity.ai/) - LLM API with built-in web search grounding. Sonar models combine language understanding with real-time internet data retrieval.
- [DeepInfra](https://deepinfra.com/) - Cost-effective inference for open models. Llama 3.1 8B at $0.03/$0.05 per 1M tokens. Serverless GPUs with global edge deployment.
- [Cerebras](https://cerebras.ai/) - Wafer-scale inference engine. Extremely fast inference for Llama 3.1 models at $0.10/1M tokens for 8B model. Record-setting throughput.
- [Lepton AI](https://www.lepton.ai/) - Developer-friendly platform for running open-source AI models. Simple API with auto-scaling and built-in monitoring.
- [Hyperbolic](https://hyperbolic.xyz/) - Decentralized AI inference platform. Competitive pricing for open-source model hosting with global GPU network.
- [OpenRouter](https://openrouter.ai/) - Unified API gateway routing to 100+ models from multiple providers. Automatic fallback and load balancing. Single API key for all providers.
- [Novita AI](https://novita.ai/) - Affordable GPU cloud for open-source model inference. Image generation, LLM hosting, and fine-tuning services.
- [OctoAI](https://octo.ai/) - Efficient AI inference platform with optimized serving for popular open models. Self-serve fine-tuning and customization.

## Specialized APIs

AI APIs focused on specific modalities beyond text generation.

### Voice & Audio
- [ElevenLabs](https://elevenlabs.io/) - Industry-leading AI voice synthesis and cloning. Text-to-speech, voice cloning, and dubbing. Used by major media companies.
- [OpenAI Whisper API](https://platform.openai.com/docs/guides/speech-to-text) - State-of-the-art speech-to-text. Supports 50+ languages. $0.006 per minute of audio.
- [AssemblyAI](https://www.assemblyai.com/) - Speech-to-text with speaker diarization, sentiment analysis, and summarization. Real-time and batch transcription APIs.
- [Deepgram](https://deepgram.com/) - Fast, accurate speech recognition API. Real-time streaming and batch processing. Custom model training available.
- [Suno](https://suno.com/) - AI music generation. Create full songs with vocals, instruments, and lyrics from text prompts.

### Image & Video
- [Stability AI](https://platform.stability.ai/) - Creators of Stable Diffusion. Image generation, upscaling, editing, and video generation APIs. Open-source models available.
- [Midjourney](https://www.midjourney.com/) - Premium AI image generation known for artistic quality. Available through Discord and web interface.
- [RunwayML](https://runwayml.com/) - AI-powered video generation and editing. Gen-3 Alpha for text-to-video. Used in professional film and media production.
- [Luma AI](https://lumalabs.ai/) - Dream Machine for text-to-video and image-to-video generation. Realistic 3D-aware video synthesis.
- [Ideogram](https://ideogram.ai/) - AI image generation with strong text rendering capabilities. Free tier available.
- [Kling AI](https://klingai.com/) - Video generation API by Kuaishou. High-quality text-to-video and image-to-video with motion control.
- [Pika](https://pika.art/) - AI video generation and editing platform. Text-to-video, image-to-video, and video-to-video capabilities.

### Code
- [GitHub Copilot API](https://github.com/features/copilot) - AI pair programmer powered by OpenAI Codex. Code completion, chat, and CLI integration for 10+ languages.
- [Codestral (Mistral)](https://mistral.ai/) - Mistral's dedicated code generation model. $0.30/$0.90 per 1M tokens. 32K context window optimized for code.
- [Sourcegraph Cody](https://sourcegraph.com/cody) - AI coding assistant with full codebase context. Uses multiple LLM backends for code understanding and generation.

## Embedding APIs

APIs for generating vector embeddings from text, used in search, RAG, and similarity applications.

- [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) - text-embedding-3-large (3072 dimensions) and text-embedding-3-small (1536 dimensions). $0.13/$0.02 per 1M tokens respectively. Industry standard.
- [Cohere Embed](https://cohere.com/embed) - Embed v3 with support for 100+ languages. Optimized for search, classification, and clustering. Input types for search documents vs queries.
- [Voyage AI](https://www.voyageai.com/) - High-performance embeddings optimized for retrieval. voyage-3 and voyage-code-3 models. Leading MTEB benchmark scores.
- [Jina AI](https://jina.ai/) - jina-embeddings-v3 with 8192 token context. Multilingual support for 89 languages. $0.02 per 1M tokens. Open-source options available.
- [Google Vertex AI Embeddings](https://cloud.google.com/vertex-ai/docs/generative-ai/embeddings/get-text-embeddings) - text-embedding-005 with 768 dimensions and task-type optimization. Tight integration with Google Cloud.
- [Mixedbread AI](https://www.mixedbread.ai/) - High-quality embeddings with binary quantization support. mxbai-embed-large-v1 competitive with OpenAI at lower cost.
- [Nomic AI](https://www.nomic.ai/) - Open-source nomic-embed-text with 8192 context. Fully auditable with published training data. Free for research use.

## API   Gateways & Routers

Tools for managing, routing, and optimizing LLM API calls across multiple providers.
- **[APIClaw](https://apiclaw.biz/)**  Flat-rate OpenAI-compatible AI API gateway ($19$129/mo) with free 50-request trial; one endpoint for Claude, OpenAI, Kimi, Qwen, DeepSeek, GLM.
- [LiteLLM](https://github.com/BerriAI/litellm) - Open-source proxy supporting 100+ LLMs with a unified OpenAI-compatible API. Load balancing, fallbacks, spend tracking, and rate limiting.
- [Portkey](https://portkey.ai/) - AI gateway with semantic caching, automatic retries, load balancing, and observability. Supports 200+ models. SOC2 compliant
- [Helicone](https://www.helicone.ai/) - Open-source LLM observability platform. Request logging, caching, rate limiting, and cost tracking with one-line integration.
- [Martian](https://withmartian.com/) - Intelligent model router that automatically selects the best LLM for each request based on cost, quality, and latency requirements.
- [OpenRouter](https://openrouter.ai/) - Unified API for 100+ models. Single API key, automatic failover, and competitive pricing across providers.
- [Unify AI](https://unify.ai/) - LLM routing platform that benchmarks and routes requests to the optimal provider based on quality, cost, and speed.
- [Not Diamond](https://www.notdiamond.ai/) - AI model router that learns which model performs best for your specific use cases. Automatic quality-based routing.
- [Keywords AI](https://keywordsai.co/) - LLM monitoring and gateway with analytics, prompt management, and A/B testing. Unified API for all major providers.

## LLM SDKs & Libraries

Developer tools, frameworks, and SDKs for building LLM-powered applications.

- [LangChain](https://www.langchain.com/) - Popular framework for building LLM applications. Chains, agents, RAG, and memory. Python and JavaScript. Integrates with 70+ LLM providers.
- [LlamaIndex](https://www.llamaindex.ai/) - Data framework for LLM apps. Specializes in connecting LLMs with external data for RAG. Advanced indexing and retrieval strategies.
- [Vercel AI SDK](https://sdk.vercel.ai/) - TypeScript toolkit for building AI-powered web apps. Streaming UI components, unified provider API, and React hooks.
- [Anthropic SDK](https://github.com/anthropics/anthropic-sdk-python) - Official Python and TypeScript SDKs for the Claude API. Streaming, tool use, vision, and prompt caching support.
- [OpenAI SDK](https://github.com/openai/openai-python) - Official Python and Node.js libraries for the OpenAI API. Streaming, function calling, assistants, and batch processing.
- [Instructor](https://github.com/jxnl/instructor) - Structured output extraction from LLMs using Pydantic models. Works with OpenAI, Anthropic, Google, and other providers.
- [Haystack](https://haystack.deepset.ai/) - End-to-end NLP framework by deepset. Modular pipelines for RAG, question answering, and document search.
- [Semantic Kernel](https://github.com/microsoft/semantic-kernel) - Microsoft's SDK for integrating LLMs into applications. C#, Python, and Java support. AI plugins and planners.
- [DSPy](https://dspy-docs.vercel.app/) - Framework for programming (not prompting) language models. Automatic prompt optimization and pipeline compilation.
- [Pydantic AI](https://ai.pydantic.dev/) - Agent framework from the Pydantic team. Type-safe, model-agnostic agent building with structured outputs.
- [CrewAI](https://www.crewai.com/) - Framework for orchestrating role-playing autonomous AI agents. Multi-agent collaboration for complex tasks.
- [AutoGen](https://microsoft.github.io/autogen/) - Microsoft framework for building multi-agent conversational AI systems. Agent-to-agent communication patterns.

## Evaluation & Testing

Tools for evaluating LLM outputs, testing prompts, and monitoring quality.

- [Braintrust](https://www.braintrust.dev/) - End-to-end platform for LLM evaluation, logging, and prompt playground. Side-by-side comparison, scoring, and regression testing.
- [Promptfoo](https://www.promptfoo.dev/) - Open-source CLI and library for testing and evaluating LLM outputs. Red-teaming, model comparison, and CI/CD integration.
- [Humanloop](https://humanloop.com/) - Prompt management and evaluation platform. Version control for prompts, A/B testing, and human feedback collection.
- [LangSmith](https://smith.langchain.com/) - By LangChain. Debugging, testing, evaluating, and monitoring LLM applications. Trace visualization and dataset management.
- [Weights & Biases (W&B)](https://wandb.ai/) - ML experiment tracking with LLM-specific features. Prompt versioning, trace logging, and evaluation dashboards.
- [Arize AI](https://arize.com/) - ML observability platform with LLM monitoring. Embedding drift detection, prompt analysis, and evaluation metrics.
- [Confident AI (DeepEval)](https://www.confident-ai.com/) - Open-source LLM evaluation framework. 14+ metrics including hallucination, relevancy, and toxicity detection.

## Rate Limiting & Cost Management

Tools for tracking, optimizing, and managing LLM API costs.

- [Helicone](https://www.helicone.ai/) - Open-source observability with built-in cost tracking, rate limiting, and caching. Supports all major LLM providers.
- [LLMeter](https://github.com/awslabs/llmeter) - AWS open-source tool for benchmarking LLM inference performance. Measure latency, throughput, and cost efficiency.
- [Portkey](https://portkey.ai/) - Cost tracking, budget alerts, and rate limiting across multiple LLM providers. Semantic caching to reduce API calls.
- [OpenMeter](https://openmeter.io/) - Usage metering and billing for AI applications. Track token consumption, set budgets, and generate invoices.
- [LangFuse](https://langfuse.com/) - Open-source LLM engineering platform. Cost tracking, prompt management, and quality evaluation with detailed analytics.
- [Lago](https://www.getlago.com/) - Open-source usage-based billing. Track AI API consumption and build metering into your product pricing.

---

## Pricing Comparison

Comparison of major LLM API providers. Prices are per **1 million tokens** (USD). Last updated: **March 2026**.

| Provider | Model | Input (per 1M) | Output (per 1M) | Context Window |
|----------|-------|---------------:|----------------:|---------------:|
| **OpenAI** | GPT-4o | $2.50 | $10.00 | 128K |
| **OpenAI** | GPT-4o mini | $0.15 | $0.60 | 128K |
| **OpenAI** | GPT-4.1 | $2.00 | $8.00 | 1M |
| **OpenAI** | GPT-4.1 mini | $0.40 | $1.60 | 1M |
| **Anthropic** | Claude Opus 4 | $15.00 | $75.00 | 200K |
| **Anthropic** | Claude Sonnet 4 | $3.00 | $15.00 | 200K |
| **Anthropic** | Claude Haiku 3.5 | $0.80 | $4.00 | 200K |
| **Google** | Gemini 2.5 Pro | $1.25 | $10.00 | 1M |
| **Google** | Gemini 2.0 Flash | $0.10 | $0.40 | 1M |
| **Google** | Gemini 2.0 Flash Lite | $0.075 | $0.30 | 1M |
| **Mistral** | Mistral Large | $2.00 | $6.00 | 128K |
| **Mistral** | Mistral Medium 3 | $0.40 | $2.00 | 128K |
| **Mistral** | Mistral Small | $0.10 | $0.30 | 128K |
| **xAI** | Grok-3 | $3.00 | $15.00 | 131K |
| **xAI** | Grok-3 Mini | $0.30 | $0.50 | 131K |
| **DeepSeek** | DeepSeek V3 | $0.27 | $1.10 | 128K |
| **DeepSeek** | DeepSeek V3 (cached) | $0.07 | $1.10 | 128K |
| **Cohere** | Command A | $2.50 | $10.00 | 256K |
| **Cohere** | Command R+ | $2.50 | $10.00 | 128K |
| **Cohere** | Command R | $0.15 | $0.60 | 128K |
| **Meta (via providers)** | Llama 3.1 405B | ~$1.00 | ~$1.00 | 128K |
| **Meta (via providers)** | Llama 3.1 70B | ~$0.50 | ~$0.70 | 128K |
| **Meta (via providers)** | Llama 3.1 8B | ~$0.05 | ~$0.08 | 128K |
| **Groq** | Llama 3.1 70B | $0.59 | $0.79 | 128K |
| **Together AI** | Llama 3.1 70B | $0.88 | $0.88 | 128K |
| **DeepInfra** | Llama 3.1 8B | $0.03 | $0.05 | 128K |
| **Cerebras** | Llama 3.1 8B | $0.10 | $0.10 | 128K |

> **Note**: Prices are approximate and subject to change. Many providers offer volume discounts, prompt caching (up to 90% savings), and batch processing (up to 50% off). Always check the provider's official pricing page for the most current rates.
>
> **Sources**: [OpenAI Pricing](https://openai.com/api/pricing/) | [Anthropic Pricing](https://www.anthropic.com/pricing) | [Google AI Pricing](https://ai.google.dev/gemini-api/docs/pricing) | [Mistral Pricing](https://mistral.ai/pricing) | [xAI Pricing](https://docs.x.ai/developers/models) | [DeepSeek Pricing](https://api-docs.deepseek.com/quick_start/pricing) | [Cohere Pricing](https://cohere.com/pricing) | [Groq Pricing](https://groq.com/pricing)

---

## Recently Added

*Last updated: March 2026*

- **DeepSeek V3** - Added pricing for cache hit/miss tiers
- **Cerebras** - Wafer-scale inference with record throughput
- **Pydantic AI** - Type-safe agent framework
- **Confident AI (DeepEval)** - Open-source evaluation framework
- **Keywords AI** - LLM monitoring gateway
- **Mixedbread AI** - High-quality embeddings with binary quantization
- **Not Diamond** - Quality-based model routing

## Related Lists

- [awesome-llm](https://github.com/Hannibal046/Awesome-LLM) - A curated list of large language models
- [awesome-generative-ai](https://github.com/steven2358/awesome-generative-ai) - A curated list of generative AI tools
- [awesome-chatgpt-api](https://github.com/reorx/awesome-chatgpt-api) - Curated list of apps and tools using ChatGPT API
- [open-llms](https://github.com/eugeneyan/open-llms) - List of open LLMs available for commercial use
- [awesome-ai-agents](https://github.com/e2b-dev/awesome-ai-agents) - A list of AI autonomous agents

## Contributing

Contributions are welcome! Please read the [Contributing Guidelines](CONTRIBUTING.md) before submitting a pull request.

To add a new provider or tool:

1. Fork this repository
2. Add your entry in the appropriate section (alphabetical order)
3. Include accurate pricing data with sources
4. Submit a pull request

---

<p align="center">
  <sub>Maintained by <a href="https://github.com/awesome-ai-tools">awesome-ai-tools</a>. Star this repo if you find it useful!</sub>
</p>
