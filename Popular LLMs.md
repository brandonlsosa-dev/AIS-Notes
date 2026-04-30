---
title: Popular LLMs ​ 📊 - Build Your Portfolio · AI Automation Society Plus
description: >-
  Transcript Module Summary This module introduces you to popular large language
  models (LLMs) and helps you understand how to choose the right one for your
  use c
author: Build Your Portfolio · AI Automation Society Plus
source: >-
  https://www.skool.com/ai-automation-society-plus/classroom/d99017d2?md=f8ce9de33ce345f08e19f8a909678424
created: "2026-04-30"
tags:
  - hover-notes
  - skool
---

## Intro to Popular LLMs

### Model Selection in a Fast-Changing Space

- **Key Goal**: Understand differences between model families (proprietary, open-source, reasoning systems)
- Choose specific models for specific use cases
    - Essential when starting out or working with clients
    - AI space changes very quickly

### Understanding Tokens

- LLMs process text as **tokens**—fundamental units that can be words, word parts, or punctuation
    - Example: "I love AI!" -> ["I", "love", "AI", "!"]

#### Why Tokens Matter

- Pricing based on token usage
- Context limits measured in tokens
- Critical for cost estimation

### OpenRouter for LLM Access

- **Quick aside**: OpenRouter provides a unified interface to connect agents/automations to pretty much all LLMs
    - Preferred tool for NNN AI agents and automations (more details in future material)
- **Models page** shows a ton of options, including lesser-known ones
- Key stats visible:

| Metric | Value |
| --- | --- |
| Monthly Tokens | 20T |
| Global Users | 4.2M+ |
| Active Providers | 60+ |
| Models | 500+ |

- Featured models with metrics (e.g., Gemini 2.5 Pro, GPT-5, Claude Sonnet 4.5) showing tokens/wk, latency, weekly growth
- Filters by input/output modalities (text, image, file, audio), context length, pricing, series (GPT, Claude, Gemini), categories (programming, roleplay, etc.)

### Exploring GPT Series on OpenRouter

- **Top proprietary closed-source models**: GPT, Claude, Gemini
- Filters to **GPT series** and selects **GPT-5 Pro**
    - Usage: 711M tokens (likely weekly)
    - Context length: 400K tokens
        - Indicates maximum tokens model can process in one interaction
    - Pricing:

| Type | Cost per Million Tokens |
| --- | --- |
| Input | $15 |
| Output | $120 |

- Additional GPT variants visible (e.g., GPT-5 Image, o3 Deep Research, GPT-5 Codex, GPT-4o Audio) with their own context lengths and pricing

### GPT-5 Pro Pricing and Context Details

- **Context length (400,000 tokens)**: Maximum tokens the model can process at once—its 'window' for looking at input
- **Input vs. output pricing** (per million tokens):

| Type | Cost |
| --- | --- |
| Input | $15 |
| Output | $120 |

    - Input: Cost for tokens we send to the model (prompt)
    - Output: Cost for tokens the model generates in response
    - Charged differently because output requires more computational work

### Parameters & Context Windows

- **400K tokens perspective**: A million tokens is enormous, so 400K remains a huge context window
    - Context windows keep growing larger daily, fundamentally changing how this space operates
- **Parameters**: The model's "knowledge bank"—numerical values storing learned patterns
    - More parameters = greater capability and versatility
- **Context Window**: Maximum information processed per interaction—the model's "working memory"
    - Measured in tokens: 4K tokens ≈ 3,000 words
    - Larger windows enable:
        - Longer conversations
        - Full document analysis
        - More examples in prompts
- Ties back to why this matters for practical use, cost, and capabilities

### Parameters as Model Size

- Parameters indicate **model size** via weights and internal technical components
    - No need to understand formulas—just high-level view
- **7 billion parameter model** vs. **671 billion parameter model**:
    - Smaller (7B): faster, cheaper to host locally
    - Larger (671B): slower, more expensive

### Two Model Types

- **Standard LLMs**:
    - Fast token-by-token generation
    - Examples: GPT-4o, Claude Sonnet, Gemini Pro
    - Use for: quick responses, general tasks (writing, Q&A, summarization)
- **Reasoning Models**:
    - Step-by-step deliberation
    - Examples: OpenAI o3, o4-mini, DeepSeek R1
    - Slower but more accurate
    - Use for: complex problem decomposition (math, coding, scientific logic)
