## Mihir Parekh

M.S. Artificial Intelligence, Wayne State University. Based in Michigan.

I build AI systems and then try to break them. Every repository below documents
something that went wrong and how it was caught — because the failures are
where the engineering is.

### Projects

**[arxiv-research-assistant](https://github.com/MihirParekh14/arxiv-research-assistant)** — retrieval-augmented question answering over 253,405 passages
Found two retrieval failure modes by testing it. Fixed one with a cross-encoder
reranker, documented the other as still open. The system refuses to answer when
its best match is weak, because a confident wrong answer with a citation
attached is harder to catch than no answer. *140 tests.*

**[llm-adaptation-study](https://github.com/MihirParekh14/llm-adaptation-study)** — LoRA fine-tuning against in-context learning, 77 classes
Three measurement bugs found by running it, each of which produced a believable
number and raised nothing. The finding: scoring model answers by exact string
match grades instruction-following rather than capability — worth 15 points on
one model and zero on another. *87 tests, none needing a GPU.*

**[job-salary-prediction](https://github.com/MihirParekh14/job-salary-prediction)** — salary modelling across 33,246 job postings
38% of disclosed pay was quoted hourly in the same column as annual figures.
And only 40% of postings disclose pay at all — 72% in Colorado against 19% in
Louisiana, tracking state transparency law, which makes the modelling sample a
regulated subset rather than the market. *62 tests.*

**[telco-churn-prediction](https://github.com/MihirParekh14/telco-churn-prediction)** — churn classifier, rebuilt
Four defects in the original, including preprocessing fitted before the
train/test split — which inflated every score it reported. *15 tests.*

### How I work

Tests alongside the code, CI on every push, and a README that says what the
limitation is rather than leaving it out. 304 tests across four repositories.

Python · PyTorch · scikit-learn · FAISS · Transformers · Docker · SQL

### Contact

[LinkedIn](https://linkedin.com/in/mihirparekh14) · parekhmihir1410@gmail.com
