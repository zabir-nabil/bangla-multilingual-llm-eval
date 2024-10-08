# bangla-multilingual-llm-eval

## Summarization Results

| Model         | Prompts          | ROUGE-L F    | ROUGE-L Precision | ROUGE-L Recall   | BERT Precision  | BERT Recall     | BERT F1       | BLEU         |
| ------------- | ---------------- | ------------ | ----------------- | ---------------- | --------------- | --------------- | ------------- | ------------ |
| GPT-3.5 Turbo | Zero Shot        | 0.1109       | 0.1117            | 0.1200           | **0.7071**      | 0.7089          | 0.7076        | 0.2800       |
| GPT-3.5 Turbo | Three Shot       | 0.1140       | 0.1049            | 0.1500           | 0.6922          | 0.7133          | 0.7019        | 0.2570       |
| GPT-3.5 Turbo | Chain of Thought | 0.1050       | 0.0836            | 0.1589           | 0.6261          | 0.6775          | 0.6504        | 0.1718       |
| GPT-4o        | Zero Shot        | **0.1357**   | **0.1161**        | 0.1766           | 0.7025          | **0.7372**      | **0.7190**    | **0.3039**   |
| GPT-4o        | Three Shot       | **0.1483**   | **0.1459**        | 0.1603           | **0.7234**      | **0.7347**      | **0.7287**    | **0.3387**   |
| GPT-4o        | Chain of Thought | **0.1405**   | **0.1282**        | 0.1662           | 0.7026          | 0.7295          | **0.7155**    | **0.3121**   |
| gemini-1.5-flash  | Zero Shot        | 0.1098    | 0.0973            | 0.1346         | 0.7014         | 0.7233      | 0.7119   | 0.3141 |
| gemini-1.5-flash  | Three Shot       | 0.1112    | 0.1018            | 0.1316         | 0.7033         | 0.7218      | 0.7121   | 0.3196 |
| gemini-1.5-flash  | Chain of Thought | 0.1121    | 0.0976            | 0.1410         | 0.6990         | 0.7242      | 0.7110   | 0.3148 |
| Aya 101       | Zero Shot        | 0.1109       | 0.1117            | 0.1200           | **0.7071**      | 0.7089          | 0.7076        | 0.2800       |
| Aya 101       | Three Shot       | 0.1140       | 0.1049            | 0.1500           | 0.6922          | 0.7133          | 0.7019        | 0.2570       |
| Aya 101       | Chain of Thought | 0.1050       | 0.0836            | 0.1589           | 0.6261          | 0.6775          | 0.6504        | 0.1718       |
| bloom-7b1     | Zero Shot        | 0.0534       | 0.0288            | **0.4376**       | 0.6150          | **0.7384**      | 0.6707        | 0.0354       |
| bloom-7b1     | Three Shot       | 0.0319       | 0.0166            | **0.4480**       | 0.5651          | 0.6503          | 0.6046        | 0.0203       |
| bloom-7b1     | Chain of Thought | 0.0293       | 0.0152            | **0.4419**       | 0.5551          | 0.6386          | 0.5938        | 0.0183       |
| LLaMA   | Zero Shot   | 0.1150    | 0.1007            | 0.1542         | 0.6954         | 0.7228      | 0.7083  | 0.2663 |
| LLaMA   | Three Shot   | 0.1085    | 0.1113            | 0.1232         | 0.7031         | 0.7100      | 0.7059  | 0.2570 |
| LLaMA     | Chain of Thought     | 0.0783    | 0.0655            | 0.1535         | 0.6416         | 0.6945      | 0.6659  | 0.1660 |

