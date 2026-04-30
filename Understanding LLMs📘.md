---
title: Understanding LLMs📘 - Build Your Portfolio · AI Automation Society Plus
description: >-
  Transcript Module Summary This module provides a beginner-friendly overview of
  tokens and context windows — two of the most important concepts for
  understanding
author: Build Your Portfolio · AI Automation Society Plus
source: >-
  https://www.skool.com/ai-automation-society-plus/classroom/d99017d2?md=dc2e349aa4bc48829b74752d1d48fb52
created: "2026-04-30"
tags:
  - hover-notes
  - skool
---

## Understanding LLM Tokens

### Beginner's Guide to How AI Reads and Processes Language

- High-level overview (not technical)
    - Goal: Get familiar with the words/terms
    - Understand what they mean when heard or seen

### What Are Tokens?

- Tokens are the basic building blocks LLMs use to understand text
    - Think of them as the "atoms" of language for AI systems
- Examples of tokens:
        - Complete words: "apple"
        - Word fragments: "ham-bur-ger"
        - Punctuation: "!"
        - Spaces: between words

## Why Tokens Matter

- **Tokenization**: Process of chunking text into tokens for LLMs to understand
- Tokens cost money
- Models have maximum token limits
    - Causes "this is too long" messages in ChatGPT or Claude

### Token Limits in Practice

- Models have fixed token windows (e.g., this ChatGPT version: 200,000 tokens max)
    - Exceeding it (e.g., 240,000 tokens) triggers 'can't process all at once'
    - Solution: Split input (e.g., first 120,000 tokens, then second 120,000)

### How Text Becomes Tokens

- AI processes via **tokenization** (not whole words)
- Example: "Hello world!" = 3 tokens total

```javascript
1. "Hello"          → 1 token
  2. " world"         → 1 token (space included)
  3. "!"              → 1 token
```

### Token Estimates for English Text

- Quick rough estimates (not source of truth)
    - 4 characters ≈ 1 token
    - 0.75 words ≈ 1 token
    - 75 words ≈ 100 tokens
    - 30 tokens ≈ 1-2 sentences
    - 100 tokens ≈ 1 paragraph

| Metric | ≈ Tokens/Units |
| --- | --- |
| 4 Characters | 1 token |
| 0.75 Words | 1 token |
| 75 Words | 100 tokens |
| 30 Tokens | 1-2 sentences |
| 100 Tokens | 1 paragraph |

### Scale of Token Limits

- A 200,000 token context window holds **a lot, a lot, a lot** of text
    - Tokens are 'less than you think' — meaning each token packs more text content than expected
    - Ties back to estimates: e.g., 100 tokens ≈ 1 paragraph, so 200k tokens = enormous document size

### Demo: Token Usage for Transcript Analysis

- Demo pasting entire transcript (10-20 minutes of text) + chat input into AI
    - AI reads: recent chat + full transcript
- Total tokens used: **4,000**
        - Shows how even lengthy transcripts fit well within large token limits

### Token Count Example: 10-Min Video

- 10-minute YouTube video transcript = **4,956 promptTokens** (visual) or **\~4,500 tokens** (audio)
    - Plus **537 completionTokens**, **totalTokens 4,953**
    - Puts scale in perspective: 200,000 token limit holds **a lot** of content

### Why Token Size Varies

- LLMs use **Byte-Pair Encoding (BPE)** to efficiently handle any text
    - Breaks text into subword units
- **Common words**: 1 token each
    - "the" = 1 token
    - "and" = 1 token
    - "you" = 1 token
- **Less common words**: Multiple tokens
    - "unbelievable" = 3 tokens ("un" + "believ" + "able")
- **Rare words**: Split into individual letters
    - "asdfghjkl" = 9 tokens
- **Key benefit**: Handles any text, even unseen words

### Why Token Size Varies

- LLMs use **Byte-Pair Encoding (BPE)** to handle text efficiently
    - No need to know exact formula for building systems, pricing, or windows
- **Common words**: 1 token each
        - "the" = 1 token
        - "and" = 1 token
        - "you" = 1 token
- **Less common words**: broken into fragments
        - "unbelievable" = 3 tokens
            - "un" + "believ" + "able"
        - Not always by syllables
