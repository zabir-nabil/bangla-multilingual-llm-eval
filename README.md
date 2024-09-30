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

## Sentiment Analysis Results
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

## RQA Eval Results
| Evaluation Type | Model          | Prompts          | Dataset                         | Accuracy  | Precision | Recall  | F1 Score | AUC-ROC  | Log Loss  |
|-----------------|----------------|------------------|---------------------------------|-----------|-----------|---------|----------|----------|-----------|
| GPT-3.5 Turbo   | Zero Shot        | BEnQA Dataset (8th-Science.csv)    | 0.2149    | 0.1298    | 0.1260  | 0.1239   | 0.6114   | 28.2974   |
| GPT-3.5 Turbo   | Three Shot       | BEnQA Dataset (8th-Science.csv)    | 0.3377| 0.2202| 0.2170| 0.2132   | 0.6717   | 23.8710   |
| GPT-3.5 Turbo   | Chain of Thought | BEnQA Dataset (8th-Science.csv)    | 0.2982    | 0.1923    | 0.1858  | 0.1852   | 0.6529   | 25.2938   |
| GPT-3.5 Turbo   | Zero Shot        | BEnQA Dataset (12th-math-1.csv)   | 0.2222    | 0.0809    | 0.0734  | 0.0717   | 0.6697   | 28.0340   |
| GPT-3.5 Turbo   | Three Shot       | BEnQA Dataset (12th-math-1.csv)   | 0.2803| 0.1203    | 0.1338| 0.1170   | 0.6459   | 25.9405   |
| GPT-3.5 Turbo   | Chain of Thought | BEnQA Dataset (12th-math-1.csv)   | 0.3207| 0.0536    | 0.0426  | 0.0461   | 0.6524   | 24.4842   |
| GPT-3.5 Turbo   | Zero Shot        | BEnQA Dataset (12th-math-2.csv)   | 0.2097    | 0.0498    | 0.0468  | 0.0454   | 0.5925   | 28.4846   |
| GPT-3.5 Turbo   | Three Shot       | BEnQA Dataset (12th-math-2.csv)   | 0.2737| 0.1172| 0.1097  | 0.1018   | 0.5923   | 26.1800   |
| GPT-3.5 Turbo   | Chain of Thought | BEnQA Dataset (12th-math-2.csv)   | 0.2583    | 0.0542    | 0.0440  | 0.0465   | 0.6107   | 26.7331   |
| GPT-3.5 Turbo   | Zero Shot        | BEnQA Dataset (12th-physics-1.csv) | 0.2434| 0.1616| 0.1627| 0.1572   | 0.6654   | 27.2699   |
| GPT-3.5 Turbo   | Three Shot       | BEnQA Dataset (12th-physics-1.csv) | 0.2796| 0.1742    | 0.1693  | 0.1662   | 0.6379   | 25.9657   |
| GPT-3.5 Turbo   | Chain of Thought | BEnQA Dataset (12th-physics-1.csv) | 0.3553| 0.1813    | 0.1682  | 0.1716   | 0.6657| 23.2387 |
| GPT-3.5 Turbo   | Zero Shot        | BEnQA Dataset (12th-physics-2.csv) | 0.2192    | 0.1195    | 0.1122  | 0.1122   | 0.6134   | 28.1422   |
| GPT-3.5 Turbo   | Three Shot       | BEnQA Dataset (12th-physics-2.csv) | 0.2793| 0.1428| 0.1464| 0.1414   | 0.6198   | 25.9774   |
| GPT-3.5 Turbo   | Chain of Thought | BEnQA Dataset (12th-physics-2.csv) | 0.2613    | 0.1244    | 0.1229  | 0.1226   | 0.6200   | 26.6268   |
| GPT-4o          | Zero Shot        | BEnQA Dataset (8th-Science.csv) | 0.6886| 0.5347| 0.5331| 0.5291| 0.8421| 11.2241 |
| GPT-4o          | Three Shot       | BEnQA Dataset (8th-Science.csv) | **0.7325**| 0.5836| 0.5742| 0.5751| **0.8613**| **9.6433**  |
| GPT-4o          | Chain of Thought | BEnQA Dataset (8th-Science.csv) | 0.6842| 0.5519| 0.5534| 0.5495| 0.8534| 11.3822    |
| GPT-4o          | Zero Shot        | BEnQA Dataset (12th-math-1.csv) | 0.5126    | 0.3049    | 0.2949  | 0.2937   | 0.6808   | 17.5667    |
| GPT-4o          | Three Shot       | BEnQA Dataset (12th-math-1.csv) | 0.5404| 0.5416| 0.5048| 0.5135| 0.7791| 16.5655 |
| GPT-4o          | Chain of Thought | BEnQA Dataset (12th-math-1.csv) | 0.4747    | 0.3592| 0.3586  | 0.3447   | 0.7520   | 18.9320    |
| GPT-4o          | Zero Shot        | BEnQA Dataset (12th-math-2.csv) | 0.4757    | 0.6128| **0.6165**| 0.6025| 0.8301| 18.8976    |
| GPT-4o          | Three Shot       | BEnQA Dataset (12th-math-2.csv) | 0.4783    | 0.5092    | 0.4881  | 0.4907   | 0.7942   | 18.8054    |
| GPT-4o          | Chain of Thought | BEnQA Dataset (12th-math-2.csv) | 0.4348    | 0.2804    | 0.2470  | 0.2500   | 0.6961   | 20.3725    |
| GPT-4o          | Zero Shot        | BEnQA Dataset (12th-physics-1.csv)| 0.6776| 0.6199| 0.6159| 0.6157| **0.8745**| 11.6193 |
| GPT-4o          | Three Shot       | BEnQA Dataset (12th-physics-1.csv)| **0.7007**| **0.7144**| **0.7110**| **0.7103**| **0.9064**| **10.7894** |
| GPT-4o          | Chain of Thought | BEnQA Dataset (12th-physics-1.csv)| 0.6711    | 0.6422| 0.6299  | 0.6332   | 0.8863| 11.8565    |
| GPT-4o          | Zero Shot        | BEnQA Dataset (12th-physics-2.csv)| 0.6847| **0.6615**| **0.6548**| **0.6556**| 0.8881| 11.3651 |
| GPT-4o          | Three Shot       | BEnQA Dataset (12th-physics-2.csv)| **0.6937**| 0.6323    | 0.6291  | 0.6283   | 0.8780   | **11.0404** |
| GPT-4o          | Chain of Thought | BEnQA Dataset (12th-physics-2.csv)| 0.6727    | **0.6570**| 0.6493  | **0.6476**   | 0.8875| 11.7981    |
| gemini-1.5-flash  | Three Shot       | BEnQA Dataset (8th-science.csv)  | 0.5399   | 0.3867    | 0.3771 | 0.3763   | 0.7687  | 16.5835  |
| gemini-1.5-flash  | Chain of Thought | BEnQA Dataset (8th-science.csv)  | 0.5025   | 0.3578    | 0.3548 | 0.3524   | 0.7462  | 17.9313  |
| gemini-1.5-flash  | Three Shot       | BEnQA Dataset (12th-math-1.csv)  | 0.5058   | 0.4393    | 0.3804 | 0.3788   | 0.7161  | 17.8110  |
| gemini-1.5-flash  | Chain of Thought | BEnQA Dataset (12th-math-1.csv)  | 0.5263   | 0.2173    | 0.1875 | 0.1976   | 0.7648  | 17.0733  |
| gemini-1.5-flash  | Three Shot       | BEnQA Dataset (12th-math-2.csv)  | 0.4624   | 0.4014    | 0.3433 | 0.3529   | 0.7239  | 19.3761  |
| gemini-1.5-flash  | Chain of Thought | BEnQA Dataset (12th-math-2.csv)  | 0.4414   | 0.1947    | 0.1854 | 0.1886   | 0.7479  | 20.1355  |
| gemini-1.5-flash  | Three Shot       | BEnQA Dataset (12th-physics-1.csv) | 0.6008   | 0.5421    | 0.5374 | 0.5343   | 0.8348  | 14.3901  |
| gemini-1.5-flash  | Chain of Thought | BEnQA Dataset (12th-physics-1.csv) | 0.5785   | 0.3671    | 0.3595 | 0.3621   | 0.7813  | 15.1908  |
| gemini-1.5-flash  | Three Shot       | BEnQA Dataset (12th-physics-2.csv) | 0.5676   | 0.4426    | 0.4435 | 0.4400   | 0.7962  | 15.5864  |
| gemini-1.5-flash  | Chain of Thought | BEnQA Dataset (12th-physics-2.csv) | 0.5192   | 0.3817    | 0.3820 | 0.3796   | 0.7692  | 17.3311  |
| Aya 101    | Zero Shot       | BEnQA Dataset (8th-Science.csv)  | 0.0307   | 0.0009    | 0.0076  | 0.0012   | 0.5007  | 34.9370  |
| Aya 101    | Three Shot      | BEnQA Dataset (8th-Science.csv)  | 0.0833   | 0.0461    | 0.0498  | 0.0454   | 0.5312  | 33.0400  |
| Aya 101    | Chain of Thought| BEnQA Dataset (8th-Science.csv)  | 0.1009   | 0.0565    | 0.0631  | 0.0570   | 0.5411  | 32.4077  |
| Aya 101    | Zero Shot       | BEnQA Dataset (12th-Math-1.csv)  | 0.1995   | 0.0545    | 0.0580  | 0.0295   | 0.5015  | 28.8531  |
| Aya 101    | Three Shot      | BEnQA Dataset (12th-Math-1.csv)  | 0.2172   | 0.1660    | 0.2002  | 0.1573   | 0.5847  | 28.2160  |
| Aya 101    | Chain of Thought| BEnQA Dataset (12th-Math-1.csv)  | 0.2172   | 0.0454    | 0.0865  | 0.0557   | 0.5843  | 28.2160  |
| Aya 101    | Zero Shot       | BEnQA Dataset (12th-Math-2.csv)  | 0.1790   | 0.0452    | 0.0340  | 0.0182   | 0.5013  | 29.5908  |
| Aya 101    | Three Shot      | BEnQA Dataset (12th-Math-2.csv)  | 0.2276   | 0.0877    | 0.0992  | 0.0833   | 0.5517  | 27.8393  |
| Aya 101    | Chain of Thought| BEnQA Dataset (12th-Math-2.csv)  | 0.1765   | 0.0117    | 0.0231  | 0.0145   | 0.5235  | 29.6830  |
| Aya 101    | Zero Shot       | BEnQA Dataset (12th-Physics-1.csv)| 0.1382  | 0.0053    | 0.0104  | 0.0055   | 0.5000  | 31.0639  |
| Aya 101    | Three Shot      | BEnQA Dataset (12th-Physics-1.csv)| 0.1908  | 0.0807    | 0.0757  | 0.0735   | 0.5473  | 29.1669  |
| Aya 101    | Chain of Thought| BEnQA Dataset (12th-Physics-1.csv)| 0.1645  | 0.0334    | 0.0444  | 0.0361   | 0.5305  | 30.1154  |
| Aya 101    | Zero Shot       | BEnQA Dataset (12th-Physics-2.csv)| 0.1261  | 0.0017    | 0.0085  | 0.0028   | 0.5004  | 31.4976  |
| Aya 101    | Three Shot      | BEnQA Dataset (12th-Physics-2.csv)| 0.1802  | 0.0597    | 0.0571  | 0.0528   | 0.5328  | 29.5493  |
| Aya 101    | Chain of Thought| BEnQA Dataset (12th-Physics-2.csv)| 0.1682  | 0.0292    | 0.0371  | 0.0286   | 0.5208  | 29.9823  |
