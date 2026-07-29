# Arabic Fake News Detection

Academic NLP research project using AraBERT and stylometric features.

## Summary

This project evaluates Arabic fake-news/source-credibility classification using the Arabic Fake News Dataset (AFND). It proposes LinguaBERT-Arabic, which combines AraBERT with simple stylometric features.

The project uses a strict source-disjoint split, meaning test sources were not seen during training. This makes the evaluation harder and more realistic than a random article split.

## Portfolio Label

Best public label:

> Academic research project

## Feature Design

The proposed model adds five stylometric features:

- Sensationalism
- Type-token ratio
- Numerical density
- Elongation rate
- Negative sentiment proxy

## Main Results

Final reported test results:

| Model | Macro F1 |
| --- | ---: |
| NB with TF-IDF | 0.4940 |
| LinguaBERT-Arabic | 0.4332 |
| Vanilla AraBERT | 0.4055 |

The honest conclusion is that stylometric features improved over vanilla AraBERT, but the simple NB TF-IDF baseline performed best overall in this run.

## Security and Ethics Relevance

This is useful for misinformation analysis and Arabic NLP, but the project correctly notes that fake-news models should support human judgment, not replace it. AFND labels are source-credibility based, so the model should not be treated as a final truth detector for individual articles.

## Repository Contents

- `artifacts/Arabic_Fake_News_Detection_Research_Paper.pdf` - academic research paper
- `notebooks/Arabic_Fake_News_Detection_Code_public.ipynb` - public sanitized executed notebook

The paper is uploaded in its original academic PDF format. The notebook copy is sanitized for public release.
