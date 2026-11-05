# Hi, I'm Gulnar Hasanova

**Data analyst and machine-learning engineer in progress.**
I build small, complete projects — and then measure them instead of claiming they work.

Most of my repositories end with a report: a metric table, an error analysis, or a
list of limitations. That is deliberate. A model that fails 40% of negated
sentences is more useful to write down than a model that "works well".

- 🔭 Currently: evaluating fine-tuned LLMs (QLoRA on Qwen2.5) and dataset quality for computer vision
- 🧪 Interested in: evaluation, error analysis, retrieval, and anything that runs locally
- 🌍 Based in Azerbaijan · writing code and reports in English, tutoring content in Azerbaijani
- 📫 Reach me: **[your email]** · **[your LinkedIn]**

---

## Selected work

| Project | What it does | Stack | Result |
|---|---|---|---|
| **[Data Collection Quality Ablation](https://github.com/HasanovaGulnar/data-collection-quality-ablation)** | Two YOLO detectors with identical architecture and hyperparameters — only the dataset changes (300 images / 4 sessions vs 800 / 15+ sessions) | Python, YOLOv8, OpenCV | Diversity beat size on a clip from conditions in neither training set |
| **[Negation & Sarcasm Stress Test](https://github.com/HasanovaGulnar/negation-sarcasm-stress-test)** | 15 hand-written sentences that break sentiment models in specific, explainable ways | Python, scikit-learn, Transformers | TF-IDF 40% failure · BERT 46.7% · transformer fails every sarcasm case |
| **[Base vs Fine-Tuned Panel](https://github.com/HasanovaGulnar/base-vs-finetuned-panel)** | One prompt, two variants of the same model, side-by-side answers with measured latency | Transformers, PEFT/QLoRA, Streamlit | Adapter: +0.17 s load, +10.4% latency; quality mixed, documented per prompt |
| **[ReviewPulse](https://github.com/HasanovaGulnar/reviewpulse-ai-sentiment-analysis)** | Sentiment app for small sellers: one review or a CSV batch, with confidence and a batch summary | scikit-learn, Streamlit, pandas | Capstone — classical NLP delivered as a usable product |
| **[Local Research Agent](https://github.com/HasanovaGulnar/research-agent)** | Plans, calls tools through Ollama's native tool API, and cites only evidence it actually retrieved | Python, Ollama, JSONL traces | Fake citations invalidate the run; every step is inspectable |
| **[License Plate Recognition](https://github.com/HasanovaGulnar/plate-recognition)** | Detect → crop → OCR pipeline with an honest end-to-end evaluation | YOLOv8, Tesseract, OpenCV | mIoU 0.888 · recall 100% · exact match 15% (3/20) |

---

## Projects by area

### Computer vision

**[Pen/Pencil Webcam Detector](https://github.com/HasanovaGulnar/pen-pencil-detector)** — fine-tuned YOLOv8n for one custom class, live webcam overlay with FPS.
`Python` `Ultralytics YOLOv8` `OpenCV`

**[CNNs & Image Classification](https://github.com/HasanovaGulnar/CNNs-and-Image-Classification)** — a CNN trained from scratch against an MLP, same seed and schedule, plus five hand-drawn digits as a reality check.
`PyTorch` `CNN` `MNIST` — CNN 98.73% vs MLP 97.36%

**[Object Detection & Tracking](https://github.com/HasanovaGulnar/CodeAlpha_ObjectDetectionTracking)** — webcam/video input, YOLOv8n detections, ByteTrack IDs.
`Python` `YOLOv8` `ByteTrack` `OpenCV` — CodeAlpha AI internship, Task 4

### NLP & LLMs

**[Qwen Python Tutor](https://github.com/HasanovaGulnar/qwen-local-assistant)** — local Azerbaijani Python tutor built on a 4-bit QLoRA adapter over Qwen2.5-1.5B-Instruct.
`Transformers` `PEFT` `QLoRA` `Streamlit` — 72-example dataset, r=4, adapter 2.09 MB

**[Retrieval-Augmented Generation](https://github.com/HasanovaGulnar/Retrieval-Augmented-Generation)** — from-scratch RAG over a real AzTU examination-regulations PDF, no framework.
`multilingual-e5-small` `FAISS` `Cross-encoder reranking` `Ollama`

**[Product Review Sentiment](https://github.com/HasanovaGulnar/product-review-sentiment)** — classical TF-IDF baseline vs a pretrained transformer on the same saved Yelp split.
`scikit-learn` `BERT` `pandas` — identical reviews, labels and test set for both

**[FAQ Chatbot](https://github.com/HasanovaGulnar/CodeAlpha_FAQChatbot)** — TF-IDF + cosine similarity over a 12-question FAQ, with stemming and a fallback threshold.
`NLTK` `scikit-learn` `Streamlit` — CodeAlpha AI internship, Task 2

**[Language Translation Tool](https://github.com/HasanovaGulnar/CodeAlpha_LanguageTranslationTool)** — Streamlit translator with input, size and language validation.
`Streamlit` `REST API` — CodeAlpha AI internship, Task 1

**[Music Generation](https://github.com/HasanovaGulnar/CodeAlpha_MusicGeneration)** — LSTM/Transformer MIDI generation with audio rendering.
`PyTorch` `MIDI` `SoundFont` — CodeAlpha AI internship

### Data analysis & statistics

**[Actuarial Claims Reserving](https://github.com/HasanovaGulnar/actuarial-reserving)** — Chain Ladder reserving with loss development factors and a tail factor, written up with formulas.
`Python` `pandas` `SQL` — estimated unpaid reserve 392,974.60 AZN (synthetic data)

**[Bank Marketing Campaign Analysis](https://github.com/HasanovaGulnar/bank-marketing-campaign-analysis)** — chi-square testing and logistic regression on a bank's campaign data.
`R` `Logistic Regression` `R Markdown`

**[Retail Sales Analysis](https://github.com/HasanovaGulnar/retail-sales-analysis-r)** — cleaning, EDA, anomaly detection and visualisation of Azerbaijani retail data.
`R` `dplyr` `ggplot2` — Code Academy Data Analytics

**[EDA & Data Visualization](https://github.com/HasanovaGulnar/EDA-Data-Visualization)** — reusable exploratory workflow: missing values, outliers, correlations, hypotheses.
`pandas` `NumPy` `Matplotlib` `Seaborn` `SciPy`

### Automation

**[AI Customer Support Ticket Bot](https://github.com/HasanovaGulnar/ai-customer-support-ticket-bot)** — n8n workflow that classifies tickets with an AI node and logs them to Google Sheets.
`n8n` `AI agent` `Google Sheets`

**[Telegram Support Bot](https://github.com/HasanovaGulnar/customer-support-ticket-bot-n8n)** — n8n workflow that turns Telegram messages into support tickets.
`n8n` `Telegram` `Automation`

---

## How I work

1. **Fix the comparison.** Same data, same seed, same hyperparameters — change one thing.
2. **Measure the failure.** A metric table beats an adjective; error analysis beats a demo.
3. **Write the limitations.** Every README has a section about what the project does not prove.
4. **Keep it local.** Most projects run offline on a laptop, with no paid API in the loop.

---

## Toolbox

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)

---

## Programs

- **CodeAlpha AI internship** — four tasks: translation tool, FAQ chatbot, object detection & tracking, music generation
- **Code Academy — Data Analytics** — R retail-sales analysis and reporting
- **Course projects** — weekly builds in computer vision, NLP, RAG and agentic systems, each closed with an evaluation report
