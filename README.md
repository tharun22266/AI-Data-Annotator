# Human-in-the-Loop AI Data Annotator

A minimal-code portfolio project for human annotation and quality review of:
- AI chatbot responses
- Customer product/service reviews

## Project goals
Create a repeatable workflow to label text, document annotation decisions, review label quality, and summarize results.

## Features
- Google Colab notebook (no local Python setup required)
- Starter chatbot-response and customer-review CSV datasets
- Interactive annotation widgets
- Labels for relevance, factuality, clarity, safety, bias, sentiment, topic, spam, and priority
- Annotation completion summary and label-distribution chart
- CSV export of annotated datasets
- Written annotation guidelines

## Quick start (Google Colab)
1. Download or clone this repository.
2. Open `notebooks/AI_Data_Annotator_Google_Colab.ipynb` in Google Colab:
   https://colab.research.google.com/
3. Run cells from top to bottom.
4. Use the annotation widgets to label records.
5. Run the export cell and download your labelled CSV files.

The notebook creates starter data if the CSV files are not already present. To use repository datasets, upload `data/raw/chatbot_responses.csv` and `data/raw/customer_reviews.csv` when the optional upload cell asks for files.

## Repository structure
```text
AI_Data_Annotator_GitHub_Ready/
├── data/
│   ├── raw/
│   │   ├── chatbot_responses.csv
│   │   └── customer_reviews.csv
│   └── processed/
├── docs/
│   └── annotation_guidelines.md
├── notebooks/
│   └── AI_Data_Annotator_Google_Colab.ipynb
├── exports/
├── screenshots/
├── .gitignore
├── LICENSE
└── README.md
```

## Annotation labels

### Chatbot responses
- Relevance: Relevant / Partially relevant / Irrelevant / Needs review
- Factuality: Supported / Partially supported / Unsupported / Needs review
- Clarity: Clear / Somewhat unclear / Unclear
- Safety: Safe / Potentially harmful / Needs review
- Bias: No obvious bias / Potential bias / Needs review
- Quality score: 1–5

### Customer reviews
- Sentiment: Positive / Neutral / Negative / Mixed
- Topic: Product quality / Delivery / Price / Customer service / Usability / Other
- Spam: Not spam / Possible spam / Spam
- Language quality: Understandable / Difficult to understand
- Priority: Low / Medium / High

## Quality and research notes
- The included records are illustrative examples for demonstrating the workflow, not a representative or benchmark dataset.
- Factuality labels must be checked against reliable references.
- A completion percentage is not the same as annotation accuracy.
- Do not claim annotation accuracy without independently verified gold/reference labels.
- Inter-annotator agreement requires at least two annotators to label the same records independently. Cohen's kappa measures agreement adjusted for chance, not truth.
- Use `Needs review` when evidence is insufficient.
- Do not upload private, confidential, or personally identifying data.

## Suggested future improvements
- Add a second independent annotator workflow.
- Calculate Cohen's kappa for selected categorical labels.
- Add a review queue for uncertain or conflicting labels.
- Expand datasets using clearly licensed public data and document each source.
- Add a Streamlit dashboard for local deployment.

## Author
Add your name, course, institution, and contact details here before publishing.
