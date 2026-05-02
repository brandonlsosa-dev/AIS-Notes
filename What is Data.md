---
title: What is Data? 📊 - Build Your Portfolio · AI Automation Society Plus
description: >-
  Doc & Transcript What This Module Covers Data fundamentals for automation
  builders - defining data paths. Key Learning Outcomes Data Types - Structured:
  Spreads
author: Build Your Portfolio · AI Automation Society Plus
source: >-
  https://www.skool.com/ai-automation-society-plus/classroom/d99017d2?md=65868a3130fd4b9782cb20eb5ba0ab66
created: "2026-05-02"
tags:
  - hover-notes
  - skool
---

## What is Data?

- At its core, data is a collection of facts, statistics, or information used for analysis, reasoning, or planning
    - Comes in many forms:
        - Numbers
        - Text
        - Images
        - Sounds
        - Sensor readings
        - Or anything that represents information
- Data is everywhere and powers everything from healthcare to marketing to machine learning

### Why Learn About Data for Automations?

- As automation builders, we define the path data follows:
    - Where it enters (input)
    - How it's processed (logic or AI)
    - What happens next (output or action)
- Over time, need to:
    - Handle unstructured or messy data
    - Convert between data formats
    - Integrate with external APIs (next module)
- Mastering data enables turning ideas into action, building smarter automations, and unlocking full power of AI-driven systems
- Data is the most important foundational element for creating automations (besides the prompt)
- **Garbage in, garbage out** — poor input data leads to poor outputs in automations
    - Data quality is crucial for seamless integration and adopting the right tone/subject matter expertise
- Data (with the prompt) forms the most important foundation for creating effective automations

### Basic Data Types

- Terms common in automations and data analytics (universal across tools):
    - **String**: text or words
    - **Float** and **integer**: numbers
    - **Boolean**: true or false

### Structured vs. Unstructured Data

- **Structured Data**:
    - Organized, follows a fixed schema, fits into rows and columns
    - Key characteristics:
        - Tabular format (rows/columns)
        - Consistent schema
        - Easily searchable
        - Stored in relational databases
        - Managed using SQL
    - Examples:
        - Spreadsheets with employee details
        - Customer contact details

### Unstructured Data and Handling Challenges

- **Unstructured Data**:
    - Opposite of structured: lacks fixed schema, doesn't fit neatly into rows/columns
    - Examples: free-form text, images, sounds, sensor readings (messy or variable formats)
- **Handling unstructured/messy data** (key skill over time):
    - Clean and fix inconsistencies
    - Convert between data formats
    - Integrate with **external APIs** (next module)
- **Why APIs enable real power**:
    - Automations can't access external services without them
    - Examples of services needing APIs:
        - Calendar
        - Email
        - CRM
        - Database
    - APIs make end-to-end automation possible across systems

### Unstructured Data Volume and Tools

- Makes up **80-90%** of all data generated today
- **Not searchable** using standard methods
- Requires **specialized tools** (e.g., NLP, AI)

### Expanded Structured Data Examples

- **Additional examples** (beyond spreadsheets/customer details):
    - Financial transaction logs
    - Inventory records

### Expanded Unstructured Data Examples

- **Additional examples**:
    - Text documents and emails
    - Social media posts
    - Photos and videos
- **SQL querying advantage** of structured data:
    - Write queries to filter rows (e.g., 'what was our total sales in March?')
        - Pull every row where sale date equals March
        - Sum up all those sales
    - Enables analytics because data fits predictably into rows/columns
    - Makes it 'easily searchable' as shown in characteristics

### Relational Databases - Linking Tables via Keys

- **How relations work**:
    - Separate tables connected by shared identifiers (e.g., **student ID**)
        - Student table: student ID, name (e.g., Nathan Herkelman), birthday, email
        - Course table: course name, enrolled student IDs, grades
    - Lookup process:

        1. See student ID (e.g., 12) in course table
        2. Query student table using that ID
        3. Retrieve full details (name, birthday, email)

- **Why relational?** Because data is split logically across tables but linked predictably, keeping structured format efficient and searchable with SQL

### Text vs. Numerical Data

- **Text Data (Qualitative)**:
        - Describes qualities or categories—not measured with numbers
        - Examples:
                - Names of people or places
                - Product descriptions
                - Customer feedback
                - Emails or chat logs
                - Text based SCPs
- **Numerical Data (Quantitative)**:
        - Represents measurable quantities

### Semi-Structured Data

- Sits between structured and unstructured
    - Has some organization (like tags or fields)
    - But not enough to fit into a traditional database
- Examples:
        - XML or JSON files
        - Email (structured header + unstructured message)
        - Log files from websites or applications

### Why Data Type Distinctions Matter

- Each type requires different approaches for:
        - Storage
        - Processing
        - Analysis
- Foundation for work in AI, data science, or automation

### Additional Unstructured Data Examples

- Real-world messy formats:
    - PDFs or SOP documents
    - Walls of text
    - Emails
    - Information in CRM systems
- Reiterates: messy data without predictable fixed schema
    - Makes up 80-90% of all data in the world (especially online)

### Numerical Data Characteristics

- **Numerical Data (Quantitative)**:
    - Represents measurable quantities
    - Meaning derived from comparisons (e.g., which is higher/lower)
- **Contrast with Text**:
    - Text: Meaning from word context
    - Numbers: Meaning from relative values

### Types of Numerical Data

- **Discrete**: Countable (e.g., number of products sold)
- **Continuous**: Measurable (e.g., temperature)

### Numerical Data Examples

- Age
- Price
- Website traffic
- Product ratings
- Income
- **Discrete Numerical Data**: Countable, whole numbers only
    - Examples: Number of products sold (12 products—not 12.1 or 12.125)
    - **Why discrete?** Because you can't sell fractional products; it's exact counts
- **Continuous Numerical Data**: Infinitely measurable values
    - Examples: Temperature (73.12569 degrees)
    - **Why continuous?** Can drill down forever; no exact finite value—always more precision possible

**Key distinction**: Discrete = countable steps (integers), Continuous = smooth measurable spectrum (any real number)

- **Numerical Examples Clarification**:
    - Age: Continuous (measurable with precision)
    - Price: Discrete (countable units)
    - Product ratings: Quantitative
    - Income: Quantitative
    - Website traffic: Quantitative (countable visits)

**Key Insight**: Numerical data varies as discrete (exact counts) or continuous (infinite precision), all conveying quantities through comparisons.

- Sits between structured and unstructured
    - Has some organization (tags or fields)
    - But not enough for traditional databases
- **Examples**:
        - XML or JSON files
        - Email (structured header + unstructured message)
        - Log files from websites or applications
- Each data type requires a different approach for:
    - **Storage**
    - **Processing**
    - **Analysis**
- **Key Insight**: Understanding these distinctions is the foundation for any work in AI, data science, or automation