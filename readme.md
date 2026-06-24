# TakeMeter – FIFA World Cup Comment Classifier

## Project Overview
This project classifies FIFA World Cup Reddit comments into four categories: Analysis, Prediction, Reaction, and Other. It compares a zero-shot baseline model with a fine-tuned DistilBERT model.

---

## Labels

- Analysis: Comments that explain or describe events using facts or reasoning  
- Prediction: Comments that predict future outcomes  
- Reaction: Emotional or opinion-based comments  
- Other: Questions or unrelated/logistical comments  

---

## Models Used

- Zero-shot baseline (Groq: llama-3.3-70b-versatile)
- Fine-tuned DistilBERT (distilbert-base-uncased)

---

## Dataset

- Source: `world_cup_comments.csv`
- Size: 36 labeled test examples
- Format: text + label_id

---

## Evaluation Method
Both models were evaluated on the same test set using accuracy, classification report, and confusion matrix.

---

## Evaluation Results

### Baseline accuracy
- 0.611

### Fine-tuned accuracy
- 0.417

---

## Confusion Matrix
See `confusion_matrix.png`

---

## Error Analysis (Baseline Model)

1. “The people do for the most part”  
   - True: Reaction  
   - Predicted: Other  

2. “I went Harry to win so badly”  
   - True: Reaction  
   - Predicted: Prediction  

3. “I think the atmosphere down there tomorrow will be unlike anything Seattle has ever experienced”  
   - True: Reaction  
   - Predicted: Analysis  

---

## Demo

A screen recording of the model running predictions and showing evaluation results is included in the repository.

- File: `data/demo2.mov`

## Demo
Demo video included in repo:

![Demo](./data/demo2.mp4)

The demo shows:
- 3–5 sample predictions from the model
- Correct and incorrect prediction examples
- Final evaluation output including accuracy and confusion matrix

---

## Files Included

- world_cup_comments.csv
- evaluation_results.json
- confusion_matrix.png
- README.md

---

## Conclusion
The fine-tuned model did not outperform the baseline in this run, but it still learns patterns in the classification task. Most errors come from short or ambiguous comments, and Reaction is the most commonly confused label.