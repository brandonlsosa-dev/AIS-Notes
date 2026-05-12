---
title: Context Windows - Build Your Portfolio · AI Automation Society Plus
description: >-
  Doc & Transcript What This Module Covers AI's "attention span" for text
  processing. Key Learning Outcomes Basics - Memory capacity measured in tokens
  - 1,000 to
author: Build Your Portfolio · AI Automation Society Plus
source: >-
  https://www.skool.com/ai-automation-society-plus/classroom/d99017d2?md=aeea5ef374c24284a2a1e753e19232d2
created: "2026-05-12"
tags:
  - hover-notes
  - skool
---

## Understanding Context Windows

- **Definition**: The amount of text an AI model can "remember" and process at one time
    - It functions like the model's attention span or short-term working memory
- **Impact of Window Size**:
        - **Small Context Window**:
                - Can only focus on short passages of text
                - Might forget what happened earlier in a sequence
        - **Large Context Window**:
                - Can analyze entire documents or long conversations
                - Allows the model to remember more of the story/context

### Benefits of a Large Context Window

- **Increased Accuracy**: By referencing earlier context, the model can provide:
    - More accurate general outputs
    - More accurate answers
    - More accurate tool calling

### How Context Windows Work

- AI models do not read like humans
    - They use **tokenization** to break text down into smaller units called tokens
    - This applies to sentences, which get chunked and split up
- Context window measurement
    - The window is measured in **tokens**, not words
    - These tokens are what are sent to the model (e.g., OpenAI) or vector databases (e.g., Pinecone)

### Token and Word Estimation

- A rough rule of thumb for estimating text volume:
    - 1,000 tokens $\approx$ 750 words
    - This is roughly equivalent to one page of text

### Why RAG is Needed

- **The limitation of finite context windows**:
    - When processing books, transcripts, or multiple documents, the total information often exceeds the model's context window.
    - Because the model cannot read an entire book at once, RAG is used to retrieve only the relevant chunks needed to answer a specific question.

### Recent Advances in Context Windows

- Context window sizes are increasing very rapidly
    - Early models like GPT-3.5 Turbo had only 4,000 tokens
    - Current 4.0 models are typically in the 128,000 to 200,000 token range
    - Recent breakthroughs have seen massive jumps, such as moving from 300,000 to 1,000,000 tokens
- **Google's Gemini 2.0 Flash**
    - Features a 1 million token context window
    - This allows the model to process entire PDFs, research papers, or long conversations in one go

### Context Window and Hallucination Rates

- **Correlation with Hallucination Rates**:
    - As models gain larger context windows, hallucination rates tend to decrease
    - **[Why?]** More context provides more information for the model to reference, leading to better reasoning and more truthful outputs
- **Leaderboards and Benchmarks**:
    - Various leaderboards track model performance across different metrics, including context window size and hallucination rates

### Why Larger Context Windows Matter

- **Increased intelligence and utility**:
    - Larger windows allow the AI to scan more text directly rather than relying on pulling small, disconnected chunks.
    - This enables the handling of more complex information and queries without needing to break data into smaller pieces.
- **Key advantages of bigger context windows**:
    - **Answering complex questions**: By considering more information simultaneously.
    - **Analyzing long conversations**: Without forgetting what was said earlier in the interaction.
    - **Processing entire documents**: Without the need for chunking or special retrieval techniques.
    - **Reducing hallucinations**: Because the model has more direct context to reference, leading to more accurate reasoning.

### The Trade-off: Utility vs. Cost

- **[Why it matters]** While larger windows improve performance, they come with a financial implication
- **Increased Token Usage**: More tokens in the context window directly lead to higher costs
- **Model Variability**: Every model has different pricing structures for token usage
- **Cost Efficiency Examples**:
    - DeepSeek recently gained attention for being significantly more affordable (e.g., being 97% cheaper)

### The Cost of Large Context Windows

- **More tokens = Higher costs**: AI companies charge based on the volume of tokens used.
- **More processing power needed**: Larger context windows require more computing resources, making AI slower and more expensive for large-scale use.
- **Business decision: Utility vs. Cost**:
    - Small context windows are sufficient for casual tasks (e.g., simple conversations).
    - For analyzing long documents, a larger context window is necessary, but it comes with a higher price tag.

#### Token Pricing Mechanics

- Costs are split between two types of tokens:
    - **Input tokens**: The text you send to the model.
    - **Output tokens**: The text the model generates in response.
- **Example: OpenAI GPT-4o Pricing** (per 1 million tokens):

| Token Type | Price |
| --- | --- |
| Input | $2.50 |
| Output | $10.00 |

#### Future Cost Trends

- Costs are expected to decrease due to several factors:
    - Expanding context windows becoming more efficient.
    - Token prices becoming more competitive.
    - The rise of **open source** models, which allow users to run them locally and avoid per-token fees.