# Datathon 2026 — Task 2: Wikipedia Navigation Prediction

Team cupuu — predicting which Wikipedia article a reader clicks next.

## Open this first
- [`cupuu_Task2_Notebook.ipynb`](./cupuu_Task2_Notebook.ipynb) — the final notebook.
- [`cupuu_Task1_Writeup.pdf`](./cupuu_Task1_Writeup.pdf) / [`cupuu_Task2_Writeup.pdf`](./cupuu_Task2_Writeup.pdf) — written report for each task.

## Approach
An initial LightGBM similarity model scored only ~0.28, limited by just 360 unique target
articles to learn from. Wikipedia navigation is closer to a shortest-path problem than a
learned-similarity one, so the final approach OCRs hyperlinks out of page screenshots into
a graph, then predicts the next click as a shortest path toward the target article.

No dataset is committed here.