- **Selection tip**: Choose reasoning models when accuracy > speed (e.g., math proofs, competitive programming, debugging)

### Spotting Reasoning Models in ChatGPT

- **Behavior indicators**:
    - Complex questions: Shows 'thinking...' (or 'thought for 40 seconds') before responding
    - Simple queries (e.g., 'what's a definition of gravity'): Instant answers
- Signals more internal reasoning/thinking in reasoning models (slower but more accurate for complex problem decomposition)

### OpenAI Model Families

- **GPT Models**: General-purpose language models
    - Examples: GPT-4o, GPT-3.5, GPT-5
- **Turbo Models**: Speed-optimized GPT variants
    - Examples: 4 Turbo, 3.5 Turbo
    - Typically cheaper
- **O-Series**: Deliberative thinking models
    - Build on reasoning model concept (step-by-step deliberation)

### Evergreen Model Family Patterns

- **Slide icons for quick recognition**:
    - ⚡ **GPT Models**: General-purpose
    - 🚀 **Turbo Models**: Speed-optimized
    - 💲 **O-Series**: Deliberative thinking
- **Evergreen strategy**: Focus on family logic (e.g., 'O' prefix signals reasoning models like o3, o4, o3-mini) rather than version numbers—patterns persist as models evolve for reliable selection

### Anthropic Model Families

- **Sonnet Models**: General-purpose language models
- **Haiku Models**: Speed-optimized variants (usually the cheapest)
- **Opus Models**: Deliberative thinking models
- **Sonnet nuance**: Can enable thinking for deeper processing, making it a hybrid reasoning model (explains why some classify it beyond standard LLMs)

### Anthropic Model Families

- **Sonnet Models**: General-Purpose Language Models
- **Haiku Models**: Speed-Optimized variants
- **Opus Models**: Deliberative Thinking Models
    - Heavy reasoning and thinking
    - Typically larger context
    - Higher cost

### Google Model Families

- **Pro Models**: Flagship "thinking" model for complex reasoning
    - Also general hybrid
- **Flash Models**: Performance-optimized tier balancing cost and speed
    - Super fast, cheapest used, still very good
- **Flash-Lite Models**: Entry-level for huge-scale, text-only workloads
    - Rarely used in practice

### Alternative Models

- Beyond the big three proprietary closed-source providers (OpenAI, Anthropic, Google)
    - Includes other closed-source like **xAI Grok 3**
        - 1M context
        - Real-time X integration, Think Mode
        - Benchmarks: 93.3% AIME math, 84.6% GPQA reasoning
        - Pricing: $3 in / $15 out
    - **Open-source models** (e.g., Meta Llama 4, DeepSeek R1 & V3)
        - Customizable and free (Llama)
        - DeepSeek: 236B params, rivals OpenAI o1
        - Strong in math & coding
        - Extremely cost-effective (\~$2.18 per M tokens)
- **Meta Llama 4 specifics**
    - Scout: 10M token context (record-breaking)
    - Maverick: 400B params, beats GPT-4o

### Cost-Saving Strategies

- **Right-Size Models**
    - Match model power to task needs: use smaller/cheaper models for simpler tasks
    - Avoid overkill like deep reasoning models for basic email classification/tagging
- **Core Principle**: Balance power, speed, and reasoning based on task
    - Sometimes speed isn't needed; sometimes deeper reasoning isn't required
- **Prompt Caching**
    - Cache repeated content for up to 90% savings on redundant processing
- **Batch Processing**
    - Queue non-urgent tasks for 50% discount on processing costs
- **Open-Source Deployment**
    - Llama & DeepSeek eliminate API costs for high-volume use

### Advanced Token Saving & Tools

- **Token Saving Techniques**
    - Process only the most important words
    - Send summaries instead of full text
- **Vellum LLM Leaderboard**
    - Updated 21st of October
    - Latest public benchmarks for SOTA models (post-April 2024)
        - Data from providers + independent evals (Vellum/open-source community)
        - Non-saturated benchmarks (excludes outdated like MMLU)
    - **Top Models per Task**
        - Best in Reasoning (GPQA Diamond)
        - Best in High School Math (AIME 2025)
        - Best in Agentic Coding (SWE Bench)
    - Vellum Evals for custom use-case evaluation

### LLM Benchmarks on Vellum Leaderboard

- Displays latest public benchmarks for SOTA models post-April 2024
    - Data from providers + independent evals by Vellum/open-source community
    - Categories: Reasoning (SFGA Diamond), High-School Math (MAME 2020), Agentic Coding (SWE Bench), Tool Use (BFCL), Adaptive Reasoning (GRND), Overall (Humanity's Last Exam)
- **Top performers highlighted**
    - GPT-5: Recent release, excels across many benchmarks
    - Llama 2 70B: Best in Tool Use; open-source Meta model
    - Others: GPT-4 strong in reasoning/math/coding/adaptive; Claude 2 competitive; AWS noted in tool use; GPT-4-Turbo in Tool Use; Claude 1 in Adaptive
- **Key insight**: Quick visual ranking helps select models by task strength (e.g., Llama for tool use)

### Model Comparison Tools

- Platforms provide independent evals and charts for:
    - Best in Tool Use (RFCL), Adaptive Reasoning (GRND)
    - Fastest models (tokens/second)
    - Lowest latency (TTFT, seconds to first token)
    - Cheapest models (USD per 1M tokens)
- **Head-to-Head Comparisons** (e.g., GPT-4o vs Claude 3.5 Sonnet):

| Metric | GPT-4o | Claude 3.5 Sonnet |
| --- | --- | --- |
| Context size | 128,000 | 200,000 |
| Cutoff date | Oct 2023 | Apr 2024 |
| I/O cost | $2.5 / $10 | $3 / $15 |
| Max output | 4096 | 4096 |
| Latency | 0.51s | 1.22s |
| Speed | 143 t/s | 78 t/s |

- **Cutoff Date**: Knowledge limit from training data cutoff
    - Models unaware of events post-cutoff (e.g., GPT-3.5 may not know recent info)
- Standard benchmarks shown: GPQA Diamond, BFCL, MATH 500, AIME 2024, SWE Bench, Aider Polyglot
- **Additional Comparison Metrics**
    - Max output: tokens limit per response (e.g., 4096 for both GPT-4o and Claude 3.5 Sonnet)
    - Latency: response delay shown as 0.5s (GPT-4o) vs 1.2s (Claude 3.5 Sonnet)
- **LLM Arena for Model Evaluation**
    - Chat with multiple models side-by-side to compare outputs directly
    - Vote on preferred answers to contribute to public leaderboards
    - Leaderboards rank models anonymously by user votes
    - Text arena: Top models like Gemini-7.5-pro (1451), Claude Opus 4.1 (1447), GPT-4.5 (1441)
    - WebDev arena: GPT-4 high (1478), Claude Opus 4.1 (1472), Claude Sonnet 4.5 (1421)
    - Overview snapshots across text, image, vision, etc., with deeper tabs for each
- **Extended Benchmark Table** (selected models)

| Model | GRND | AIME 2024 | GPQA | SWE Bench | MATH 500 | BFCL | Aider Polyglot |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Grok 3 (Beta) | n/a | 93.3% | 84.6% | n/a | n/a | n/a | n/a |
| Gemini 2.5 Pro | 82.1% | 92% | 80.4% | 59.8% | n/a | 82.2% | n/a |
| Llama 4 Maverick | 53.6% | n/a | 69.8% | n/a | n/a | 15.6% | n/a |

- **LLM Arena Voting Process**: Users chat with multiple models side-by-side without knowing which is which, rank preferred answers anonymously to generate leaderboards
- **Gemini 2.6 Pro**: Strong hybrid model leading Text Arena (score 1451) and Vision Arena (score 1241)
- **Specialized Arenas**:
    - **Vision Arena**: Multimodal models for visual inputs (Gemini 2.6 Pro top with 62,824 votes)
    - **Text-to-Image Arena**: Image generation from text (e.g., hunyuan-image-3.0 at 1181)
    - **Image Edit Arena**: Image generation/editing (e.g., gemini-2.6-flash-image-preview at 1342)
    - **Search Arena**: LLMs with web search (e.g., xk-grokk-4-fast-search at 1164)
- **Practical Value**: Use these tools to track general population preferences and latest benchmarks across text, vision, and specialized tasks