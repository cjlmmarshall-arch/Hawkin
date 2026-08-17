# 01 — Subjective wellbeing

The domain where the gap between "what the data says" and "what everyone knows the data says" is
widest. The famous result — money doesn't buy happiness past a point — has now failed to replicate
three separate times, in three separate ways, and continues to be cited.

## The datasets

| Dataset | Coverage | Instrument | Access |
|---|---|---|---|
| [Gallup World Poll](https://www.gallup.com/analytics/318923/world-poll-public-datasets.aspx) | ~150 countries, 2005– , ~1,000 respondents/country/year | Cantril ladder (0–10), plus affect items | Commercial; aggregates free via [World Happiness Report](https://worldhappiness.report) |
| [World Happiness Report](https://worldhappiness.report) | Country-year aggregates from GWP | Ladder + six explanatory covariates | Free, with underlying tables |
| [Eurobarometer](https://europa.eu/eurobarometer) | EU, 1973– | 4-point life satisfaction | Free (GESIS) |
| [General Social Survey](https://gss.norc.org) | US, 1972– | 3-point happiness item | Free |
| [ONS Annual Population Survey wellbeing](https://www.ons.gov.uk/peoplepopulationandcommunity/wellbeing) | UK, 2011– , ~150k/yr | ONS4: life satisfaction, worthwhile, happy, anxious | Free |
| [Understanding Society](https://www.understandingsociety.ac.uk) | UK, 40k households, panel | GHQ-12 + satisfaction | Free (UKDS registration) |
| [Track Your Happiness](https://www.trackyourhappiness.org) | Killingsworth's ESM app, ~33k people, 1.7m moments | Experience sampling, real-time | Via author |
| [SOEP](https://www.diw.de/soep) | Germany, 1984– , panel | Life satisfaction, 0–10 | Free (application) |

The methodological split that matters: **evaluative** measures (the Cantril ladder — "think of a
ladder, where does your life stand?") versus **experiential** measures (how you felt during a
sampled moment). They correlate but they are not the same construct, and the income literature
behaves differently across the two. Much of the confusion below is people arguing about one while
citing the other.

## Headline: the Easterlin paradox

Easterlin (1974) observed that richer people within a country report more happiness, richer
countries do not obviously report more happiness than poorer ones, and countries growing richer over
time do not get happier. If all three held, income's effect would be purely positional, with large
implications: growth would be a treadmill and redistribution nearly free in welfare terms.

## The corrections

**Between countries, the gradient is real and large.** Stevenson and Wolfers (2008), using GWP,
found a clear log-linear relationship across countries with no satiation point. In the current
Gallup data the within-country slope is roughly **0.3 ladder points per doubling of household
income**; the between-country gradient is at least as steep. There is no income level at which the
cross-sectional line goes flat. Deaton's (2008) analysis of the first GWP wave reached the same
conclusion and was, notably, a reversal of his own prior.

**The within-country and between-country slopes are similar.** This is the finding that does most
damage to the pure-positional reading. If happiness depended only on relative income, the
between-country slope should be near zero while the within-country slope stayed steep. It isn't.

**The time-series claim is where Easterlin still has a case.** Easterlin and O'Connor's
[Easterlin Paradox at 50](https://www.brookings.edu/wp-content/uploads/2025/01/20250116_CSDP_Easterlin_WorkingPaper.pdf)
(2025) restricts to long series and finds the growth–happiness relation is weak or absent over
horizons of a decade or more. The counter is that long series are short in the statistical sense —
you have perhaps a dozen effectively independent observations per country, standard errors are
wide, and "we cannot reject zero" is being reported as "it is zero". My read: the time-series
evidence is genuinely underpowered, which means it supports agnosticism rather than Easterlin's
positive claim.

## The $75,000 saga, and why it is the best story in the field

- **Kahneman and Deaton (2010)**, Gallup daily poll: experienced wellbeing rose with income up to
  ~$75k/yr and then plateaued. Evaluative wellbeing kept rising. The plateau went into a million
  op-eds; the second half did not.
- **Killingsworth (2021)**, experience sampling: no plateau. Wellbeing rose log-linearly past $75k.
- **[Killingsworth, Kahneman and Mellers (2023)](https://www.pnas.org/doi/10.1073/pnas.2208661120)**,
  an adversarial collaboration — the two principals jointly reanalysing the ESM data with a
  pre-agreed protocol. Result: both were right about different people. For the least happy
  ~15–20%, wellbeing rises with income to roughly $100k and then flattens. For everyone else it
  keeps rising, and for the happiest group the slope *steepens*. Kahneman's original plateau was a
  bottom-of-the-distribution effect that mean-based analysis had smeared across the whole sample.

This is the model of how a disagreement should be resolved, and it is worth noting why it worked:
both parties committed in advance to an analysis that could embarrass either of them. Kahneman
co-authored the paper that overturned his own most-cited empirical claim, a year before he died.

The saga is not quite over. A [2024 reanalysis](https://arxiv.org/pdf/2401.05347) argues for a
plateau nearer $200k, and [commentaries in PNAS](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11572929/)
object that KKM's income coefficients are being read causally when the design is cross-sectional.
The second objection is correct and applies to essentially this entire literature: nothing here
randomises income. The one place it is randomised — lottery studies, e.g. Lindqvist, Östling and
Cesarini (2020) on Swedish administrative data — finds persistent gains in life satisfaction, more
modest gains in happiness, and effects that do not fade over a decade. That is the closest thing to
a clean identification the field has, and it points the same way.

## Wider literature

- **Adaptation is selective, not universal.** Clark et al. (2008) and the SOEP literature find near-
  complete adaptation to marriage, partial to divorce and widowhood, and strikingly little to
  unemployment and to disability. Unemployment leaves a scar in life satisfaction that does not close
  even after re-employment. If you want one policy implication from this entire field, it is that
  unemployment is far more expensive in welfare terms than the income loss implies.
- **The U-shape in age is contested.** Blanchflower finds a midlife trough in ~130 countries; Galambos,
  Bartolini and others argue it is an artefact of controlling for variables (income, marital status,
  employment) that are themselves consequences of age. Conditioning on mediators to find a "pure"
  age effect is a mistake, and this literature makes it constantly.
- **Cardinality.** Bond and Lang (2019) showed that ordinal happiness data can have its group
  rankings reversed by monotone rescaling, so "are Danes happier than Americans" may be
  non-identified without a cardinality assumption. Kaiser and Vendrik (2023) reply that the
  reversals require implausibly extreme transformations. Unresolved, and it undercuts far more
  published work than has been withdrawn.
- **Wellbeing as a policy objective.** The UK's [Green Book](https://www.gov.uk/government/publications/green-book-supplementary-guidance-wellbeing)
  wellbeing supplement now permits WELLBY-based appraisal, at roughly £13,000 per WELLBY. This is a
  real institutional commitment resting on a literature that has not settled cardinality (above).
  Worth watching whether the measurement problems bite in practice or turn out to be second-order.

## Honest summary

Income raises subjective wellbeing, roughly log-linearly, with no satiation point that survives
scrutiny, and the effect is not purely relative. The residual Easterlin claim — that *national*
growth does not raise *national* average happiness over long horizons — is not refuted, but it is
supported by data too thin to carry the weight placed on it. The interesting frontier is not
whether money buys happiness (it does, at a declining rate) but why the unhappy tail is so much less
responsive to income than everyone else.
