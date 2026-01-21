# Urdu Datasets & Engineering Resources

A comprehensive registry of **Urdu datasets, models, and tools** designed for the urdu NLP and Large Language Models (LLM) development. Resources are taxonomized by use case, from **Pre-training** (CLM) and **Supervised Fine-tuning** (SFT/Instruction Tuning) to **Evaluation** and **Inference**.
This repository aims to standardize the data landscape for Urdu as a low-to-mid resource language.

---

- [LLM Datasets](#llm-datasets)
  - [Pre-training Corpora](#pre-training-corpora)
---

# LLM Datasets


## Pre-training Corpora 
**Task Description:** Raw, unlabeled text used for **Causal Language Modeling (CLM)**. These datasets are essential for the foundational training phase to teach the model grammar, world knowledge, and vocabulary via next-token prediction.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [Urdu Rekhta](https://huggingface.co/datasets/mahwizzzz/Urdu_Rekhta) | Mahwiz Khalil | 2025 | Literary Domain including Structured poetry metadata and rhymes. |
| [Rekhta Ghazals](https://github.com/amir9ume/urdu_ghazals_rekhta) | Rekhta Community | 2020 |  High-quality literary text for Domain Adaptation |
| [Maḵẖzan](https://github.com/zeerakahmed/makhzan) | Zeerak Ahmed | 2020 | Classical Urdu Data for Pre-training |
| [UFAL Urdu Corpus](https://lindat.mff.cuni.cz/repository/xmlui/handle/11858/00-097C-0000-0023-65A9-5) | UFAL | 2014 | 5.4M sentences with linguistic morphology tags. |
| [Urdu Wikipedia Dumps](https://dumps.wikimedia.org/urwiki/) | Wikimedia | Ongoing |High-factuality encyclopedic text for Knowledge Base Injection |
| [iNLTK Wiki Articles](https://www.kaggle.com/disisbig/urdu-wikipedia-articles) | iNLTK | 2020 | Cleaned Knowledge Data |
| [PK Multilang](https://huggingface.co/datasets/mahwizzzz/pak-cleaned-multilang-2025) | Mahwiz Khalil | 2025 | Multingual Data |
| [OSCAR Corpus (Urdu)](https://oscar-project.github.io/documentation/versions/oscar-2301/) | Ortiz Suárez et al. | 2020 | High-quality Web CLM |
| [CC-100 (Urdu)](http://data.statmt.org/cc-100/) | Facebook AI | 2019 | Massive Web Crawl (CommonCrawl) |
| [WMT Raw](http://data.statmt.org/ngrams/raw/) | WMT | 2017 | Web Text useful for robustness training. |
| [Leipzig Corpora](https://wortschatz.uni-leipzig.de/en/download/urd) | Univ. Leipzig | — | Curated Monolingual Text  |
| [Urdu Quotes](https://huggingface.co/datasets/mahwizzzz/UrduQuotes) | Mahwiz Khalil | 2023 |Aphorisms and proverbs for semantic understanding.


---

## 2. Instruction Tuning 
**Task Description:** Complex prompt-response pairs and semantic clusters. Used for **Instruction Tuning ** to improve reasoning and instruction following  capabilities.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [Urdu Chat Alpaca](https://huggingface.co/datasets/large-traversaal/urdu_chat_alpaca) | Traversaal.ai | 2025 |Synthetic/Distilled data of52k Alpaca samples translated for general instruction following. |
| [Urdu Instruct](https://huggingface.co/datasets/large-traversaal/urdu-instruct) | Traversaal.ai | 2025 | Diverse prompts for broad capability alignment. |
| [GSM8K Urdu](https://huggingface.co/datasets/large-traversaal/gsm8k_urdu) | Traversaal.ai | 2025 | Grade-school math problems for logic/reasoning. |
| [Urdu Assistant](https://huggingface.co/datasets/mahwizzzz/UrduAssistant) | Mahwiz Khalil | 2023 | Dialogue-focused structure for conversational agents and Supervised Dialogue Training. |
| [Dolly Urdu](https://huggingface.co/datasets/aaqibsaeed/databricks-dolly-15k-ur) | Aaqib Saeed | 2023 |Open-ended QA/Brainstorming data useful for Instruction Tuning. |
| [Urdu Alpaca Filtered](https://huggingface.co/datasets/mahwizzzz/urdu_alpaca_yc_filtered) | Mahwiz Khalil | 2025 | Filtered version of Alpaca to remove translation hallucinations. |
| [Urdu Alpaca](https://huggingface.co/datasets/ravithejads/alpaca_urdu) | Ravi Theja | 2024 | Standard machine-translated Alpaca dataset. |
| [Urdu Legal](https://huggingface.co/datasets/mahwizzzz/UrduLegal) | Mahwiz Khalil | 2024 | Legal QA pairs for specialized fine-tuning. |
| [UQuAD](https://github.com/ahsanfarooqui/UQuAD---Urdu-Question-Answer-Dataset/tree/main) | Ahsan Farooqi | - | SQuAD-style (Context → Question → Answer). Ideal for RAG. |
| [QA](https://github.com/mirfan899/Urdu/tree/master/qa) | Muhammad Irfan | - | Simple fact-retrieval pairs. |
| [UQA](https://huggingface.co/datasets/uqa/UQA) | Samee Arif | 2024 | Open-domain question answering. |
| [Urdu Q-A](https://github.com/nabeelDanish/Urdu-Q-A-System) | Nabeel Danish | 2024 |Dataset built for retrieval systems. |
| [Wiki- UQA](https://huggingface.co/datasets/uqa/Wiki-UQA) | Samee Arif | 2024 | Wikipedia-grounded QA pairs for RAG/Context. |

---

## 3. Task Specific Fine-tuning

### A. Sequence Classification & Alignment
**Task Description:** Labeled data for **Sequence Classification**. These datasets are critical for training **Reward Models (RM)** in RLHF pipelines or building specialized classifiers for sentiment and safety (guardrails).

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [Urdu IMDb Reviews](https://www.kaggle.com/akkefa/imdb-dataset-of-50k-movie-translated-urdu-reviews) | Kaggle Contributors | — | Sentiment Analysis / RLHF |
| [Urdu Sentiment Benchmark](https://github.com/MuhammadYaseenKhan/Urdu-Sentiment-Corpus) | M. Yaseen Khan | 2020 | Binary Classification |
| [Roman Urdu Dataset](https://github.com/Smat26/Roman-Urdu-Dataset) | Smat26 | — | Roman-script Sentiment |
| [Urdu Financial Phrasebank ](https://huggingface.co/datasets/mahwizzzz/ur_financial_phrasebank) | Mahwiz Khalil | 2023 | Sentiment Classification (Financial Domain |
| [UCI Roman-Urdu Sentiment](https://archive.ics.uci.edu/ml/datasets/Roman+Urdu+Data+Set) | UCI ML Repo | 2018 | Noisy Text Classification |
| [Hate Speech Detection](https://github.com/haroonshakeel/roman_urdu_hate_speech) | Haroon Shakeel | 2020 | Toxicity Detection / Safety |
| [Awesome Urdu]( https://github.com/urduhack/awesome-urdu/tree/master) | Ikram Ali | 2019 | Differnet Urdu NLP and NLU Datasets |
                     
                                                                                                                                                    
### B. Token Classification (POS, NER)
**Task Description:** Text with token-level annotations. Used for **Token Classification** tasks to extract structured entities (NER) or understand syntactic roles (POS), improving the model's information extraction capabilities.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [Urdu NLP Collection](https://github.com/mirfan899/Urdu) | Mirfan | — | General Token Classification |
| [Urdu UD Treebank](https://github.com/UniversalDependencies/UD_Urdu-UDTB) | Universal Dependencies | — | Syntactic Parsing / Dependency |
| [MK-PUCIT NER](https://www.kaggle.com/safiakanwal/mkpucit-ner-dataet) | PUCIT | 2019 | Named Entity Recognition |
| [WikiAnn (Urdu)](https://elisa-ie.github.io/wikiann/) | Pan et al. | 2017 | Cross-lingual NER Transfer |
| [Urdu Word Segmentation](https://github.com/harisbinzia/Urdu-Word-Segmentation) | Haris Bin Zia | 2018 | Tokenizer Optimization / CRF |


### c. Semantic Tasks (Summarization, Data Augmentation)
**Task Description:** Paired or unpaired text data used for semantic generation tasks. The model learns to map source text to a semantically faithful target text (summaries or augmented variants), focusing on meaning preservation, abstraction, and contextual coherence rather than token-level labeling.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [UrduSummary Corpus](https://github.com/humsha/USCorpus) | Humsha et al. | 2016 | Abstractive Summarization |
| [Text Generation](https://huggingface.co/datasets/mahwizzzz/dumm) | Mahwiz Khalil | 2025 | Text Generation |
| [Urdu Paraphrase Corpus](http://ucrel.lancs.ac.uk/textreuse/uppc.php) | UCREL | 2016 | Paraphrase Detection |
| [Urdu Short Text Reuse](http://ucrel.lancs.ac.uk/textreuse/ustrc.php) | UCREL | 2018 | Semantic Similarity (STS) |
| [TaPaCo](https://zenodo.org/record/3707949) | Scherrer et al. | 2020 | Data Augmentation / Paraphrasing |
| [ursum](https://huggingface.co/datasets/mahwizzzz/ursum) | Mahwiz Khalil | 2023 | Urdu SUmmarization |

---


## 4. Evaluation & Analysis Benchmarks
**Task Description:** Standardized test sets for **Zero-shot and Few-shot Evaluation**. These datasets must be excluded from training data to prevent contamination and ensure valid performance metrics.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [OpenbookQA Urdu](https://huggingface.co/datasets/large-traversaal/openbookqa_urdu_cleaned) | Traversaal.ai | 2025 | OpenBookQA Benchmark Translation  |
| [Math500 Urdu ](https://huggingface.co/datasets/large-traversaal/math500_urdu_cleaned) | Traversaal.ai | 2025 | Math500 Benchmark Translation |
| [CommonSenseQA Urdu](https://huggingface.co/datasets/large-traversaal/commonsenseqa_urdu_cleaned) | Traversaal.ai | 2025 | CommonsenseQA Benchmark Translation  |
| [MGSM Urdu](https://huggingface.co/datasets/large-traversaal/mgsm_urdu_cleaned) | Traversaal.ai | 2025 | MGSM Benchmark Translation  |
| [Urdu Error Correction](https://huggingface.co/datasets/mahwizzzz/urdu_error_correction) | Mahwiz Khalil | 2025 |Error Detection & Correction |

---

## 5. Multimodal (Vision–Language)
**Task Description:** Image-Text pairs used for **Visual Language Modeling (VLM)**. Enables the model to perform image captioning, visual reasoning, and multimodal alignment.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [Flickr8k Urdu Captions](https://github.com/abdullahzia510/Effecient-Urdu-Caption-Generation-using-Attention-Mechanism) | Abdullah Zia | 2020 | Image-to-Text Generation |
| [CLE Urdu Image Corpora](https://www.cle.org.pk/clestore/imagecorpora.htm) | CLE Pakistan | — | OCR / Visual Grounding |

---

## 6. OCR & Text Recognition
**Task Description:** Images of text paired with transcriptions. Used to train **Optical Character Recognition (OCR)** encoders or to fine-tune multimodal models on the Nastaliq script.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [Qaida](https://github.com/AtiqueUrRehman/qaida) | Atique ur Rehman | — | Synthetic Data Generation |
| [U-HAT](https://www.kaggle.com/hazrat/uhat-urdu-handwritten-text-dataset) | Hazrat | — | Handwritten Text Recognition |
| [45K Urdu Ligatures](https://github.com/UltramindSoft/45K-Clean-Background-Urdu-Ligatures-Dataset) | UltramindSoft | 2019 | Ligature Recognition |
| [IIIT-H Urdu OCR](https://cvit.iiit.ac.in/research/projects/cvit-projects/iiit-urdu-ocr) | IIIT Hyderabad | 2017 | Printed Text OCR |
| [Cursive-Text](https://www.sciencedirect.com/science/article/pii/S2352340920306430) | Scene Text Authors | 2020 | Natural Scene Text OCR |

---

## 7. Machine Translation (Seq2Seq)
**Task Description:** Parallel bitexts (English-Urdu). Used for **Sequence-to-Sequence (Seq2Seq)** training to align the Urdu embedding space with high-resource languages like English.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [OPUS Corpora](https://opus.nlpl.eu/) | OPUS Team | — | Massive Parallel Corpus |
| [PM India Corpus](http://data.statmt.org/pmindia/) | WMT | — | Low-resource Alignment |
| [English–Urdu Religious](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-2582) | UFAL | — | Domain Specific Translation |
| [Anuvaad Parallel Corpus](https://github.com/project-anuvaad/anuvaad-parallel-corpus) | Govt. of India | — | Legal/Admin Documentation |
| [CLEU Corpus](http://ucrel.lancs.ac.uk/textreuse/cleu.php) | UCREL | 2018 | Translation & Reuse Detection |

---

## 8. Transliteration & Normalization
**Task Description:** Character-level mappings between scripts. Used for **Text Normalization** pipelines to handle Romanized Urdu input or convert scripts before tokenization.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [Google Dakshina](https://github.com/google-research-datasets/dakshina) | Google Research | 2020 | Script Transliteration |
| [TRANSLIT](https://github.com/fbenites/TRANSLIT) | Benites et al. | 2020 | Named Entity Transliteration |
| [Roman-Urdu Corpus](https://github.com/irshadbhat/roman-urdu-corpus) | Irshad Bhat | 2020 | Roman-to-Nastaliq Mapping |
| [Ur–RomUr–Eng Dict](https://github.com/MoizRauf/Urdu--Roman-Urdu--English--Dictionary) | Moiz Rauf | 2019 | Multi-script Dictionary |

---

## 9. Lexical & Linguistic Resources
**Task Description:** Dictionaries and N-grams. Used for **Tokenizer Training** (BPE/WordPiece), vocabulary expansion, and heuristic data filtering/cleaning.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [Urdu Sentiment Lexicon](https://chaoticity.com/urdu-sentiment-lexicon/) | — | — | Polarity Lookup / Heuristics |
| [UrduHack Word Lists](https://github.com/urduhack/urdu-words) | UrduHack | — | Stopwords / Normalization |
| [CLE Urdu WordNet](https://www.cle.org.pk/clestore/urduwordnet.htm) | CLE Pakistan | — | Semantic Graph / Synsets |
| [IndoWordNet](https://github.com/anoopkunchukuttan/indowordnet_parallel) | IIT Bombay | — | Multilingual WordNet |
| [Urdu N-grams](https://www.kaggle.com/tafseerahmed/urdu-ngrams) | Kaggle | 2020 | Statistical Language Modeling |

---

## 10. Speech & Audio (ASR)
**Task Description:** Audio paired with text transcriptions. Used for training **Automatic Speech Recognition (ASR)** models or fine-tuning Whisper-style models for Urdu.

| Dataset | Authors | Date | Notes |
| :--- | :--- | :--- | :--- |
| [UAT](https://huggingface.co/datasets/mahwizzzz/UAT) | Mahwiz Khalil | 2025 | Urdu Audio and Text |
| [Urdu 250 Isolated Words](https://www.kaggle.com/hazrat/urdu-speech-dataset) | Hazrat | 2018 | Keyword Spotting (KWS) |
| [CLE Phonetic Speech](https://www.cle.org.pk/software/ling_resources/phoneticallyrichurduspeechcorpus.htm) | CLE Pakistan | — | Phonetic Alignment / ASR |
| [CMU Wilderness](http://www.festvox.org/cmu_wilderness/) | CMU | 2019 | Aligned Speech (Bible) |
| [LibriVox Urdu](https://librivox.org/search?primary_key=57&search_category=language&search_page=1&search_form=get_results) | Community | — | Audiobooks (Long-form ASR) |
| [Urdu-Sindhi Emotion](https://zenodo.org/record/3685274) | Researchers | 2020 | Speech Emotion Recognition |


# Tools & Utilities

Essential libraries, models, and resources for building Urdu LLM pipelines.

## 1.Python Libraries 
**Use Case:** NLP, Data cleaning, normalization, and linguistic analysis.

| Tool | Type | Notes |
| :--- | :--- | :--- |
| [UrduHack](https://github.com/urduhack/urduhack) | Library | NLP including Normalization, Tokenization, NER etc. |
| [UrduHack-Lite](https://pypi.org/project/urduhack-lite/) | Library | Lightweight version for low-memory environments. |
| [Stanza](https://stanfordnlp.github.io/stanza/) | Pipeline | High-accuracy dependency parsing and POS tagging. |
| [spaCy](https://spacy.io/usage/models) | Pipeline | Industrial NLP pipeline with community Urdu support. |
| [iNLTK](https://github.com/goru001/inltk) | Toolkit | Data Augmentation and embeddings. |
| [LughaatNLP](https://github.com/Hassan-M-Khan/LughaatNLP) | Library | Lexical processing and stemming. |
| [UNLT](https://github.com/UCREL/UNLT) | Toolkit | UCREL normalization and stemming utilities. |

## 2.Model-Based Utilities (HuggingFace)
**Use Case:** Ready-to-use weights (Adapters/LLMs) to use as baselines or functional tools.

| Collection / Model | Maintainer | Notes |
| :--- | :--- | :--- |
| [Alif-1.0-8B-Instruct](https://huggingface.co/large-traversaal/Alif-1.0-8B-Instruct) | Traversaal.ai | 8B parameter instruction-tuned model (Llama-3 based). Best for semantic tasks. |
| [Mahwizzzz Models](https://huggingface.co/mahwizzzz) | Mahwizzzz | Collection of fine-tuned models for specific Urdu tasks. |
| [UrduHack Models](https://huggingface.co/urduhack) | UrduHack | BERT/RoBERTa encoders optimized for Sentiment and NER. |

## 3.APIs & Online Services
**Use Case:** Benchmarking and OCR/TTS without local deployment.

| Service | Provider | Notes |
| :--- | :--- | :--- |
| [Text Processing](https://tech.cle.org.pk/text_services) | CLE Pakistan | APIs for Text Processing. |
| [Speech Processing](https://tech.cle.org.pk/speech_services) | CLE Pakistan | APIs for speech Processing. |
| [Image Processing](https://tech.cle.org.pk/image_services) | CLE Pakistan | APIs for Image Processing. |
| [Google Translate](https://translate.google.com/) | Google | Translator (Other Language ↔ Urdu). |
| [Matnsaz](https://matnsaz.net/) | Tool | Autocorrecter: Writing assistant for text validation. |

## 4.Input & Typography
**Use Case:** Solving Nastaliq rendering issues and input testing.

| Resource | Category | Notes |
| :--- | :--- | :--- |
| [Urdu Fonts](https://luc.devroye.org/fonts-45771.html) | Fonts | Testing model output rendering (Nastaliq vs Naskh). |
| [Branah Keyboard](https://www.branah.com/urdu) | Input | Virtual keyboard for prompt testing. |
| [Lexilogos](https://www.lexilogos.com/keyboard/urdu.htm) | Input | Phonetic keyboard layout. |
