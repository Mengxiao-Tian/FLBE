# Knowledge-Guided Interpretable Livestock Behavior Analysis with Retrieval-Augmented Reasoning

**Mengxiao Tian**<sup>a</sup>, **Fujia Guo**<sup>b</sup>, **Hao Guo**<sup>c</sup>, **Alexey Ruchay**<sup>d</sup>, **Haifeng Wang**<sup>a</sup>, **Nan Jia**<sup>a</sup>, **Bin Li**<sup>*a</sup>, **Xinxiao Wu**<sup>*b</sup>

<sup>a</sup> Intelligent Equipment Research Center, Beijing Academy of Agriculture and Forestry Sciences, Beijing 100097, China  
<sup>b</sup> Beijing Key Laboratory of Intelligent Information Technology, School of Computer Science and Technology, Beijing Institute of Technology, Beijing 100081, China  
<sup>c</sup> College of Land Science and Technology, China Agricultural University, Beijing 100083, China  
<sup>d</sup> Faculty of Economics, Peoples’ Friendship University of Russia, Moscow 117198, Russia  
<sup>*</sup> Corresponding authors: Bin Li (Email: Lib@nercita.org.cn), Xinxiao Wu (Email: wuxinxiao@bit.edu.cn).

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

---|

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