## Classification Results
| Model         | Prompts          | Accuracy  | Precision | Recall   | F1 Score | AUC-ROC  | Log Loss |
| ------------- | ---------------- | --------- | --------- | -------- | -------- | -------- | -------- |
| GPT-3.5 Turbo | Zero Shot        | 0.5455    | 0.4582    | 0.4463   | 0.4388   | 0.7528   | 11.8022  |
| GPT-3.5 Turbo | Three Shot       | 0.5859    | 0.5618    | 0.4793   | 0.4792   | 0.7730   | 11.7135  |
| GPT-3.5 Turbo | Chain of Thought | 0.1354    | 0.3590    | 0.1107   | 0.1535   | 0.5572   | **7.5751** |
| GPT-4o        | Zero Shot        | **0.7697**| **0.8012**| **0.7697**| **0.7449**| **0.8705**| 8.3010   |
| GPT-4o        | Three Shot       | **0.8505**| **0.8571**| **0.8505**| **0.8454**| **0.9159**| **5.3883** |
| GPT-4o        | Chain of Thought | **0.7414**| **0.8151**| **0.7414**| **0.7324**| **0.8545**| 9.3204   |
| gemini-1.5-flash  | Zero Shot        | 0.6848   | 0.7057    | 0.6164 | 0.6170   | 0.8235  | 10.9490  |
| gemini-1.5-flash  | Three Shot       | 0.6990   | 0.6433    | 0.5719 | 0.5761   | 0.8313  | 10.5076  |
| gemini-1.5-flash  | Chain of Thought | 0.5737   | 0.6070    | 0.4694 | 0.4880   | 0.7626  | 14.0649  |
| Aya 101       | Zero Shot        | 0.5818    | 0.7139    | 0.4760   | 0.5256   | 0.7848   | **4.0550** |
| Aya 101       | Three Shot       | 0.7273    | 0.7158    | 0.5950   | 0.6227   | 0.8559   | 4.5848   |
| Aya 101       | Chain of Thought | 0.6384    | 0.6909    | 0.5223   | 0.5549   | 0.8093   | 5.8908   |
| bloom-7b1     | Zero Shot        | 0.1111    | 0.0123    | 0.1111   | 0.0222   | 0.5000   | 30.7011  |
| bloom-7b1     | Three Shot       | 0.1111    | 0.0123    | 0.1111   | 0.0222   | 0.5000   | 30.7011  |
| bloom-7b1     | Chain of Thought | 0.1111    | 0.0123    | 0.1111   | 0.0222   | 0.5000   | 30.7011  |
| LLaMA  | Zero Shot   | 0.46     | 0.54      | 0.41   | 0.42     | 0.70    | 19.44    |
| LLaMA  | Three Shot   | 0.47     | 0.57      | 0.42   | 0.44     | 0.70    | 19.22    |
| LLaMA     | Chain of Thought     | 0.38     | 0.43      | 0.31   | 0.32     | 0.66    | 22.35    |


