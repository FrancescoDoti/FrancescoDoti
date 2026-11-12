# Francesco Doti

Applied AI / data science engineer. I build ML systems end to end, and I care most about the part that's usually skipped: **measuring whether they work**, with held-out data, baselines that are hard to beat, uncertainty on the numbers, and a written account of what failed.

## Selected projects

| Project | What it shows | Headline result |
|---|---|---|
| [**safe-sql-mcp**](https://github.com/FrancescoDoti/safe-sql-mcp) | MCP server giving AI agents read-only, policy-checked SQL: AST validation, PII column rules, timeouts, audit log | 77/77 red-team cases as expected, including 13 evasion attempts written after the guard |
| [**invoice-extraction-pipeline**](https://github.com/FrancescoDoti/invoice-extraction-pipeline) | PDF → validated JSON with OCR, arithmetic validation and human-review routing; LLM fallback via schema-forced tool use | 0 wrong amounts auto-approved on 400 test invoices; unseen templates are routed to review, not guessed |
| [**hybrid-retrieval-bench**](https://github.com/FrancescoDoti/hybrid-retrieval-bench) | BM25 vs dense vs fusion vs reranking on BEIR, tuned on train, bootstrap CIs on test, plus a search/answer API | Hybrid +0.062 nDCG@10 over BM25 on SciFact; the off-the-shelf reranker *hurt* |
| [**ticket-triage-classifier**](https://github.com/FrancescoDoti/ticket-triage-classifier) | Banking77 intent triage: TF-IDF vs embeddings vs fine-tuned encoder, temperature calibration, confidence routing | 93.5% accuracy with a 33M-param model; 85.5% of tickets automated at 98.4% accuracy |
| [**demand-forecasting-backtest**](https://github.com/FrancescoDoti/demand-forecasting-backtest) | Day-ahead forecasting with leakage tests, rolling-origin backtest, dev/test protocol, conformal intervals | 11% lower WAPE than seasonal naive; documents why the first model lost to it |
| [**ab-testing-toolkit**](https://github.com/FrancescoDoti/ab-testing-toolkit) | CUPED, delta method, mSPRT sequential tests and SRM checks, each verified by simulation | Naive peeking: 25% false positives; mSPRT: 0.7% |

Earlier work: reinforcement learning for [Scopone](https://github.com/FrancescoDoti/Scopone_RL) (Italian card game) and [Flappy Bird](https://github.com/FrancescoDoti/Flappy_Bird_RL), [eye detection](https://github.com/FrancescoDoti/Eye_Detection), and [NBA Hall of Fame prediction](https://github.com/FrancescoDoti/NBA-memorablia-final).

**Stack:** Python, PyTorch, Hugging Face, scikit-learn, LightGBM, FastAPI, SQL, Docker, MCP, Claude API.