- **Rare words**: split into individual letters
        - "asdfghjkl" = 9 tokens
- Allows AI to handle **any text**, even unseen words

### Understanding Context Windows

- AI's **working memory** — maximum tokens it can process at once
- **What's included?**
    - 01. Your prompt (questions or instructions)
    - 02. Conversation history (all previous messages)
    - 03. System instructions (background guidance)
    - 04. AI's response (generated output)

### Context Window Components

- **Prompt tokens** include:
    - User prompt (e.g., questions/instructions like 'what is the best way to get my first client?')
    - Conversation history (all previous messages, if any)
    - System instructions (background guidance)
    - Full input text (e.g., video transcript)
- **Completion tokens**: AI's generated response/output
- Ties to workflow: chat message received → AI agent (chat mode, memory, tools) → model processes → output

### Context Window Components (Continued)

- **Conversation history**: All previous messages (if any)
    - Counts toward the total tokens in working memory
    - No history in current example, but would add if present

### Model Context Window Comparison

- Different models have varying limits:
    - **Gemini 2.5 Flash**: 1,000,000 tokens
    - **GPT-5**: \~400,000 tokens
    - **Claude 4 Opus**: \~200,000 tokens

| Model | Context Window (tokens) |
| --- | --- |
| Gemini 2.5 Flash | 1,000,000 |
| GPT-5 | ~400,000 |
| Claude 4 Opus | ~200,000 |

- **Larger windows** = more memory (handles bigger inputs/history)
    - But also **higher costs**

### Factors for Choosing a Model

- Key factors to consider for your use case:
    - **Speed**
    - **Cost**
    - **Token window size**
    - **Use case specifics** (e.g., coding? writing?)
    - Other factors
- Models vary, so match to your needs

### Why Context Windows Matter

- **Three key reasons** to consider when choosing models:
    - **Memory Limitations**
        - Exceed limit → AI "forgets" earlier conversation parts
    - **Cost Implications**
        - Pay for **every token** in context window **per request**
        - Costs multiply in long conversations
    - **Model Selection**
        - Match window to task:
            - Small: quick chats
            - Medium: documents
            - Large: books

| Reason | Implication |
| --- | --- |
| Memory Limitations | Exceed → AI forgets earlier parts |
| Cost Implications | Pay per token per request; multiplies in long convos |
| Model Selection | Small (chats), medium (docs), large (books) |

- Larger windows = more memory (typically more expensive, but not always)

### Token Pricing: What You Pay

- AI providers charge **based on tokens**, not words
    - **Input tokens** (prompt tokens): Your prompts, questions, context — **lower cost**
    - **Output tokens** (completion tokens): AI-generated responses — **3-4x higher cost**

| Model | Input (per 1M tokens) | Output (per 1M tokens) |
| --- | --- | --- |
| Gemini 2.5 Flash | $0.15 | $0.60 |
| GPT-5 | $1.25 | $10.00 |
| Claude 4 Opus | $15.00 | $75.00 |

- Ties to n8n demo: **promptTokens** = input, **completionTokens** = output, **totalTokens** = sum (charged separately at different rates)

### Key Takeaways on Tokens and Context

- **Tokens ≠ words**: Smaller units like characters, spaces, word fragments
- **Cost follows usage**: Every processed token (input + output) adds to bill
- **Context = memory limit**: Fixed tokens per model it can remember at once
- **Optimization matters**: Use shorter prompts, concise responses, smart model choices to save money
- **Choose wisely**: Match context window size and model capability to your needs
- Pricing varies **widely** across models
    - Context windows differ too
    - Factor in: speed, cost per million tokens, token window, use case (coding? writing? etc.)

### Token Optimization Strategies

- **Limit inputs and outputs**: Control what goes into prompts and what AI generates to manage token usage
- **Be concise**: Shorter prompts and responses reduce tokens processed
    - Saves money tied to every token (input + output)
- **Choose right model**: Match to use case considering speed, cost, window size

### Context as Working Memory

- Context = AI's working memory: everything it can look at at once
    - Fixed per model; fixed token limit

### Final Advice

- **Choose wisely**: Sum of all points — align model context window and capabilities to actual needs

---

### Tokenomics

- Term for being **efficient and economical** with tokens
    - Covers prompting and AI-generated responses