## Sentiment Analysis Results
| Model         | Prompts          | Accuracy  | Precision | Recall   | F1 Score | AUC-ROC  | Log Loss |
| ------------- | ---------------- | --------- | --------- | -------- | -------- | -------- | -------- |
| GPT-3.5 Turbo | Zero Shot        | 0.3654    | 0.3462    | 0.3600   | 0.3529   | 0.3652   | 22.8739  |
| GPT-3.5 Turbo | Three Shot       | 0.9295    | 0.9706    | 0.8800   | 0.9231   | **0.9277**   | 2.5415 |
| GPT-3.5 Turbo | Chain of Thought | 0.0192    | 0.0125    | 0.0133   | 0.0129   | 0.0190   | 35.3505  |
| GPT-4o        | Zero Shot        | **0.9551**| **0.9857**    | 0.9200   | **0.9517**   | 0.9538   | **1.6173** |
| GPT-4o        | Three Shot       | **0.9744**| **0.9863**| **0.9600**| **0.9730**| **0.9738**| **0.9242** |
| GPT-4o        | Chain of Thought | **0.9872**| **0.9867**| **0.9867**| **0.9867**| **0.9872**| **0.4621** |
| gemini-1.5-flash  | Zero Shot        | 0.9103   | 0.9692    | 0.8400 | 0.9000   | 0.9077  | 3.2347   |
| gemini-1.5-flash  | Three Shot       | 0.8718   | 0.9825    | 0.7467 | 0.8485   | 0.8672  | 4.6210   |
| gemini-1.5-flash  | Chain of Thought | 0.8782   | 0.8684    | 0.8800 | 0.8742   | 0.8783  | 4.3899   |
| Aya 101       | Zero Shot        | 0.3654    | 0.3462    | 0.3600   | 0.3529   | 0.3652   | 22.8739  |
| Aya 101       | Three Shot       | 0.9295    | 0.9706    | 0.8800   | 0.9231   | **0.9277**   | 2.5415 |
| Aya 101       | Chain of Thought | 0.0192    | 0.0125    | 0.0133   | 0.0129   | 0.0190   | 35.3505  |
| bloom-7b1     | Zero Shot        | 0.4808    | 0.4808    | **1.0000**| 0.6494   | 0.5000   | 18.7150  |
| bloom-7b1     | Three Shot       | 0.4808    | 0.4808    | **1.0000**| 0.6494   | 0.5000   | 18.7150  |
| bloom-7b1     | Chain of Thought | 0.4808    | 0.4808    | **1.0000**| 0.6494   | 0.5000   | 18.7150  |
| LLaMA  | Zero Shot         | 0.7692   | 0.7532    | 0.7733 | 0.7632   | 0.7694  | 8.3178   |
| LLaMA  | Three Shot        | 0.8526   | 0.7889    | 0.9467 | 0.8606   | 0.8560  | 5.3141   |
| LLaMA  | Chain of Thought   | 0.7115   | 0.6316    | 0.9600 | 0.7619   | 0.7207  | 10.3972  |

