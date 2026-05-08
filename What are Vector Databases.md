---
title: What are Vector Databases? - Build Your Portfolio · AI Automation Society Plus
description: >-
  Doc & Transcript What This Module Covers "Smart libraries" storing data as
  numerical vectors for AI comparison. Key Learning Outcomes Basics - Store data
  as num
author: Build Your Portfolio · AI Automation Society Plus
source: >-
  https://www.skool.com/ai-automation-society-plus/classroom/d99017d2?md=6a065ae9366549f698b1445cd9a596f4
created: "2026-05-08"
tags:
  - hover-notes
  - skool
---

## Intro to Vector Databases

- Builds on RAG: Agents use retrieval augmented generation to access vector databases
- Analogy: A unique kind of library that doesn't just store books
- Stores data as **vectors** (lists of numbers)
    - Helps AI understand complex items like words, images, and sounds

### Vector Storage Basics

- Unlike regular databases using structured data (rows, columns, tables, shelves)
- Stores info as **vectors**: groups of numbers representing certain things
    - Numbers don't resemble original words or pictures
- Like a special library or AI **memory bank**

### Multidimensional Nature of Vectors

- Vectors act as lists of numbers representing text, images, and sounds
    - Designed for computers to understand complex data
- Functions like a **multidimensional relational database**
    - Not limited to 2D (X/Y axes) but extends to 3D and beyond (e.g., 500 dimensions)
    - Data points scatter across multiple dimensions
- **Clustering for similarity**: Related items group together
    - Animals cluster in one area (e.g., bird, fox icons)
    - Fruits in another (e.g., apple)
    - AI finds connections by navigating these multidimensional spaces (e.g., linking to Google, change)

### Definition of a Single Vector

- A **vector** is a list of numbers that describes a complex object
    - Example: Word "car" represented as numbers capturing its meaning
- Numbers derived from the object's **characteristics**
    - AI uses context to position vectors in multidimensional spaces for finding relations

**Example vector**: `(0.34, 2.35, 8.34, ...)` (up to 500 dimensions)

- Numbers in a vector (e.g., **0.34, 2.35, 8.34**) represent **different aspects** of the specific item or text
    - **Similar number structures** place related items **relationally in the same area**
        - Enables AI to identify connections via proximity in multidimensional space
- Vectors help AI understand **characteristics** rather than raw words or images

### Embeddings in Vector Databases

- **Magic behind vector DBs**: Embeddings turn words, images into numbers (vectors)
    - AI uses these groups of vectors to **remember things**
    - Enables matching based on **relationships** (not static hardcoded data)
- **Use cases**:
        - Chatbots/language models: Store relationships for context understanding
- Deeper dive on embeddings coming next
- **Chatbots/language models**: Store relationships between words as vectors to understand conversation context
    - Example: User says "tell me a joke" → AI recognizes intent and responds with humor
- **Image and video recognition**: Enables searching for similar images online
    - Vector DB recognizes patterns, compares, and places similar images near known ones
- **Recommendations**: Suggests similar products online
    - System uses vectors to match based on user activity

### Benefits of Vector Databases

- **Flexibility**: Handles text, images, audio, and more
    - Supports diverse unstructured data types
- **Scalability**: Stores millions or billions of data points
    - Manages massive volumes without issues
- **Speed**: Fast searches and comparisons
    - High performance for quick similarity matching
- Everyday use already familiar (e.g., Google searching)
    - Now configuring them directly for AI agents

### Why Vector Databases are Essential for AI

- Acts as AI's **memory** for understanding and comparing complex info
- Crucial for businesses adding AI capabilities
    - Enables handling high-dimensional, unstructured data like text/images/audio
- Ideal for:
    - Finding similar items (articles, products, sounds)
    - Complex feature comparisons via vector distances
- **Flexibility details**: Handles tons of different types of data — text, images, audio, and more
    - Can just embed them in there without changing or manipulating too much
    - Some optimization exists, but not needed much for today
- **Scalability details**: Stores millions and even billions of data points
    - Perfect for AI models that need tons of information to work well
    - Especially useful when helping out businesses

### When to Use a Vector Database

- **Unstructured Data**: For text, images, or audio
- **Finding Similar Items**: Like related articles, products, or sounds
- **High-Dimensional Data**: For complex features in data

### How Vector Databases are Structured

- Each piece of data (text, image, etc.) is stored as a vector
- AI finds similar items by comparing "distances" between vectors

### Summary

- A vector database is a "smart library" for AI
- Makes it easier for AI to recognize, summarize, and understand complex data

### Speed and Scalability Advantages

- **Scalability for RAG/Agents**: Handles tons of data generated by implementing agents and RAG systems
    - Super scalable for massive data volumes
- **Performance Edge**: Numeric format enables super quick searches, comparisons, and relation-finding
    - Far faster than scanning thousands of rows in an Excel spreadsheet
    - Leads to smoother, much faster AI response processes
- **AI's Memory Role**: Vector DB acts as AI's memory
    - AI pulls info for answering questions, recommendations, keeping conversations going
    - Gives power for context, history, comparisons
- **When to Use Vector vs Structured DBs**
    - Structured (Excel/Airtable): For exact matches in rows/columns
    - **Vector DBs Best For**: Situations needing to find similar items
        - Handles unstructured, high-dimensional data where similarity matters over exact equality

### Vector Database Decision Criteria

- Use vector storage when similarity searching is key (vs. exact lookups in tables)
- **Vector Numbers as Features**: Each number in the vector represents a specific feature or quality of the data
    - Example with cars:
        - First number: how fast the car can go
        - Second number: type of engine
        - Third number: color (this kind of stuff)
    - **Why it works**: Similar vectors cluster close together, so searching for 'vintage blue car with specific engine' finds matches by comparing these feature numbers
    - Enables precise similarity searches in multidimensional space
- **Vector DB Power**: Finds similar things even without hardcoded descriptions (e.g., vintage blue car matches via feature vectors)
- **Core Summary**: Powerful tool for AI handling complex data
    - Helps AI **understand and remember** by clustering similar vectors
    - **Essential for**:
        - Recommendation systems
        - Search engines
        - Any app recognizing patterns from simple natural language keywords
- **Smart Library Analogy**: Captures full essence – AI pulls contextual matches quickly
- **Future Impact**: Vector databases crucial for AI's future
    - Enable creating advanced use cases and applications
    - Far beyond current limitations of Google Sheets

### Vector Indexing Visualization

- **Indexing**: Labeled "BRI WORKS"
- **3D Scatter Plot Demo**: Vectors as blue dots with icons (bird, dog, cat, fox, apple, speech bubble, lightbulb, gear)
    - Related points connected by lines
    - Dimensions shown: "0.34, 2.35, 8.34, ... 300 dimensions"
    - "Change" indicator for dynamic updates or transformations