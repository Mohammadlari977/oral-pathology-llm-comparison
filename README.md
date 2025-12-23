# LLM Comparison in Oral Pathology Differential Diagnosis

This repository contains the automation scripts used to evaluate the diagnostic accuracy of multiple Large Language Models (LLMs) in the field of oral pathology.

## Project Overview
The study compares the performance of 10 different LLM variants across 170 clinical cases sourced from the University of Washington Oral Pathology Archives. 

### Models Evaluated:
- **OpenAI:** GPT-4o, GPT-4o-mini
- **DeepSeek:** DeepSeek-Chat, DeepSeek-Reasoner (V3/R1)
- **Anthropic:** Claude 3.5 Sonnet, Claude 3.5 Haiku
- **Google:** Gemini 1.5 Pro, Gemini 1.5 Flash
- **xAI:** Grok-2, Grok-2-mini

## Configuration
- **Cases:** 1–170
- **Runs per Case:** 3
- **Temperature:** 0.7 (Standardized across all models)
- **Platform:** Google Apps Script

## Setup Instructions
1. Create a Google Sheet and open the Apps Script editor.
2. Copy the contents of `Code.gs` into the editor.
3. Navigate to **Project Settings** (gear icon).
4. Add the following **Script Properties** with your private API keys:
   - `OPENAI_API_KEY`
   - `DEEPSEEK_API_KEY`
   - `ANTHROPIC_API_KEY`
   - `GEMINI_API_KEY`
   - `XAI_API_KEY`
5. Ensure your clinical cases are stored as individual Google Docs named "Case 1", "Case 2", etc.

## Data Availability
The clinical case data are derived from the [University of Washington Oral Pathology Case of the Month Archives](https://dental.washington.edu/oral-pathology/case-of-the-month-archives/).

## Citation
If you use this code in your research, please cite it using the DOI provided via Zenodo:
`[Insert your Zenodo DOI here]`