## RQA Eval Results
| Model          | Prompts          | Dataset                         | Accuracy  | Precision | Recall  | F1 Score | AUC-ROC  | Log Loss  |
|----------------|------------------|---------------------------------|-----------|-----------|---------|----------|----------|-----------|
| GPT-3.5 Turbo   | Zero Shot        | BEnQA Dataset (8th-Science.csv)    | 0.2149    | 0.1298    | 0.1260  | 0.1239   | 0.6114   | 28.2974   |
| GPT-3.5 Turbo   | Three Shot       | BEnQA Dataset (8th-Science.csv)    | 0.3377| 0.2202| 0.2170| 0.2132   | 0.6717   | 23.8710   |
| GPT-3.5 Turbo   | Chain of Thought | BEnQA Dataset (8th-Science.csv)    | 0.2982    | 0.1923    | 0.1858  | 0.1852   | 0.6529   | 25.2938   |
| GPT-3.5 Turbo   | Zero Shot        | BEnQA Dataset (12th-math.csv) | 0.21595   | 0.06535   | 0.06010 | 0.05855  | 0.63110  | 28.2593   |
| GPT-3.5 Turbo   | Three Shot       |BEnQA Dataset (12th-math.csv) | 0.27700   | 0.11875   | 0.12175 | 0.10940  | 0.61910  | 26.06025  |
| GPT-3.5 Turbo   | Chain of Thought |BEnQA Dataset (12th-math.csv) | 0.28950   | 0.05390   | 0.04330 | 0.04630  | 0.63155  | 25.60865  |
| GPT-3.5 Turbo   | Zero Shot        | BEnQA Dataset (12th-physics.csv)| 0.23130   | 0.14055   | 0.13745 | 0.13470  | 0.63940  | 27.70605  |
| GPT-3.5 Turbo   | Three Shot       | BEnQA Dataset (12th-physics.csv)| 0.27945   | 0.15850   | 0.15785 | 0.15380  | 0.62885  | 25.97155  |
| GPT-3.5 Turbo   | Chain of Thought | BEnQA Dataset (12th-physics.csv)| 0.30830   | 0.15285   | 0.14555 | 0.14710  | 0.64285  | 24.93275  |
| GPT-4o          | Zero Shot        | BEnQA Dataset (8th-Science.csv) | 0.6886| 0.5347| 0.5331| 0.5291| 0.8421| 11.2241 |
| GPT-4o          | Three Shot       | BEnQA Dataset (8th-Science.csv) | **0.7325**| 0.5836| 0.5742| 0.5751| **0.8613**| **9.6433**  |
| GPT-4o          | Chain of Thought | BEnQA Dataset (8th-Science.csv) | 0.6842| 0.5519| 0.5534| 0.5495| 0.8534| 11.3822    |
| GPT-4o         | Zero Shot        | BEnQA Dataset (12th-math.csv)    | 0.4942    | 0.4589    | 0.4557  | 0.4481   | 0.7555   | 18.2322   |
| GPT-4o         | Three Shot       | BEnQA Dataset (12th-math.csv)    | 0.5094    | 0.5254    | 0.4965  | 0.5021   | 0.7867   | 17.6855   |
| GPT-4o         | Chain of Thought | BEnQA Dataset (12th-math.csv)    | 0.4548    | 0.3198    | 0.3028  | 0.2974   | 0.7241   | 19.6523   |
| GPT-4o         | Zero Shot        | BEnQA Dataset (12th-physics.csv) | 0.6812    | 0.6407    | 0.6354  | 0.6357   | 0.8813   | 11.4922   |
| GPT-4o         | Three Shot       | BEnQA Dataset (12th-physics.csv) | 0.6972    | 0.6734    | 0.6701  | 0.6693   | 0.8922   | 10.9149   |
| GPT-4o         | Chain of Thought | BEnQA Dataset (12th-physics.csv) | 0.6719    | 0.6496    | 0.6396  | 0.6404   | 0.8869   | 11.8273   |
| gemini-1.5-flash  | Zero Shot        | BEnQA Dataset (8th-science.csv) | 0.5991   | 0.4198    | 0.4182 | 0.4148   | 0.7900  | 14.4492  |
| gemini-1.5-flash  | Three Shot       | BEnQA Dataset (8th-science.csv) | 0.5399   | 0.3867    | 0.3771 | 0.3763   | 0.7687  | 16.5835  |
| gemini-1.5-flash  | Chain of Thought | BEnQA Dataset (8th-science.csv) | 0.5025   | 0.3578    | 0.3548 | 0.3524   | 0.7462  | 17.9313  |
| gemini-1.5-flash  | Zero Shot        | BEnQA Dataset (12th-math.csv)    | 0.5221    | 0.3394    | 0.3189  | 0.3218   | 0.7274   | 17.2246   |
| gemini-1.5-flash  | Three Shot       | BEnQA Dataset (12th-math.csv)    | 0.4841    | 0.4204    | 0.3619  | 0.3659   | 0.7200   | 18.5936   |
| gemini-1.5-flash  | Chain of Thought | BEnQA Dataset (12th-math.csv)    | 0.4839    | 0.2060    | 0.1865  | 0.1931   | 0.7564   | 18.6044   |
| gemini-1.5-flash  | Zero Shot        | BEnQA Dataset (12th-physics.csv) | 0.5805    | 0.4343    | 0.4350  | 0.4315   | 0.7906   | 16.2609   |
| gemini-1.5-flash  | Three Shot       | BEnQA Dataset (12th-physics.csv) | 0.5842    | 0.4924    | 0.4905  | 0.4872   | 0.8155   | 14.9883   |
| gemini-1.5-flash  | Chain of Thought | BEnQA Dataset (12th-physics.csv) | 0.5489    | 0.3744    | 0.3708  | 0.3709   | 0.7753   | 16.2610   |
| Aya 101    | Zero Shot       | BEnQA Dataset (8th-Science.csv)  | 0.0307   | 0.0009    | 0.0076  | 0.0012   | 0.5007  | 34.9370  |
| Aya 101    | Three Shot      | BEnQA Dataset (8th-Science.csv)  | 0.0833   | 0.0461    | 0.0498  | 0.0454   | 0.5312  | 33.0400  |
| Aya 101    | Chain of Thought| BEnQA Dataset (8th-Science.csv)  | 0.1009   | 0.0565    | 0.0631  | 0.0570   | 0.5411  | 32.4077  |
| Aya 101        | Zero Shot         | BEnQA Dataset (12th-Math.csv)   | 0.18925   | 0.04985   | 0.0460  | 0.02385  | 0.50140  | 29.22195  |
| Aya 101        | Three Shot        | BEnQA Dataset (12th-Math.csv)   | 0.22240   | 0.12685   | 0.1497  | 0.12030  | 0.56820  | 28.02765  |
| Aya 101        | Chain of Thought  | BEnQA Dataset (12th-Math.csv)   | 0.19685   | 0.02855   | 0.0548  | 0.03510  | 0.55390  | 28.94950  |
| Aya 101        | Zero Shot         | BEnQA Dataset (12th-Physics.csv)| 0.13215   | 0.00350   | 0.00945 | 0.00415  | 0.50020  | 31.28075  |
| Aya 101        | Three Shot        | BEnQA Dataset (12th-Physics.csv)| 0.18550   | 0.07020   | 0.0664  | 0.06315  | 0.54005  | 29.35810  |
| Aya 101        | Chain of Thought  | BEnQA Dataset (12th-Physics.csv)| 0.16635   | 0.03130   | 0.04075 | 0.03235  | 0.52565  | 30.04885  |
| bloom-7b1         | Zero Shot        | BEnQA Dataset (8th-Science.csv) | 0.2237   | 0.1277    | 0.1427  | 0.1311   | 0.6184  | 27.9813  |
| bloom-7b1         | Three Shot       | BEnQA Dataset (8th-Science.csv) | 0.0439   | 0.0003    | 0.0063  | 0.0005   | 0.5000  | 34.4628  |
| bloom-7b1   | Zero Shot  | BEnQA Dataset (12th-math.csv)     | 0.2045    | 0.03515   | 0.0642  | 0.04245  | 0.5795   | 28.67355  |
| bloom-7b1   | Three Shot | BEnQA Dataset (12th-math.csv)     | 0.21715   | 0.01005   | 0.04565 | 0.0165   | 0.5000   | 28.21615  |
| bloom-7b1   | Zero Shot  | BEnQA Dataset (12th-physics.csv)  | 0.1960    | 0.0893    | 0.0966  | 0.09115  | 0.59095  | 28.97925  |
| bloom-7b1   | Three Shot | BEnQA Dataset (12th-physics.csv)  | 0.15445   | 0.0015    | 0.00935 | 0.0025   | 0.5000   | 30.47665  |
| LLaMA  | Zero Shot   | BEnQA Dataset (8th-Science.csv)     | 0.0965   | 0.0482    | 0.0436 | 0.0441   | 0.5478  | 32.5658  |
| LLaMA  | Three Shot  | BEnQA Dataset (8th-Science.csv)     | 0.1930   | 0.1141    | 0.1027 | 0.1056   | 0.5986  | 29.0879  |
| LLaMA          | Zero Shot        | BEnQA Dataset (12th-math.csv)    | 0.11685   | 0.01840   | 0.01080 | 0.01260  | 0.54890  | 31.83235  |
| LLaMA          | Three Shot       | BEnQA Dataset (12th-math.csv)    | 0.12840   | 0.02265   | 0.01750 | 0.01895  | 0.56155  | 31.41575  |
| LLaMA          | Zero Shot        | BEnQA Dataset (12th-physics.csv) | 0.12820   | 0.06450   | 0.05965 | 0.06080  | 0.58190  | 31.42250  |
| LLaMA          | Three Shot       | BEnQA Dataset (12th-physics.csv) | 0.17635   | 0.07640   | 0.07150 | 0.07300  | 0.58315  | 29.68800  |

