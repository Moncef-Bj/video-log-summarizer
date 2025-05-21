#  Video Log Summarizer

This project is a prototype using a Large Language Model (LLM) to automatically summarize video-generated logs, such as surveillance footage or behavioral observation in retail or logistics environments.

---

##  Objective

In settings where video footage generates long, low-level event logs, this tool helps generate concise and readable summaries using natural language generation.  
The goal is to assist operators, analysts, or managers in quickly understanding what happened without having to read raw logs line by line.

---
## 📁 Example

### 📝 Input (raw log text)

[08:00] Camera 1: A customer enters.
[08:05] Camera 2: Customer looks at the beverage shelves.
[08:07] Camera 3: Customer hesitates between two products.
[08:10] Camera 2: Customer places an item in their basket.
[08:12] Camera 1: Customer leaves the frame.
[08:20] Camera 1: Two new customers enter.
[08:25] Camera 4: Customers talk in the central aisle.
[08:30] Camera 2: First customer returns to the fresh food section.
[08:35] Camera 3: One customer puts back a product.
[08:40] Camera 1: Both customers exit the store.


###  Expected Output (summary)

> A first customer entered around 8:00, explored the beverage section, hesitated between two products, selected one, and left the store at 8:12.  
> Around 8:20, two additional customers arrived, briefly interacted in the central aisle, browsed the store, and left before 8:45.

---
## 🚀 Getting Started

### Install dependencies

```bash
pip install -r requirements.txt
```
### Run the summarization script
```bash
python src/summarize_logs.py
```

## Upcoming Features

-Time-window-based summarization (e.g., summaries every 30 minutes)
-Multi-customer tracking and summarization
-Enrichment with behavior classification (e.g., hesitations, group movement)
-Comparison between local and remote LLMs (Mistral, GPT, etc.)

##  Contributions

Contributions are welcome to:
- Enhance the summarization pipeline
- Add new summarization modes or data sources
- Apply the system to new domains (logistics, retail analytics, security)

Feel free to open an issue or a pull request!

## License

This project is licensed under the MIT License.
