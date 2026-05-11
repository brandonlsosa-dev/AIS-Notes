---
title: Vector Embeddings - Build Your Portfolio · AI Automation Society Plus
description: >-
  Doc & Transcript What This Module Covers "Magic numbers" helping AI understand
  and compare data types. Key Learning Outcomes Basics - Convert data to
  numerical 
author: Build Your Portfolio · AI Automation Society Plus
source: >-
  https://www.skool.com/ai-automation-society-plus/classroom/d99017d2?md=bf61acad011c41d8af1f6041c4c63177
created: "2026-05-11"
tags:
  - hover-notes
  - skool
---

## Vector Embeddings

- **[What are they?]** Representations of media (images, sounds, or large amounts of text)
    - They help computers understand and compare semantics

### Types of Embeddings

- **Text Embeddings**
    - Capture the meaning of text
    - Show context and semantic relationships
- **Image Embeddings**
    - Represent visual features
    - Reveal visual context, patterns, and relationships
- **Audio Embeddings**
    - Capture sound patterns
    - Reveal temporal and melodic relationships
- **Video Embeddings**
    - Capture images and motion over time
    - Show temporal patterns and action detection
- **Multimodal Embeddings**
    - Combine data types (e.g., text + images)
    - Enable cross-modal relationships
- **Graph Embeddings**
    - Represent relationships in networks
    - Reveal social, structural, and connection systems
- **tabular Data Embeddings**
    - Capture patterns in tabular data
    - Reveal patterns and relationships in data tables

### Practical Application of Embeddings

- **[Personal Workflow]** For processing large amounts of text for AI agents, the speaker uses `text-embedding-3-small`
    - This model is used to convert "big walls of text" into a format the AI can effectively read and use within a vector database

### The Core Concept of Embeddings

- **[What they are]** Numbers that represent complex data
    - They act as a bridge to help AI and computers understand different data types (text, images, audio, etc.) entering a vector database
    - These numbers capture the unique qualities and specific characteristics of an item

### Semantic vs. Surface Similarity

- Embeddings prioritize semantic meaning over superficial patterns
    - **Text example**: The word "cat" is semantically closer to "kitten" than to "car", even though "cat" and "car" might look more similar visually/orthographically
    - **Image example**: An image of a beach is more semantically similar to an image of water than to an image of a mountain

### Text Embeddings

- **[Purpose]** To capture the semantic meaning of sentences, documents, or numbers
- **Text Splitting Strategies**
    - Before embedding, text must be split into manageable chunks
    - Different methods are used depending on how you want to preserve context:
        - `Character splitter`
        - `Recursive splitter`
        - `Token splitter`
        - Splitting based on punctuation
- **The Embedding Process**
    - Uses specific models to transform text into vectors
    - The goal is to ensure that text with similar meanings are positioned near each other in the vector space

### Types of Vector Embeddings

- **Image Embeddings**
    - Represent the visual features of an image
    - **[How it works]** Similar images result in similar vectors
    - **[Real-world use case]** Google Image Search, where searching for a concept returns visually or semantically related images
- **Audio Embeddings**
    - Encodes and transcribes audio data into a vector format

### Video Embeddings

- **[How it works]** Combines both image and motion data
    - Processes individual frames from the video
    - Adds temporal data to capture changes and movement over time

### Multimodal Embeddings

- **[Definition]** Embeddings that combine multiple different data types into a single vector
    - Integrates various sources such as text, images, PDFs, and binary data
    - Requires a method to link and integrate these disparate data sources into one cohesive embedding
- **[Use Case]** Enabling highly complex searches
    - Allows for queries that span different media types (e.g., searching for a text description to find a specific image or video segment)

### Graph Embeddings

- **[Purpose]** To represent entities, relationships, and networks
    - Captures how different points (nodes) are connected to one another
    - Useful for modeling social media networks, specific graph structures, or numerical data visualizations
- **[Use Case]** Predicting connections
    - Can be used to predict potential connections within a social network

### Tabular Embeddings

- Represents structured data
    - Functions similarly to relational schemas found in a SQL warehouse
    - Uses tables and keys to establish relationships between different data points
    - Each row in the table represents a single entity or observation

### Tabular Embeddings (cont.)

- **[How it works]** Represents structured data similar to relational schemas in a SQL warehouse
    - Data is organized into tables with keys that align to establish relationships
    - Each row represents a single entity or observation (e.g., a family)
- **[Use Cases]**
    - **Predictive modeling**: Using the correlations between rows to predict outcomes
    - **Recommendation systems**: Leveraging the inherent relationships within structured data to suggest items

### OpenAI Text Embeddings

- Primary versions include `text-embedding-3-small` and `text-embedding-3-large`
- **`text-embedding-3-small`&#32;characteristics:**
    - Faster and uses fewer resources
    - Produces lower dimensional vectors
    - Ideal for general-purpose tasks and quick lookups

### OpenAI Text Embeddings (cont.)

- **`text-embedding-3-large`&#32;characteristics:**
    - More detailed and captures subtle information
    - Produces higher dimensional vectors
    - **[Use Case]** Perfect for very complex, in-depth searches of specific data
- **Comparison Summary**
    - Use `text-embedding-3-small` for basic matching and general-purpose applications
    - Use `text-embedding-3-large` when you need to perform "deep dives" into the data

### Summary of Embeddings

- **[Core Concept]** Embeddings turn different types of data into "magic vector numbers"
    - This process allows an AI to store data in a vector database
    - Once embedded, the AI can effectively find relationships between different data points
- **[Practical Takeaway]** You don't need to be an expert to build functional AI agents
    - Having a basic grasp of vectors and token splitters is enough to get agents running as desired
