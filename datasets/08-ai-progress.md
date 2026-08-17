# 08 — AI progress

The youngest literature here, and the one where the measurement problem is most acute: the inputs
(compute, parameters, data) are measured well, and the outputs (capability) are measured badly. Most
disagreement about AI trajectories is downstream of that asymmetry.

## The datasets

| Dataset | Coverage | What it is | Access |
|---|---|---|---|
| [Epoch AI database](https://epoch.ai/data) | 3,500+ models, 1950– | Training compute, parameters, dataset size, cost, power | Free, CSV |
| [Epoch Trends](https://epoch.ai/trends) | Ongoing | Curated trend estimates with methodology | Free |
| [Stanford AI Index](https://aiindex.stanford.edu) | Annual since 2017 | Broad compilation: capability, investment, policy, opinion | Free |
| [METR time horizons](https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/) | 2019– | Task length at 50% success, benchmarked to human completion time | Free |
| [LMArena / Chatbot Arena](https://lmarena.ai) | 2023– , millions of votes | Blind pairwise human preference, Elo-style | Free (public leaderboard + released votes) |
| [Open LLM Leaderboard / HELM](https://crfm.stanford.edu/helm/) | Many models | Standardised multi-metric evaluation | Free |
| [Papers With Code / SOTA](https://paperswithcode.com/sota) | Benchmark histories | Long-run benchmark saturation curves | Free |
| [AI Incident Database](https://incidentdatabase.ai) | 2018– | Catalogued deployment harms | Free |
| [Our World in Data — AI](https://ourworldindata.org/artificial-intelligence) | Curated | Epoch data, charted and sourced | Free, CC-BY |

## Headline findings

**Compute is the cleanest trend in the field.** Epoch's database — the largest of its kind, tracking
3,500+ notable models — puts training compute for notable systems doubling roughly every **6 months**
since 2010, and for frontier language models roughly every **5.2 months** since 2020. For context, a
6-month doubling is about 4× per year, against Moore's Law's ~2× every 2 years. Training compute has
grown by something like nine orders of magnitude since AlexNet. Training cost for the largest models
doubles every ~8 months, and global AI compute capacity has grown ~3.3× per year since 2022.

The reason this trend matters more than a capability benchmark: it is *measured in physical units*,
it cannot be gamed, and it is bounded by things — fabs, power, capital — that have known, slow
supply curves. It is the closest thing to an exogenous clock the field has.

**Capability, measured as task duration, is on its own exponential.** METR's contribution was to
stop asking "what score does it get" and start asking "how long a task can it finish". Their metric —
the length of task (as timed on skilled humans) that an agent completes with 50% reliability — has
doubled roughly every **7 months** over 2019–2025, from seconds to hours. Their more recent tracking
suggests **~4 months** over 2024–2025, i.e. acceleration.

This is the best capability metric anyone has built, for three reasons: the units are human-
interpretable, it is not saturable (you can always time longer tasks), and it is anchored to human
performance rather than to an arbitrary scale. It is also, and this should be stated clearly, built
on a software-engineering task distribution of a few hundred tasks, so extrapolating it to "AI can do
X% of the economy" involves a leap the data does not license.

**Benchmarks saturate, and saturation is not progress.** The Papers With Code histories show the same
pattern repeatedly: a benchmark is introduced, sits near-flat, then goes from well-below to
above-human in two or three years, and is retired. MMLU, GSM8K, HumanEval have all followed it.
Because benchmarks are retired when saturated, the *observable* benchmark set is permanently composed
of unsaturated ones, which systematically understates progress in retrospectives and overstates
remaining difficulty in forecasts. This selection effect is rarely acknowledged.

**Contamination is the field's replication crisis.** Test sets leak into training corpora. The effect
is measurable — models do markedly better on pre-cutoff versions of a benchmark than on freshly
generated post-cutoff variants of the same difficulty (the GSM1k and similar studies). Any benchmark
number without contamination controls should be discounted, and most are.

## What the data does not tell you

**The scaling laws are about loss, not capability.** Kaplan et al. (2020) and Hoffmann et al. (2022,
"Chinchilla") establish smooth power-law relationships between compute, data, parameters and
cross-entropy loss. These are among the most reliable empirical regularities in computer science.
But the object being predicted is next-token prediction loss, and the mapping from loss to *anything
anyone cares about* is neither smooth nor characterised. Chinchilla's revision — that prior models
were substantially undertrained relative to compute-optimal — moved the field's entire resource
allocation on the basis of loss curves alone.

**"Emergence" was partly a measurement artefact.** Wei et al. (2022) reported capabilities appearing
discontinuously at scale. Schaeffer, Miranda and Koyejo (2023) showed that much of this is produced
by discontinuous metrics: score a task with exact-match accuracy and you get a sharp jump; score the
same model outputs with a continuous metric (token edit distance, log-probability of the correct
answer) and the improvement is smooth. Not all claimed emergence dissolves, but the strong version
of the thesis does. This is a very good example of the general rule in this repo: the metric made
the phenomenon.

**Arena rankings measure preference, not correctness.** LMArena's blind pairwise voting is valuable
because it is hard to game directly and reflects real user judgement. But human raters reward
formatting, length, confidence and agreeableness, and the correlation between Elo and factual
accuracy is imperfect. There is also a live concern about private variant testing letting labs
select their best-performing checkpoint for public release, which is a selection effect on the
leaderboard rather than on the models.

## Wider literature

- **Economic impact is thin.** The productivity evidence is a handful of well-designed field
  experiments — Brynjolfsson, Li and Raymond on customer support (~14% average, concentrated in
  novices), Noy and Zhang on writing, Peng et al. on GitHub Copilot, Dell'Acqua et al. on BCG
  consultants (the "jagged frontier": large gains inside the frontier, *negative* gains outside it).
  These are all short-horizon, single-task, and mostly pre-agentic. Aggregate productivity statistics
  show nothing yet, which is either the Solow paradox repeating or evidence the gains are smaller
  than claimed. Too early to say, and anyone confident either way is not reasoning from data.
- **Compute forecasting.** Epoch's data-constraint work (Villalobos et al.) projects the stock of
  high-quality public text being exhausted around the late 2020s at current consumption growth. The
  responses — synthetic data, multimodal corpora, RL from verifiable rewards, inference-time compute —
  are all real, and whether they substitute cleanly for human text is the open question that most
  affects the trend line.
- **The inference-time shift breaks the old metrics.** Once models spend variable compute at inference,
  "the capability of model X" is no longer well-defined without specifying a compute budget, and a
  single point on a leaderboard hides a curve. Most reporting has not caught up with this, and the
  measurement infrastructure will need rebuilding around capability-per-dollar rather than
  capability-per-model.
- **Forecasting AI is where superforecasting fails.** See §04: the Existential Risk Persuasion
  Tournament found superforecasters and AI domain experts differing by orders of magnitude on
  catastrophic risk, with structured debate barely moving either group. The forecasting methods that
  work on 6-month geopolitical questions have no demonstrated validity here, and the confidence with
  which numbers from this domain get quoted is unwarranted in both directions.

## Honest summary

Use Epoch for inputs, METR for capability trends, and treat every benchmark leaderboard as a
lower bound with an unknown contamination correction. The compute trends are the most reliable
quantitative fact about AI; the mapping from compute to capability is decently characterised; the
mapping from capability to economic or social consequence is essentially uncharacterised, and that
last gap is where all the interesting disagreement actually lives.
