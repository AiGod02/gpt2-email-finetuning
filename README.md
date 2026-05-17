
# GPT-2 Domain Fine-Tuning — Corporate Email Generation

Fine-tuned GPT-2 on internal company documents (PDF, JSON, HTML) to generate 
domain-specific marketing emails with controllable tone and objective.

Built during an internship at Epack PreFab as a practical exploration of 
causal language model adaptation on proprietary data.

## What this does
- Ingests corporate data from PDF, JSON, and HTML sources
- Cleans and prepares a prompt-output dataset for causal LM training
- Fine-tunes GPT-2 using HuggingFace Trainer
- Generates subject lines, email bodies, and CTAs from a prompt
- Post-processes output: proofreading, humanising, creativity scoring

## Stack
- Python, PyTorch, HuggingFace Transformers
- Google Colab (T4 GPU)
- LanguageTool, BeautifulSoup, PyPDF2

## Usage
Open `Gpt2_finetuned_clean.ipynb` in Google Colab and run top to bottom.  
Update the data paths in Section 3 to point to your own documents.

## Notes
Data used during training is proprietary and not included in this repo.  
Sample outputs in the notebook reflect a real training run on the internship dataset.