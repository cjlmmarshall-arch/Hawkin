# 04 — Beliefs, expectations and forecasting

The best-behaved literature in the social sciences, for one structural reason: the outcome is
observed. A forecast is scored against reality on a date fixed in advance. There is no researcher
degrees-of-freedom problem when the question is "did the thing happen", which is why this field has
made more cumulative progress in fifteen years than adjacent fields have in fifty.

## The datasets

| Dataset | Coverage | What it is | Access |
|---|---|---|---|
| [Good Judgment Project archive](https://dataverse.harvard.edu/dataverse/gjp) | 2011–2015, ~1m forecasts, ~500 questions | The IARPA ACE tournament data | Free (Harvard Dataverse) |
| [Metaculus](https://www.metaculus.com/questions/track-record/) | 2015– , 100k+ questions | Community + aggregate forecasts, full track record | Free API |
| [Manifold](https://manifold.markets) | 2022– | Play-money prediction market | Free API |
| [Polymarket](https://polymarket.com) | 2020– | Real-money prediction market | Public order books |
| [Survey of Professional Forecasters](https://www.philadelphiafed.org/surveys-and-data/real-time-data-research/survey-of-professional-forecasters) | US, 1968– | The longest macro forecast panel | Free |
| [Michigan Surveys of Consumers](https://data.sca.isr.umich.edu) | US, 1946– , monthly | Sentiment and inflation expectations, with party crosstabs | Free |
| [NY Fed Survey of Consumer Expectations](https://www.newyorkfed.org/microeconomics/sce) | US, 2013– , rotating panel | Inflation, labour, household finance expectations | Free |
| [Replication Markets / SSRP](https://osf.io/) | ~3,000 claims scored | Markets forecasting replication outcomes | Free (OSF) |
| [Forecasting Research Institute XPT](https://forecastingresearch.org) | Existential risk questions | Superforecaster vs domain-expert disagreement | Free reports |

## Headline findings

**Aggregation and selection both work, and they compound.** The Good Judgment Project won the IARPA
tournament by roughly 50–70% over the control group's Brier scores — the largest improvement in
judgemental forecasting accuracy in the literature. The winning recipe was unglamorous: identify the
top ~2% of forecasters by track record, put them on teams, extremise the aggregate to correct for
under-confident averaging, and update frequently. Superforecasters ran roughly 60–85% more accurate
than the average forecaster, and — the finding that got the attention — beat intelligence analysts
with access to classified material.

**The skill is real and it persists.** The obvious objection to "superforecasters" is regression to
the mean: pick the top 2% of any noisy process and they will look great in-sample. GJP handled this
by tracking identified superforecasters into *subsequent* years, where they continued to outperform.
Skill, not luck.

**Resolution beats knowledge.** Tetlock's older *Expert Political Judgment* result — that the average
expert is barely better than chance, and that famous experts are worse — has been widely
misread as anti-expertise. What GJP established is more specific: subject-matter knowledge has
modest returns, while *cognitive style* has large ones. Granular probability estimates (the ability
to distinguish 10–15 degrees of uncertainty and stay calibrated), frequent small updates, and
outside-view base rates predict accuracy. Confident narrative coherence predicts inaccuracy.

**Time-horizon advantage.** Superforecasters at 400 days out were about as accurate as regular
forecasters at 150 days. This is the most striking way to state the effect size and the one I would
use on a sceptic.

**Markets forecast replication.** Prediction markets called the outcome of **71%** of Many Labs 2
replications and about **73%** across a pooled 104 studies, beating expert surveys (67%) with lower
prediction error. Set against replication rates of ~39% (Open Science Collaboration, psychology),
~62% (Camerer's Social Sciences Replication Project, 13 of 21 *Nature*/*Science* studies) and around
half for Many Labs 2 — the field could tell in advance which findings were fake, and published them
anyway. That is not a knowledge problem. It is an incentive problem.

## The partisan expectations problem

The Michigan Surveys are the longest-running expectations series and have become, since roughly
2016, partly a measure of something other than expectations. Recent readings have shown Democrat and
Republican sentiment diverging by **50+ index points**, with the gap flipping sign within a month of
an inauguration. For scale: at the trough of the 2008–09 financial crisis, when the economy was
unambiguously terrible for everyone, the partisan gap was a handful of points.

The interpretive question is whether this is **expressive responding** ("cheerleading" — respondents
using a costless survey to signal identity) or genuinely divergent beliefs formed from divergent
media diets. The evidence cuts both ways:

- *For cheerleading:* Bullock, Gerber, Hill and Huber (2015) and Prior, Sood and Khanna (2015) show
  partisan gaps in factual economic questions shrink substantially — by half or more, though not to
  zero — when respondents are paid for correct answers. Partisans face the same prices in the same
  shops; the divergence is not informational.
- *For genuine beliefs:* the gaps show up in *behaviour*, not just talk. Meeuwis, Parker, Schoar and
  Simester (2022) find partisans actually rebalance their brokerage portfolios after elections.
  Mian, Sufi and Khoshkhou find partisan effects on spending. And independents consistently sit
  between the two parties, which pure signalling would not obviously predict.

My view, and it matches what I have argued before: this is a false dichotomy driven by a
poorly-specified notion of belief. Expressive responding and genuine belief are not exclusive
categories — the survey answer is cheap talk *and* the underlying disposition is real enough to move
money, just less real than a point estimate implies. The practical consequence is that the Michigan
series is now much less useful as a macro indicator than it was, particularly its expectations
components, and anyone using it as an input to a policy reaction function is partly tracking the
partisan composition of the sample. The NY Fed SCE, which asks for quantitative densities rather
than directional sentiment, degrades less badly and should be preferred.

## Wider literature

- **Calibration in macro.** The SPF is well-calibrated in normal times and badly calibrated at turning
  points, which is where forecasts have value. The consensus forecast has essentially never predicted
  a recession more than a quarter or two ahead. Fifty-eight years of data and the record is close to
  zero.
- **The wisdom of crowds needs independence.** Simple averaging beats most individuals; extremised
  averaging beats simple averaging; but all of it degrades as forecasters observe each other. This is
  the main argument for keeping some forecasts blind, and prediction platforms have been slow to act
  on it.
- **Existential risk forecasting is where the method breaks.** The FRI's Existential Risk Persuasion
  Tournament found superforecasters and domain experts differing by *orders of magnitude* on
  catastrophic risk probabilities, and — crucially — extended structured debate barely moved either
  side. When questions cannot resolve within a forecaster's lifetime, the feedback loop that makes
  forecasting work is severed, and the observed skill does not transfer. This is the most important
  negative result in the field and it is not cited nearly enough by people quoting p(doom) numbers.
- **Scoring rules matter.** Brier versus log scoring changes rankings, particularly for
  low-probability events. Any track record without its scoring rule attached is uninterpretable.

## Honest summary

Forecasting is the one area here where I would say the literature has *solved* something: we know
how to elicit and aggregate probabilistic judgement, and the methods beat both experts and
institutions. The unsolved part is that the methods depend on rapid resolution, which means they
work worst on exactly the questions — long-run technological, civilisational, existential — that we
most want answered.
