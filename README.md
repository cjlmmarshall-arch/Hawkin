# Datasets I like

A working catalogue of the empirical infrastructure behind the things I write about at
[Microfounded](https://microfounded.substack.com): economics, the social sciences, culture, AI,
anti-ageing. Each file covers one domain: what the data actually is, who collects it, what it has
established, and — usually the more interesting part — what it has failed to settle.

The organising bias is simple. Most arguments in the social sciences are not arguments about
values dressed up as arguments about facts. They are arguments about *measurement* dressed up as
arguments about the world. The Easterlin paradox is a dispute about whether you compare within or
between countries. The US inequality debate is a dispute about where to allocate untaxed business
income. The lifespan-limit debate is a dispute about which populations count as the frontier. In
each case, people who agree on the numbers disagree on the answer, because the numbers are not the
answer — the mapping from numbers to answer is.

So these notes try to do three things per dataset: state the headline finding, state the strongest
objection to it, and be explicit about which of the two the data can adjudicate.

## Contents

| # | File | Domain | The fight worth having |
|---|------|--------|------------------------|
| 01 | [Subjective wellbeing](datasets/01-wellbeing.md) | Happiness, life satisfaction | Does the income–happiness gradient flatten, and for whom? |
| 02 | [Growth and inequality](datasets/02-growth-and-inequality.md) | National accounts, distributional statistics | Has the US top 1% share risen 6 points or 1 point since 1960? |
| 03 | [Mobility and place](datasets/03-mobility-and-place.md) | Administrative tax data, panel surveys | Is mobility about neighbourhoods, or about who lives in them? |
| 04 | [Beliefs and forecasting](datasets/04-beliefs-forecasting.md) | Forecasting tournaments, expectation surveys | Do survey answers report beliefs or announce identities? |
| 05 | [Politics and institutions](datasets/05-politics-and-institutions.md) | Democracy indices, election studies | Is measured democratic decline decline, or drifting coders? |
| 06 | [Culture and values](datasets/06-culture-and-values.md) | Value surveys, text corpora | Does development cause value change, or merely accompany it? |
| 07 | [Ageing and health](datasets/07-ageing-and-health.md) | Mortality, biobanks, ageing panels | Are we near a lifespan ceiling or just a bad three decades? |
| 08 | [AI progress](datasets/08-ai-progress.md) | Compute, capability, evaluation | Are we measuring capability or measuring benchmarks? |
| 09 | [Development and RCTs](datasets/09-development-and-rcts.md) | Household surveys, trial registries | What generalises out of a randomised trial, and to where? |

## House rules for reading any of this

**1. Within ≠ between.** The single most productive question to ask of a social-science claim is
whether the correlation is identified across individuals, across countries, or across time within a
unit. These frequently have different signs, and almost every famous "paradox" in the field is a
collision between two of them (§01 is the canonical case).

**2. Distributional statistics are constructions, not observations.** Nobody observes the top 1%
share. It is assembled from tax records plus assumptions about the income that never reaches tax
records. Two competent teams working from the same IRS microdata produce answers that differ by a
factor of six on the trend (§02). Any headline number of this type should be read with its
allocation rules attached.

**3. Composition eats trends for breakfast.** Panel and repeated cross-section series confound
"units changed" with "the set of units changed". Rising average education in a cohort study, falling
average democracy in a country panel, changing survey response rates — all can move a series with no
underlying change in any unit.

**4. Selected samples do not become representative by being large.** UK Biobank has half a million
people and a 5.5% response rate; it is healthier, richer and more educated than the UK. It is
superb for genetic association (where selection is mostly orthogonal to genotype) and treacherous
for prevalence (where it is not). Size is not representativeness — it is precision about a possibly
wrong quantity (§07).

**5. Prefer the paper that specifies its falsifier.** Across every domain here, the literatures that
have made real progress — forecasting, replication, mortality — are the ones where someone wrote
down in advance what would count as being wrong (§04).

## Conventions

- Every dataset entry gives an access route. Most of these are free; the ones with an application
  process are marked.
- Figures are as of the most recent release I checked; releases move, so treat numbers as of
  mid-2026 and re-check before citing.
- Where a finding is contested, I have tried to state the dissent in its strongest form rather than
  its most quotable one. Where I have a view, I say so and mark it as a view.
- "Headline" means the finding that gets cited. "Honest summary" means what I think the data
  supports. These differ often enough to be worth separating.
