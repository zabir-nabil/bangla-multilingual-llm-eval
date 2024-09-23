# bangla-multilingual-llm-eval

## Summarization Results

| Evaluation Type | Model         | Prompts          | ROUGE-L F    | ROUGE-L Precision | ROUGE-L Recall   | BERT Precision  | BERT Recall     | BERT F1       | BLEU         |
| --------------- | ------------- | ---------------- | ------------ | ----------------- | ---------------- | --------------- | --------------- | ------------- | ------------ |
| Summarization   | GPT-3.5 Turbo | Zero Shot        | 0.1109       | 0.1117            | 0.1200           | **0.7071**      | 0.7089          | 0.7076        | 0.2800       |
| Summarization   | GPT-3.5 Turbo | Three Shot       | 0.1140       | 0.1049            | 0.1500           | 0.6922          | 0.7133          | 0.7019        | 0.2570       |
| Summarization   | GPT-3.5 Turbo | Chain of Thought | 0.1050       | 0.0836            | 0.1589           | 0.6261          | 0.6775          | 0.6504        | 0.1718       |
| Summarization   | GPT-4o        | Zero Shot        | **0.1357**   | **0.1161**            | 0.1766           | 0.7025          | **0.7372**      | **0.7190**    | **0.3039**       |
| Summarization   | GPT-4o        | Three Shot       | **0.1483**   | **0.1459**        | 0.1603           | **0.7234**      | **0.7347**      | **0.7287**    | **0.3387**   |
| Summarization   | GPT-4o        | Chain of Thought | **0.1405**   | **0.1282**        | 0.1662           | 0.7026          | 0.7295          | **0.7155**        | **0.3121**   |
| Summarization   | Aya 101       | Zero Shot        | 0.1109       | 0.1117            | 0.1200           | **0.7071**      | 0.7089          | 0.7076        | 0.2800       |
| Summarization   | Aya 101       | Three Shot       | 0.1140       | 0.1049            | 0.1500           | 0.6922          | 0.7133          | 0.7019        | 0.2570       |
| Summarization   | Aya 101       | Chain of Thought | 0.1050       | 0.0836            | 0.1589           | 0.6261          | 0.6775          | 0.6504        | 0.1718       |
| Summarization   | bloom-7b1     | Zero Shot        | 0.0534       | 0.0288            | **0.4376**       | 0.6150          | **0.7384**      | 0.6707        | 0.0354       |
| Summarization   | bloom-7b1     | Three Shot       | 0.0319       | 0.0166            | **0.4480**       | 0.5651          | 0.6503          | 0.6046        | 0.0203       |
| Summarization   | bloom-7b1     | Chain of Thought | 0.0293       | 0.0152            | **0.4419**       | 0.5551          | 0.6386          | 0.5938        | 0.0183       |

## Classification Results
| Evaluation Type | Model         | Prompts          | Accuracy  | Precision | Recall   | F1 Score | AUC-ROC  | Log Loss |
| --------------- | ------------- | ---------------- | --------- | --------- | -------- | -------- | -------- | -------- |
| Classification  | GPT-3.5 Turbo | Zero Shot        | 0.5455    | 0.4582    | 0.4463   | 0.4388   | 0.7528   | 11.8022  |
| Classification  | GPT-3.5 Turbo | Three Shot       | 0.5859    | 0.5618    | 0.4793   | 0.4792   | 0.7730   | 11.7135  |
| Classification  | GPT-3.5 Turbo | Chain of Thought | 0.1354    | 0.3590    | 0.1107   | 0.1535   | 0.5572   | **7.5751** |
| Classification  | GPT-4o        | Zero Shot        | **0.7697**| **0.8012**| **0.7697**| **0.7449**| **0.8705**| 8.3010   |
| Classification  | GPT-4o        | Three Shot       | **0.8505**| **0.8571**| **0.8505**| **0.8454**| **0.9159**| **5.3883** |
| Classification  | GPT-4o        | Chain of Thought | **0.7414**| **0.8151**| **0.7414**| **0.7324**| **0.8545**| 9.3204   |
| Classification  | Aya 101       | Zero Shot        | 0.5818    | 0.7139    | 0.4760   | 0.5256   | 0.7848   | **4.0550** |
| Classification  | Aya 101       | Three Shot       | 0.7273    | 0.7158    | 0.5950   | 0.6227   | 0.8559   | 4.5848   |
| Classification  | Aya 101       | Chain of Thought | 0.6384    | 0.6909    | 0.5223   | 0.5549   | 0.8093   | 5.8908   |
| Classification  | bloom-7b1     | Zero Shot        | 0.1111    | 0.0123    | 0.1111   | 0.0222   | 0.5000   | 30.7011  |
| Classification  | bloom-7b1     | Three Shot       | 0.1111    | 0.0123    | 0.1111   | 0.0222   | 0.5000   | 30.7011  |
| Classification  | bloom-7b1     | Chain of Thought | 0.1111    | 0.0123    | 0.1111   | 0.0222   | 0.5000   | 30.7011  |

## Sentiment Results
| Evaluation Type | Model         | Prompts          | Accuracy  | Precision | Recall   | F1 Score | AUC-ROC  | Log Loss |
| --------------- | ------------- | ---------------- | --------- | --------- | -------- | -------- | -------- | -------- |
| Sentiment       | GPT-3.5 Turbo | Zero Shot        | 0.3654    | 0.3462    | 0.3600   | 0.3529   | 0.3652   | 22.8739  |
| Sentiment       | GPT-3.5 Turbo | Three Shot       | 0.9295    | 0.9706    | 0.8800   | 0.9231   | **0.9277**   | 2.5415 |
| Sentiment       | GPT-3.5 Turbo | Chain of Thought | 0.0192    | 0.0125    | 0.0133   | 0.0129   | 0.0190   | 35.3505  |
| Sentiment       | GPT-4o        | Zero Shot        | **0.9551**| **0.9857**    | 0.9200   | **0.9517**   | 0.9538   | **1.6173** |
| Sentiment       | GPT-4o        | Three Shot       | **0.9744**| **0.9863**| **0.9600**| **0.9730**| **0.9738**| **0.9242** |
| Sentiment       | GPT-4o        | Chain of Thought | **0.9872**| **0.9867**| **0.9867**| **0.9867**| **0.9872**| **0.4621** |
| Sentiment       | Aya 101       | Zero Shot        | 0.3654    | 0.3462    | 0.3600   | 0.3529   | 0.3652   | 22.8739  |
| Sentiment       | Aya 101       | Three Shot       | 0.9295    | 0.9706    | 0.8800   | 0.9231   | **0.9277**   | 2.5415 |
| Sentiment       | Aya 101       | Chain of Thought | 0.0192    | 0.0125    | 0.0133   | 0.0129   | 0.0190   | 35.3505  |
| Sentiment       | bloom-7b1     | Zero Shot        | 0.4808    | 0.4808    | **1.0000**| 0.6494   | 0.5000   | 17.9340  |
| Sentiment       | bloom-7b1     | Three Shot       | 0.4808    | 0.4808    | **1.0000**| 0.6494   | 0.5000   | 17.9340  |
| Sentiment       | bloom-7b1     | Chain of Thought | 0.4808    | 0.4808    | **1.0000**| 0.6494   | 0.5000   | 17.9340  |
