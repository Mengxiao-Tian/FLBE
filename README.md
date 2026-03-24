# Knowledge-Guided Interpretable Livestock Behavior Analysis with Retrieval-Augmented Reasoning

---

## 🧩 Key Ideas

Our framework is built upon three key components:

### 1. Fine-grained Behavior Ethogram

* Constructed using domain knowledge (e.g., Wikipedia + multimodal models)
* Each behavior includes:

  * Definition
  * Context cues
  * Visual anchors
  * Negative delimiters

### 2. Explanation-enhanced Supervision

* Automatically generate natural language explanations
* Train models to produce interpretable reasoning

### 3. Retrieval-Augmented Reasoning

* Dynamically retrieve relevant behavior knowledge
* Inject into model prompts for improved reasoning

---

## 📊 FLBE Dataset

We introduce the **Fine-grained Livestock Behavior Explanation (FLBE)** dataset, the first large-scale benchmark with explanation annotations.

| Dataset      |     #Images | #Actions | Source         | Scenario      | Labels | Long-tail | Explanation |
| ------------ | ----------: | -------: | -------------- | ------------- | ------ | --------- | ----------- |
| FLBE-Pig     |      55,165 |        6 | Web + Industry | Pen / Cage    | Multi  | ✓         | ✓           |
| FLBE-Cow     |      62,424 |        7 | Surveillance   | Day & Night   | Multi  | ✓         | ✓           |
| FLBE-Sheep   |      14,455 |        5 | Grazing        | Outdoor       | Multi  | ✓         | ✓           |
| FLBE-Chicken |      35,234 |        7 | Web            | Poultry House | Multi  | ✓         | ✓           |
| **Total**    | **167,278** |        — | Mixed          | Diverse       | Multi  | ✓         | ✓           |

---

## 📊 Explanation Quality

| Model | Pig (NLI) | Pig (GPT) | Chicken (NLI) | Chicken (GPT) | Sheep (NLI) | Sheep (GPT) | Cow (NLI) | Cow (GPT) |
|------|----------|----------|--------------|--------------|------------|------------|----------|----------|
| GPT-5 | 50.83 | 33.75 | 30.92 | 19.66 | 39.62 | 32.34 | 39.79 | 39.22 |
| Gemini 3.0 Pro | 50.78 | 38.10 | 28.93 | 27.09 | 30.57 | 24.60 | 33.56 | 43.80 |
| Qwen2.5-VL-3B | 44.36 | 24.45 | 28.15 | 15.71 | 33.86 | 21.81 | 32.70 | 21.57 |
| + Ours | 50.81 | 40.36 | 36.67 | 30.34 | 45.02 | 75.72 | 39.87 | 46.10 |
| Qwen3-VL-2B | 49.01 | 32.27 | 32.38 | 21.18 | 39.02 | 22.05 | 38.63 | 29.06 |
| + Ours | 51.56 | 41.42 | 37.42 | 31.38 | 46.12 | 77.11 | 41.02 | 47.52 |
| LLaVA-1.5-7B | 47.20 | 27.80 | 5.52 | 11.71 | 20.60 | 19.35 | 19.49 | 16.73 |
| + Ours | 53.55 | 35.73 | 30.71 | 24.80 | 42.57 | 57.91 | 37.03 | 41.88 |
| InternVL3-2B | 42.20 | 22.12 | 21.87 | 13.78 | 30.60 | 20.28 | 32.49 | 22.83 |
| + Ours | 49.58 | 36.91 | 34.72 | 28.94 | 44.36 | 74.85 | 38.94 | 45.67 |

---

## 🎯 Qualitative Results

![Qualitative](figs/qualitative.png)

Compared to baseline models, our method generates:

* More accurate behavior predictions
* More coherent and grounded explanations
* Less hallucination

---

## 🏆 Contributions

* Introduce interpretable livestock behavior analysis framework
* Propose retrieval-augmented reasoning for VLMs
* Construct the FLBE dataset with explanation annotations

---

## 📄 Paper

📎 [PDF Link Coming Soon]

---

## 📌 Citation

```bibtex
@article{yourname2025livestock,
  title={Knowledge-Guided Interpretable Livestock Behavior Analysis with Retrieval-Augmented Reasoning},
  author={...},
  journal={...},
  year={2025}
}
```

---

## ⭐ Acknowledgement

This project aims to advance **interpretable AI for precision livestock farming**.
