| Model Name                    | GSM8K(8-shot) | MATh(4-shot) | MMLU-STEM(4-shot) | CMATH(6-shou) | GAOKAO MATH Cloze(5-shot) | GAOKAO MATH QA(4-shot) |
| ----------------------------- | ------------- | ------------ | ----------------- | ------------- | ------------------------- | ---------------------- |
| **Specific Base Model** |               |              |                   |               |                           |                        |
| DeepSeekMath-Base-7B          | 64.2          | 36.2         | 56.5              | 71.7          | 20.3                      | 40.7                   |
| DeepSeekMath-Base-7B-repro    | 62.8          | 32.2         | 55.4              | 58.3(71.7)    | 17.8(24.6)                | 42.5                   |
| Qwen2.5-Math-1.5B             | 76.8          | 49.8         | 51.3              | 83.0          | 47.5                      | 54.1                   |
| Qwen2.5-Math-1.5B-reproduce   | 75.0          | 51.0         | 56.3              | 64.7(80.3)    | 18.6(25.4)                | 55.3                   |
| Qwen2.5-Math-7B               | 91.6          | 55.4         | 67.8              | 85.0          | 57.6                      | 69.5                   |
| Qwen2.5-Math-7B-reproduce     | 85.3          | 58.7         | 71.4              | 73.5(88.7)    | 28.0(36.4)                | 61.3                   |

（）是在shot中引入cot后重测的结果

在GAOKAO MATH Cloze上的准确率出入较大。这个测试集是中文高考数学填空题。与原文出入较大可能是prompt和shot的问题，shot是我从测试集中挑出来几个sample再自己编写rationale，填空题较难，可能受prompt和shot的影响较大。
