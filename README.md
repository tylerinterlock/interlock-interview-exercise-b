# Interlock Systems — Technical Assessment

## About Interlock

Interlock builds AI systems that automate the design-to-manufacturing handoff for contract manufacturers in regulated industries (aerospace, defense, medical devices). Our pipeline ingests manufacturing documents — engineering drawings, spec sheets, BOMs, purchase orders — and extracts, classifies, and cross-references critical data to catch errors before they reach the shop floor.

## Task: Field Extraction & Discrepancy Detection

The `/data/` folder contains a set of manufacturing documents drawn from two **tech packets** — sets of related documents (drawing, spec sheet, BOM, etc.) for the same part.

### Your job:

1. **Parse** the PDFs and **extract** key manufacturing fields from each document.

2. **Cross-reference** the extracted fields across documents that belong to the same part. Flag any discrepancies where two documents disagree on the same field.

3. **Produce a result** that shows what you extracted and any discrepancies you found.

### What we're looking for:

We care about how you **structure the extraction**, how you **handle disagreements** between documents, and how you think about **reliability**. Talk us through your decisions as you go. Use whatever language, framework, and tools you prefer.

## Setup

```bash
# Clone this repo
git clone <repo-url>
cd exercise-b

# Set up your API key (provided at the start of the session)
cp .env.example .env
# Edit .env and add the API key we gave you
```

## API Access

We've provided an OpenRouter API key that gives you access to multiple LLM models (Claude, GPT, Gemini, Llama, etc.) through a single OpenAI-compatible endpoint.

```
Base URL: https://openrouter.ai/api/v1
```

Model choice is part of the exercise.
