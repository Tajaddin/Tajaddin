# Tajaddin Gafarov

M.S. student in Computer Science at the University of South Florida, expected May 2027. B.S. in Computer Science, USF, 2025.

[LinkedIn](https://www.linkedin.com/in/tajaddin-gafarov) · gafarovtajaddin@gmail.com

## Research interests

Human-computer interaction and human-centered AI. I want to understand how people decide when to trust an AI answer and when to check it.

- Interfaces showing sources, confidence, and uncertainty, so users verify model answers instead of accepting them.
- Calibrated model confidence, and how it changes what people do with an answer.
- Evaluating LLM systems with human judgment alongside automated metrics.

Coursework: Human-Computer Interaction (in progress), Introduction to Large Language Models, Deep Learning, Introduction to AI.

## Selected work

- **[lte-reproducibility](https://github.com/Tajaddin/lte-reproducibility)**: reproduction of Jiang et al., "Learning to Edit: Aligning LLMs with Knowledge Editing" (ACL 2024), with Marvin Osei-Kuffour for CAI 5335, Spring 2026. We trained LTE-LoRA on LLaMA-2-Chat-7B for one epoch on one Colab A100, against the paper's three epochs. Edit success reached 90.3% on WikiData counterfact and 65.4% on ZsRE, against 99.9% for both in the paper. The report documents the gaps, seven patches needed to run the released code, and an in-context editing extension to LLaMA-3-8B.
- **[langgraph-research-pilot](https://github.com/Tajaddin/langgraph-research-pilot)**: question-answering agent over Wikipedia. Each answer cites its sources, the agent pauses at two human review gates, and it answers "unknown" when retrieved sources do not support a claim. On 30 HotpotQA questions with Claude Haiku 4.5, exact match tied a single-prompt baseline at 23.3%, F1 rose from 0.313 to 0.368, and the agent abstained on 11 of 30.
- **[conf-calib](https://github.com/Tajaddin/conf-calib)**: calibration for the confidence an LLM states in words. Llama-3.1-8B reported 100% confidence on about 91% of BoolQ questions while 84% accurate. On 300 held-out questions, isotonic regression cut expected calibration error from 0.148 to 0.030 with no change in accuracy.
- **[streaming-chat-ui](https://github.com/Tajaddin/streaming-chat-ui)**: React chat interface with footnote-style source citations, stop, regenerate, and message editing, built from small tested modules.
- **[fake-news-detector-ml](https://github.com/Tajaddin/fake-news-detector-ml)**: graduate ML course project. A six-step data audit traced a 99 to 100% accuracy baseline on the ISOT corpus to publisher and stylistic leakage. On the LIAR held-out test set (1,267 statements), the result is 62.1% accuracy and 0.676 ROC-AUC.

## Background

Since 2021 I have worked part-time and remotely on ML and data systems for two companies, alongside full-time study. Most other repositories here are engineering projects: backend services, data pipelines, and LLM tooling.
