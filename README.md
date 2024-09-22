# bangla-multilingual-llm-eval

## Summarization Results

| Evaluation Type | Model         | Prompts          | ROUGE-L F | ROUGE-L Precision | ROUGE-L Recall | BERT Precision | BERT Recall | BERT F1 | BLEU  |
| --------------- | ------------- | ---------------- | --------- | ----------------- | -------------- | -------------- | ----------- | -------|-------|
| Summarization   | GPT-3.5 Turbo | Zero Shot        | 0.1109    | 0.1117            | 0.1200         | 0.7071         | 0.7089     | 0.7076 | 0.2800 |
| Summarization   | GPT-3.5 Turbo | Three Shot       | 0.1140    | 0.1049            | 0.1500         | 0.6922         | 0.7133     | 0.7019 | 0.2570 |
| Summarization   | GPT-3.5 Turbo | Chain of Thought | 0.1050    | 0.0836            | 0.1589         | 0.6261         | 0.6775     | 0.6504 | 0.1718 |
| Summarization   | GPT-4o        | Zero Shot        | 0.1357    | 0.1161            | 0.1766         | 0.7025         | 0.7372     | 0.7190 | 0.3039 |
| Summarization   | GPT-4o        | Three Shot       | 0.1483    | 0.1459            | 0.1603         | 0.7234         | 0.7347     | 0.7287 | 0.3387 |
| Summarization   | GPT-4o        | Chain of Thought | 0.1405    | 0.1282            | 0.1662         | 0.7026         | 0.7295     | 0.7155 | 0.3121 |
| Summarization   | Aya 101       | Zero Shot        | 0.1109    | 0.1117            | 0.1200         | 0.7071         | 0.7089     | 0.7076 | 0.2800 |
| Summarization   | Aya 101       | Three Shot       | 0.1140    | 0.1049            | 0.1500         | 0.6922         | 0.7133     | 0.7019 | 0.2570 |
| Summarization   | Aya 101       | Chain of Thought | 0.1050    | 0.0836            | 0.1589         | 0.6261         | 0.6775     | 0.6504 | 0.1718 |
| Summarization   | bloom-7b1     | Zero Shot        | 0.0534    | 0.0288            | 0.4376         | 0.6150         | 0.7384     | 0.6707 | 0.0354 |
| Summarization   | bloom-7b1     | Three Shot       | 0.0319    | 0.0166            | 0.4480         | 0.5651         | 0.6503     | 0.6046 | 0.0203 |
| Summarization   | bloom-7b1     | Chain of Thought | 0.0293    | 0.0152            | 0.4419         | 0.5551         | 0.6386     | 0.5938 | 0.0183 |
