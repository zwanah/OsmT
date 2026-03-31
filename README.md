# OsmT: Bridging OpenStreetMap Queries and Natural Language with Open-source Tag-aware Language Models

<p align="center">
  <a href="https://arxiv.org/abs/2512.04738"><img src="https://img.shields.io/badge/Paper-arXiv%3A2512.04738-b31b1b?style=for-the-badge&logo=arxiv" alt="Paper"></a>
  <img src="https://img.shields.io/badge/Accepted-ICDE%202026%20Research%20Track-blue?style=for-the-badge" alt="ICDE 2026">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
</p>

> **OsmT** accepted at **ICDE 2026 Research Track** 🎉

---

## 📖 Overview

**OsmT** is an open-source, tag-aware language model designed to bridge **natural language** and **Overpass Query Language (OverpassQL)** — a structured query language for accessing large-scale [OpenStreetMap (OSM)](https://www.openstreetmap.org/) data.

**Paper**: [OsmT: Bridging OpenStreetMap Queries and Natural Language with Open-source Tag-aware Language Models](https://arxiv.org/abs/2512.04738)

---

## 🎬 System Walkthrough & Demo

> **🎥 System Walkthrough Video** — A full explanation of the OsmT system is available:
>
> <p align="center"><a href="https://drive.google.com/file/d/1y4xnFzZr24Nzo0A83mX-nshoiBU6NPFn/view?usp=sharing"><img src="https://img.shields.io/badge/▶%20Watch%20Full%20System%20Walkthrough-Google%20Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white" alt="Watch Full System Walkthrough"/></a></p>

<p align="center">
  <img src="demo/OsmT_Demo.gif" alt="OsmT Demo" width="100%"/>
</p>

<p align="center">
  📹 <a href="https://drive.google.com/file/d/1y4xnFzZr24Nzo0A83mX-nshoiBU6NPFn/view?usp=sharing"><b>Watch full-quality system walkthrough video</b></a>
</p>

The end-to-end workflow of OsmT is illustrated in video. Given either a natural language question or an OverpassQL query as input, OsmT supports a unified interaction process over OpenStreetMap. For natural language input, the system generates executable OverpassQL with the assistance of tag-aware augmentation, executes the query, and visualizes the retrieved spatial entities on the map. For structured queries, OsmT produces corresponding natural language descriptions to facilitate semantic interpretation.

---

## 🗂️ OsmNL Dataset

The **OsmNL** dataset is a new benchmark we manually constructed, building upon the existing [OverpassNL](https://github.com/simonepri/overpass-nl) dataset. It is located at [`dataset/OsmNL/`](dataset/OsmNL/).

| Split | Samples | Description              |
| ----- | ------: | ------------------------ |
| Train |   6,047 | Training set             |
| Dev   |   1,000 | Validation set           |
| Test  |   1,000 | Test set                 |
| Syn   |     133 | Additional training data |

---

## 🖼️ Case Study

Static case study results are available in [`case_study/`](case_study/). For a quick preview with no setup:

1. Open [`case_study/text2ovq_case_study.html`](case_study/text2ovq_case_study.html) in any web browser.
2. The file contains a pre-generated interactive map with 17 geographic features (public squares) — no installation required.

For more details on reproducing the case study, see [`case_study/README.md`](case_study/README.md).

---


## 📄 Citation

If you find OsmT or the OsmNL dataset useful in your research, please cite our paper:

```bibtex
@misc{wan2025osmtbridgingopenstreetmapqueries,
      title={OsmT: Bridging OpenStreetMap Queries and Natural Language with Open-source Tag-aware Language Models}, 
      author={Zhuoyue Wan and Wentao Hu and Chen Jason Zhang and Yuanfeng Song and Shuaimin Li and Ruiqiang Xiao and Xiao-Yong Wei and Raymond Chi-Wing Wong},
      year={2025},
      eprint={2512.04738},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2512.04738}, 
}
```


