---
title: Data Types 1️⃣ - Build Your Portfolio · AI Automation Society Plus
description: >-
  Doc & Transcript What This Module Covers Essential n8n data types for
  error-free workflows. Key Learning Outcomes Data Types - String: Purple with
  quotes - Numb
author: Build Your Portfolio · AI Automation Society Plus
source: >-
  https://www.skool.com/ai-automation-society-plus/classroom/d99017d2?md=9f5df97f2633437bae72dbbc91110b41
created: "2026-05-04"
tags:
  - hover-notes
  - skool
---

## n8n Data Types

- Data flows through n8n workflows in a structured format, often represented as JSON objects
    - Core data types encountered:
        - **String (Text)**: sequence of characters for text, e.g. `"name": "John Doe"`
        - **Number**:
            - Integer: whole number
            - Float: decimal
        - **Boolean**:
            - True
            - False
        - **Array (Lists)**
        - **Object (Key-Value Pairs)**
        - **Null (Empty Values)**
    - These define how n8n stores and processes data in workflow executions
- Important foundation to avoid complications, errors, or data not moving correctly in workflows

### String Emphasis & Upcoming Topics

- **Strings are the most common data type** you'll encounter in n8n workflows
    - Represent words, phrases, paragraphs
    - Computer distinguishes them as text data flowing through
- **Numbers** follow as another core type
- **Upcoming**: Dedicated section on JSON and key-value pairs (straightforward concept)

### Number Details

- Numbers appear as **integers** (whole numbers) or **floats** (decimals/floating point)
    - In n8n, shown simply as 'Number'
    - Distinction helps understand data processing

### Boolean Details

- **Boolean** values are either **True** or **False** (like yes/no)
    - Used when a key needs binary state
    - Common for conditions and flags in workflows

### Array vs Object Distinction

- **Array (Lists)**: collections of items in sequence
    - Example: array of products (product one, product two, etc.)
    - Just a list of values without keys
- **Object (Key-Value Pairs)**: structured data where each item pairs a key with a value
    - Differs from arrays: not sequential unnamed items, but named pairs
    - Often confused with arrays since both resemble lists of things

### Array, Object, and Null Details

- **Array**: Lists of items
- **Object**: Container of different key-value pairs
    - Full end-to-end JSON example coming up
    - Arrays and objects sometimes confusing — will break them down
- **Null**: Special values (not just 'empty values')
    - Can be confused with empty values, so correcting the label on slide

### Null Clarification

- **Null**: Values that don't exist
    - Distinct from empty strings (e.g., "" vs null)
    - Important distinction to understand for data handling
- Upcoming breakdown for each data type:
    - Quick definitions
    - Examples

### n8n Input/Output Viewing

- Node structure: input on left, output on right
- Multiple views available, starting with **table view**

### n8n Data Views: Table, JSON, and Schema

- **Table view**: Displays data like Google Sheets
    - Headers at top, values in rows
- **JSON view**: Raw JSON format
- **Schema view** (preferred): Makes drag-and-drop easy
    - Collapsible arrows to expand/collapse items
    - Helps navigate structured data cleanly

### String Example in n8n

- Concrete example of strings as data values:
    - Key `name` → value `"John Doe"`
    - Key `email` → value `"john@example.com"`
- Appears in JSON as:

```json
{
      "name": "John Doe"
    }
```

    - Shows "1 item" with expandable `name: John Doe`
- **Key-value analogy**: Keys like Excel column headers, values like data in rows
    - Makes structured data intuitive like spreadsheets
- **Excel analogy continued**: Fields are the column headers; values are the cells within those columns that hold meaning
    - Key `name` → value `John Doe`
- **JSON string indicators**:
    - Quotation marks around value
    - Purple color (indicates string)
- **Schema view string indicator**: `A` next to the field name (A for string data type)

### Boolean Example in n8n

- Boolean values represent true or false
    - Example: `isActive: true`, `hasSubscription: false`
    - Set in set node under 'Fields to Set' with boolean dropdown (true/false options)

### Number Visual Indicators

- JSON: no quotes around value (e.g., `age: 30`), appears green
- Schema view: `#` symbol (e.g., `# age: 30`)

```json
{"age": 30}
```

### Boolean Set Node Demo

