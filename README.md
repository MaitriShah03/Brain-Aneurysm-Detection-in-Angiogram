Great! Now that you've provided the GitHub link for the IntrA dataset, here’s an enhanced version of your **README.md**, updated to reference the official dataset repository and align with best practices:

---

# Brain Aneurysm Detection using Deep Learning (ResNet-18 + IntrA Dataset)

## Overview

A deep learning project aimed at detecting intracranial aneurysms using a ResNet-18 model trained on the **IntrA 3D Intracranial Aneurysm Dataset**, which contains 3D vascular models constructed from MRA scans. The aim is to achieve high diagnostic accuracy and improve clinical interpretability via Grad-CAM visualizations.

---

## Dataset – IntrA

The **IntrA dataset** is an open-access resource containing:

* 103 reconstructed 3D models of complete brain vessels, generated from 2D time-of-flight MRA scans, split into

  * 1,909 vessel segments: 1,694 healthy and 215 aneurysm segments
  * 116 aneurysm segments manually annotated by medical experts
* Pre-computed geodesic distance matrices to enhance processing accuracy and efficiency ([GitHub][1], [CVF Open Access][2])

You can access the dataset here: **[https://github.com/intra3d2019/IntrA](https://github.com/intra3d2019/IntrA)** ([arXiv][3], [GitHub][1]).

---

## Key Features

* High classification accuracy (\~96%) using **ResNet-18**
* Handles class imbalance via **weighted cross-entropy**, improving recall by 22%
* Uses **Grad-CAM** for visual explanations, enhancing clinical trust
* Robust preprocessing: window-level normalization, affine transformations, and geodesic-aware feature engineering

---

## Tech Stack

| Component         | Tools & Libraries             |
| ----------------- | ----------------------------- |
| **Language**      | Python                        |
| **Frameworks**    | PyTorch, OpenCV, Scikit-learn |
| **Visualization** | Matplotlib, Grad-CAM          |
| **Notebook**      | Jupyter Notebook (`.ipynb`)   |

---

## Usage Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/<your-username>/brain-aneurysm-detection.git
cd brain-aneurysm-detection
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Download & Prepare Dataset

* Clone or download the IntrA dataset from its official repository.
* Update the dataset path in your notebook or configuration script accordingly.

### 4. Execute Notebook

Launch the Jupyter Notebook:

```bash
jupyter notebook "Brain Aneurysm Detection_20 Epochs.ipynb"
```

Follow the notebook cells for full preprocessing, training, evaluation, and visualization.

---

## Performance Summary

| Metric    | Value  |
| --------- | ------ |
| Accuracy  | \~96%  |
| Recall    | 0.95   |
| Precision | 1.00   |
| F1-Score  | \~0.97 |

**Grad-CAM** outputs provide interpretable heatmaps for validation and trust in decision regions.

---

## Future Enhancements

* Expand to **3D CNN architectures** for volumetric data
* Integrate **attention modules** for improved localization
* Optimize model for **real-time inference** in clinical environments

---

## Acknowledgements

* **Dataset**: IntrA: 3D Intracranial Aneurysm Dataset for Deep Learning (CVPR 2020) ([GitHub][1], [arXiv][3])
* **Authors**: Xi Yang et al.
* Please cite their paper when referencing the dataset ([arXiv][3]).

---

## About the Author

**Maitri Shah**

* M.Tech (AI & ML), PDPM IIIT Jabalpur
* B.Tech (Electronics & Communication), Dharmsinh Desai University
* Email: [shahmaitri01@gmail.com](mailto:shahmaitri01@gmail.com)
* [LinkedIn](https://www.linkedin.com/in/maitri-sanjay-shah) • [Hackerrank](https://www.hackerrank.com/profile/shahmaitri01)

---

[1]: https://github.com/intra3d2019/IntrA?utm_source=chatgpt.com "IntrA: 3D Intracranial Aneurysm Dataset for Deep Learning - GitHub"
[2]: https://openaccess.thecvf.com/content_CVPR_2020/papers/Yang_IntrA_3D_Intracranial_Aneurysm_Dataset_for_Deep_Learning_CVPR_2020_paper.pdf?utm_source=chatgpt.com "[PDF] IntrA: 3D Intracranial Aneurysm Dataset for Deep Learning"
[3]: https://arxiv.org/abs/2003.02920?utm_source=chatgpt.com "IntrA: 3D Intracranial Aneurysm Dataset for Deep Learning"
