# Multilingual Skill Extraction: Hard and Soft Skills

This repository centralizes our research on **skill extraction and classification** from
job offers and resumes in a **multilingual, multidomain** setting. The work
was carried out through a multidisciplinary, industry-grounded collaboration among HR researchers,
NLP researchers and HR-tech professionals, covering six languages, **English, French, German,
Italian, Spanish, and Portuguese**, for both **hard-skill extraction** and
**soft-skill classification**.

By [Laura Vásquez-Rodríguez](https://www.linkedin.com/in/lmvasque/),
[Bertrand Audrin](https://www.linkedin.com/in/bertrand-audrin/),
[Samuel Michel](https://www.linkedin.com/in/sam-mchl/),
[Samuele Galli](https://www.linkedin.com/in/samuele-galli/),
[Julneth Rogenhofer](https://www.linkedin.com/in/julneth-rogenhofer/),
[Jacopo Negro Cusa](https://www.linkedin.com/in/jacoponegrocusa/) and
[Lonneke van der Plas](https://www.linkedin.com/in/lvdplas/).

This README instead acts as a single entry point to the **publications** and the **public datasets** used to keep our benchmarks reproducible (see [Data Availability](#data-availability)).

## Publications

### Skill Extraction from Resumes and Job Offers across Six Languages

📄 [Paper](https://publications.idiap.ch/publications/show/5859) · accepted at the
[11th Swiss Text Analytics Conference (SwissText), 2026](https://www.swisstext.org/call-for-papers/).

> **TL;DR** — We comprehensively evaluate rule-based, semantic, and supervised skill-extraction
> methods on **1,200 annotated job offers and resumes** across six languages and diverse domains.
> Supervised models reach F1 scores up to **0.6**, while rule-based methods offer better
> interpretability. We find that skills are formulated very differently in resumes vs. job offers,
> with resumes notably understudied in prior academic work.

### Soft Skills in the Wild: Challenges in Multilingual Classification

📄 [Paper](https://publications.idiap.ch/publications/show/5592) · accepted at the
[10th Swiss Text Analytics Conference (SwissText), 2025](https://www.swisstext.org/archive/swisstext-2025/).


> **TL;DR** — Using a **multilingual BERT-based classifier** for soft skills, we compare soft
> skills, hard skills, and occupations along surface-level and semantic properties. Even when
> constrained to established taxonomy categories, soft skills show far greater variability in their
> textual expression than other entity types, a key challenge for recruitment algorithms.

## Data Availability

Due to the proprietary nature of the job offers and resumes provided by our industrial partner,
the release of the primary dataset is restricted. To ensure reproducibility while respecting these
constraints, we adopt two strategies:

1. **Experiments on public data.** Alongside the proprietary benchmarks, we report results on
   publicly available job offers and taxonomies (see [Public Datasets](#public-datasets) below).
2. **Methodological transparency.** Our papers document the methodology in full so the benchmarks
   remain as reproducible as possible, providing a transparent framework for our real-world
   skill-extraction approach.

## Public Datasets

| Dataset | Language(s) | Skill type | Link |
|---|---|---|---|
| Green | English | Hard / ICT skills in job ads | https://huggingface.co/datasets/jjzha/green |
| ESCO taxonomy | Multilingual (EU) | Skill & occupation taxonomy | https://esco.ec.europa.eu/en/use-esco/download |
| Fijo | French | Soft skills (insurance job ads) | https://huggingface.co/datasets/jjzha/fijo |
| Sayfullina | English | Soft skills | https://huggingface.co/datasets/jjzha/sayfullina |

## Citation

If you use this work, please cite the relevant paper(s):

```bibtex
@inproceedings{vasquez-rodriguez-etal-2026-skill,
    title = "Skill Extraction from Resumes and Job Offers across Six Languages",
    author = "V{\'a}squez-Rodr{\'i}guez, Laura  and
      Audrin, Bertrand  and
      Michel, Samuel  and
      Galli, Samuele  and
      Rogenhofer, Julneth  and
      Cusa, Jacopo Negro  and
      van der Plas, Lonneke",
    booktitle = "Proceedings of the 11th edition of the Swiss Text Analytics Conference",
    year = "2026"
}
```

```bibtex
@inproceedings{vasquez-rodriguez-etal-2025-soft,
    title = "Soft Skills in the Wild: Challenges in Multilingual Classification",
    author = "V{\'a}squez-Rodr{\'i}guez, Laura  and
      Audrin, Bertrand  and
      Michel, Samuel  and
      Galli, Samuele  and
      Rogenhofer, Julneth  and
      Cusa, Jacopo Negro  and
      van der Plas, Lonneke",
    editor = {Gerber, Jonathan  and
      Cieliebak, Mark  and
      Tuggener, Don  and
      H{\"u}rlimann, Manuela},
    booktitle = "Proceedings of the 10th edition of the Swiss Text Analytics Conference",
    month = may,
    year = "2025",
    address = "Winterthur, Switzerland",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.swisstext-1.11/",
    pages = "108--114"
}
```



## Acknowledgments

This research was conducted at [Idiap Research Institute](https://www.idiap.ch/) as part of the
**SEM24** project, funded by [Innosuisse](https://www.innosuisse.admin.ch/), the Swiss Innovation
Agency, and carried out in collaboration with our industrial partner [Arca24](https://www.arca24.com/), whose job offers and resumes made this multilingual, real-world study possible.
