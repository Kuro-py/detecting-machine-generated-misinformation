# Detecting Machine-Generated Misinformation in Social Media

#BibTeX

@mastersthesis{gharat2025mgm,
  author       = {Gharat, Manthan},
  title        = {Detecting Machine-Generated Misinformation in Social Media},
  school       = {University of Sheffield},
  year         = {2025},
  type         = {MSc Dissertation},
  note         = {Supervised by Carolina Scarton and Fatima Haouari},
  url          = {https://github.com/Kuro-py/detecting-machine-generated-misinformation}
}


## MSc Dissertation Project

**Author:** Manthan Gharat  
**Degree:** MSc Computer Science  
**Supervisors:** Dr. Carolina Scarton, Dr. Fatima Haouari  
**Institution:** University of Sheffield  
**Year:** 2025  

---

## Abstract

With the increasing accessibility of large language models (LLMs), the generation of machine-written content on social media platforms has grown significantly, raising concerns around the spread of machine-generated misinformation (MGM). This dissertation investigates the characteristics of LLM-generated paraphrased misinformation tweets and evaluates the effectiveness of existing detection methods.  

The work introduces newly curated machine-generated misinformation datasets, evaluates state-of-the-art long-form detectors and fine-tuned LLMs on short-form social media text, and performs detailed error analysis to understand model failure patterns.

---

## Research Questions

- **RQ1:** How similar are LLM-generated paraphrased tweets to human-written tweets?
- **RQ2:** Can existing long-form machine-generated text (MGT) detectors effectively identify machine-generated misinformation tweets?
- **RQ3:** How does fine-tuning state-of-the-art LLMs affect performance in detecting machine-generated misinformation?
- **RQ4:** What are the main failure patterns observed in machine-generated misinformation detection?

---

## Methodology

### Dataset Creation
- Curated **8 misinformation datasets**.
- Tweets were paraphrased using **three state-of-the-art LLMs**.
- Generated tweets were cleaned, labelled, and validated.
- Final dataset size: **~50,000 tweets**.

### Generated Data Analysis
Similarity between human-written and LLM-paraphrased tweets was evaluated using:
- **Jaccard Score**
- **BERTScore**
- **METEOR Score**

### Detection Models
The following categories of models were evaluated:
- Pretrained long-form MGT detectors
- Open-source large language models
- Encoder-based classification models
- Statistical models

### Evaluation Metrics
Detection performance was measured using:
- Youden Macro F1
- Macro F1
- Macro F1 @ 0.05 False Positive Rate
- True Positive Rate @ 0.01 False Positive Rate
- Overlap (OVL) Score

---

## Conclusion

- LLM-generated paraphrased tweets can closely resemble human-written tweets while maintaining semantic consistency.
- Existing long-form MGT detectors struggle with short-form misinformation detection.
- Fine-tuning LLMs on domain-specific tweet data significantly improves detection performance. Fine-tuned **Llama-3.2 3B** achieved the strongest results across all datasets.
- Certain linguistic and stylistic features remain challenging for even the best-performing models.

---
