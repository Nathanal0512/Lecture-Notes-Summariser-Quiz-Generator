# AI-Powered Lecture Notes Summariser and Quiz Generator

**Student:** Nathanal Aji | Student ID: 3358996  
**University:** University of Stirling  
**Course:** Software Engineering  
**Supervisor:** Ms. Jimmy  
**Date:** November 2026  

## Project Overview
An AI-powered application that automatically processes 
lecture notes and generates:
- Concise summaries using BART
- Key concepts using KeyBERT
- Multiple-choice quiz questions using fine-tuned T5

## Files in This Repository
| File | Description |
|------|-------------|
| `Lecture_Notes_Prototype.ipynb` | Main Jupyter Notebook prototype |
| `Prototype ss1.png` | Screenshot 1 - Full pipeline output |
| `Prototype ss2.png` | Screenshot 2 - T5 training loss table |
| `hqa_train_cleaned.csv` | Cleaned HQA training dataset |

## Technologies Used
- Python
- HuggingFace Transformers
- BART (facebook/bart-large-cnn)
- KeyBERT
- T5 (fine-tuned on HQA-Data)
- Jupyter Notebook
- Google Colab

## Dataset
HQA-Data from Mendeley Data  
doi: 10.17632/p85z3v45xk.1

## How to Run
1. Install requirements:
pip install transformers keybert torch sentencepiece
2. Open Lecture_Notes_Prototype.ipynb in Jupyter
3. Run all cells in order
4. Full pipeline runs automatically

## Results
- BART summarisation working successfully
- KeyBERT extracting 8 key concepts
- T5 model trained for 3 epochs
- Training loss reduced from 0.1268 to 0.0992
- Quiz generation producing correct questions