- Setting `isActive` field to `true` in n8n Set node
    - Type dropdown set to **Boolean**
    - Provides dropdown with only two options: `true` or `false`
        - Prevents typing arbitrary text (can't enter 'true' manually)
        - Forces selection from checkbox items
- Schema view indicator for boolean: checkbox symbol (not letter like strings)

```json
{"isActive": true}
```

- Matches example: `isActive: true`, `hasSubscription: false`

### Boolean Visual Indicators & Examples

- **JSON boolean cues**: No quotes around `true` or `false` (even though `true` looks like it could be a string)
    - Example: `isActive: true` → appears without quotes
- **Real-world boolean uses**: `isActive`, `hasSubscription`, `is it an adult or child?` → true/false logic

### Array Introduction in n8n

- Arrays are lists of values (any data type)
    - Earlier example: lists of products
- Concrete example: `tags: ["AI", "Automation", "n8n"]`

```json
{
  "tags": [
    "AI",
    "Automation",
    "n8n"
  ]
}
```

- Schema view: Shows `tags` expandable with `tags[0] AI`, `tags[1] Automation`, `tags[2] n8n`

### Array Creation in Set Node

- Arrays shown in JSON with square brackets around items: `["AI", "Automation", "n8n"]`
    - All items marked as strings (`A` indicator in schema view)
    - Indexed access: `tags[0] AI`, `tags[1] Automation`, `tags[2] n8n`

```json
{
  "tags": [
    "AI",
    "Automation",
    "n8n"
  ]
}
```

- **Set node process**: Key `tags`, value entered as `[ "AI", "Automation", "n8n" ]` with commas between items
    - Forces proper array structure

### Object Introduction

- Objects are key-value pairs used to structure data
    - Example starts with `"user": {`

### Array Schema View Details

- Arrays count as **1 item** in schema view, even with multiple elements (e.g., 3 tags = 1 array item)
    - Reason: The array itself is the single item
    - Expandable: `▾ tags` shows `tags[0] AI`, `tags[1] Automation`, `tags[2] n8n`

### Object Example in n8n

- Objects structure data as nested key-value pairs
    - Slide example: `"user": { "id": 101, "name": "Sarah", "email": "sarah@example.com" }`

```json
{
  "user": {
    "id": 101,
    "name": "Sarah",
    "email": "sarah@example.com"
  }
}
```

- Schema view: `▾ user` expands to `id 101`, `name Sarah`, `email&#32;sarah@example.com` (1 item total)
- **Confusion note**: Objects look similar to arrays but use key-value structure

### Object Key-Value Structure vs Arrays

- **Schema similarity to arrays**: Objects appear as **1 item** that's collapsible/expandable (▾ user), just like arrays
    - But inside: **key-value pairs** (`id: 101`, `name: Sarah`, `email: sarah@example.com`) rather than indexed items (`tags[0]`, `tags[1]`)
- **Mixed data types inside objects**:
    - `id`: 101 (number, no quotes, green in JSON)
    - `name`: "Sarah" (string)
    - `email`: "sarah@example.com" (string)

```json
{
  "user": {
    "id": 101,
    "name": "Sarah",
    "email": "sarah@example.com"
  }
}
```

- Schema view expands to:
    - `user`
    - `id 101`
    - `name Sarah`
    - `email&#32;sarah@example.com`

### Null Data Type in n8n

- Null represents empty or missing data
    - Example: `"phone": null`

```json
{
  "phone": null
}
```

- Schema view: `phone null` (1 item)
- **Not null**: Strings like `"phone": "some_number"`
    - Schema view: `phone` with string value (1 item)

```json
{
  "phone": "some_number"
}
```

- **Objects vs Arrays summary**:
    - Objects: Key-value pairs (e.g., `id: 101`, `name: Sarah` – each unique key)
    - Arrays: Indexed lists (e.g., `tags[0] AI`, `tags[1] Automation` – counts up)

### Null Schema View & Empty String Contrast

- Null in schema view: `phone [null]` (1 item, square brackets around null)
    - Visual cue: Two square brackets distinguish it
- **These are not null**: Empty string `""`
    - JSON: `"phone": ""` (quotes around empty value, it's a string)
    - Schema view: `phone ""` (1 item, but string type)

```json
{
  "phone": null
}
{
  "phone": ""
}
```

- Real-world: Null when phone number wasn't provided (missing data), not an empty string

### Empty String vs Null in n8n

- **Empty string behavior**: Set key `phone` as string type, leave value blank, push through
    - JSON: `"phone": ""` (empty quotes around nothing — it's a string)
    - Schema view: `phone` with empty string (no `null` word or brackets)

```json
{
  "phone": ""
}
```

- **Key distinction**: Empty string ≠ null
    - Null: Missing data (`"phone": null`, schema `phone [null]`)
    - Empty string: Actual string value (even if blank), from unfilled Set node string field
- **Practical note**: Won't see null indicator in schema for empty strings — handle separately in workflows

### Data Types Impact on Workflow Logic

- **Filtering empty strings vs null**:
    - If nodes route based on 'field exists': empty string `phone: ""` passes (key exists with string value)
    - True null `phone: null` filters out (missing data)
    - **Watch out**: Empty strings fool 'exists' checks — handle separately
- **Practical impacts by data type**:
    - Boolean: Use in If Nodes for conditional logic
    - Array: Enables looping, bulk processing (e.g., multiple emails)
    - Number: Supports calculations (e.g., pricing workflows)
    - Object: Stores structured data (e.g., user details)

### Workflow Best Practices

- Always inspect data in output panel
- Use right operators in If Nodes
- Convert types to avoid unexpected behavior
- Use Set, Function, Code Nodes to clean/format data
- Test with varied inputs: empty, null, numbers, text for robustness

```json
{"phone": null}  // Filters out on 'not exists'
{"phone": ""}   // Passes 'exists' check
```

- **Objects in form responses**: Each submission = separate object with key-value pairs
    - Example: Object 1 has `name`, `email`, `phone` for one person
    - Object 2 has same keys but different values for another person
    - Handles multiple responses as distinct structured objects
- **Common errors from type mismatches**:
    - 'Expected an object but got a string' when sending data between workflows
    - **Why inspect output panel**: Catches these before they break flows
    - Ties back to data type awareness throughout n8n
- **Core takeaway**: Data type knowledge prevents workflow errors across nodes and integrations
    - Inspect every step, especially inter-workflow data transfers

---

- **Final key distinction: Zero vs null in numbers**
    - Zero: Actual number value (e.g., "how many sales today? 0")
    - Null: Missing data (no value provided)
    - **Why it matters**: Both seem like 'nothing', but behave differently in calculations, filters, logic
        - Zero: Counts as a valid number for math (0 + 5 = 5)
        - Null: Breaks calculations or filters as missing
    - **Practical tip**: Always distinguish in sales, counts, metrics workflows
- **Overall core takeaway**: Data type awareness (including zero/null) prevents real-world errors across n8n workflows