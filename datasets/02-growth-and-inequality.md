# 02 — Growth and inequality

Two literatures with opposite epistemic characters. Long-run growth data is thin, heroic and
broadly agreed on. Inequality data is thick, administrative and violently disputed. The reason is
instructive: growth statistics are contested at the point of *historical reconstruction*, where
everyone knows the error bars are enormous, while inequality statistics are contested at the point
of *imputation*, where the error bars are invisible in the published series.

## The datasets

| Dataset | Coverage | What it is | Access |
|---|---|---|---|
| [Penn World Table 10.x](https://www.rug.nl/ggdc/productivity/pwt/) | 183 countries, 1950– | PPP-adjusted output, capital, TFP, hours | Free |
| [Maddison Project Database](https://www.rug.nl/ggdc/historicaldevelopment/maddison/) | ~170 countries, some to year 1 | Historical GDP per capita reconstructions | Free |
| [World Inequality Database](https://wid.world) | 200+ countries | Distributional national accounts (DINA) | Free |
| [Luxembourg Income Study](https://www.lisdatacenter.org) | 50+ countries, harmonised microdata | Household income/wealth surveys | Free (registration, remote execution) |
| [Auten–Splinter series](http://www.davidsplinter.com/) | US, 1960– | Alternative US distributional estimates | Free |
| [Distributional Financial Accounts](https://www.federalreserve.gov/releases/z1/dataviz/dfa/) | US, 1989– , quarterly | Fed wealth distribution tied to Z.1 | Free |
| [Our World in Data](https://ourworldindata.org) | Global | Curated, sourced, chart-first aggregation | Free, CC-BY |
| [SWIID](https://fsolt.org/swiid/) | 200 countries, 1960– | Imputed comparable Gini series | Free |
| [Long-Term Productivity Database](http://www.longtermproductivity.com) | Advanced economies, 1890– | Bergeaud–Cette–Lecat productivity | Free |

## Headline findings: growth

**Divergence, big time.** Pritchett's (1997) framing survives every data revision: the ratio between
richest and poorest countries has widened enormously since 1820. The Maddison reconstructions put
the spread at maybe 3:1 in 1820 and 50:1 or more by the late twentieth century.

**But the last three decades ran the other way.** Since roughly 1990, and decisively since 2000,
population-weighted between-country inequality has *fallen*, driven almost entirely by China and
India. The Milanović "elephant curve" summarises it: large real gains for the global middle
(Asian), stagnation for the lower-middle of rich countries, large gains at the very top. How much
of the rich-country stagnation is real versus an artefact of changing country composition in the
underlying surveys is disputed — Corlett's reanalysis shows the elephant's dip flattens considerably
when you hold country composition fixed.

**TFP, not factor accumulation, explains most cross-country income variation.** This is the Hall–
Jones and Klenow–Rodríguez-Clare result, and PWT exists largely to let people re-run it. It
survives, which is awkward, because TFP is a residual and "the residual explains it" is a confession
rather than an explanation.

**Convergence is conditional, and unconditional convergence may have arrived late.** Post-2000
there is more unconditional catch-up than in 1960–2000 (Patel, Sandefur and Subramanian, 2021),
partly commodity-cycle-driven. Whether that survives the 2020s is an open empirical question.

## The fight: US top income shares

Same underlying IRS microdata, two teams, incompatible answers:

| | Top 1% after-tax-and-transfer share, 1960 | 2019 |
|---|---|---|
| Piketty, Saez, Zucman (WID) | ~9% | ~15% |
| [Auten and Splinter](https://www.journals.uchicago.edu/doi/10.1086/728741) (JPE 2024) | ~8% | ~9% |

A six-point rise versus a one-point rise. This is not a rounding disagreement; it is the difference
between "the defining economic fact of the era" and "basically nothing happened".

The disagreement is almost entirely about **income that does not appear on tax returns** — retained
corporate earnings, underreported business income, imputed rents, tax-exempt benefits, and the
government spending that has to be allocated to someone. Roughly a third of national income is in
this category, and the series are built by allocating it. Auten and Splinter allocate a large and
growing share of unreported business income proportionally to *reported* income, which pushes it
down the distribution; PSZ allocate it in proportion to audit-based estimates of where evasion
actually occurs, which is concentrated at the top. PSZ's
[2024 technical note](https://wid.world/news-article/new-research-uncovers-key-mistakes-in-auten-and-splinters-estimates-of-us-inequality/)
argues that correcting this alone reconciles most of the gap; Auten and Splinter disagree.

My read: the honest position is that the *level* of top shares is not well identified, but the
*direction* is. Corroborating series that don't depend on the contested imputations — the Fed's
Distributional Financial Accounts on wealth, Forbes-style top-wealth data, executive compensation,
and the capital share of national income — all move up. It is hard to construct a world in which the
top 1% income share is flat while every adjacent indicator rises. But anyone quoting either series
to two significant figures is overstating what the data can bear.

A separate and underrated point: the two teams also disagree about **transfers**. Much of Auten–
Splinter's flatness comes from the growth of Medicare, Medicaid and other in-kind transfers, counted
at government cost. Whether health insurance received at a cost of $15,000 is worth $15,000 of
income to the recipient is a welfare question that no distributional series can answer, and both
teams are effectively making an assumption about it.

## Wider literature

- **Capital in the Twenty-First Century** and r > g. The empirical core — rising wealth-to-income
  ratios in rich countries — has held up better than the theoretical mechanism. Rognlie's (2015)
  decomposition showed the rise in the net capital share is almost entirely *housing*, which
  redirects the policy conclusion from capital taxation to land use. This is one of the most
  important and least-absorbed findings of the decade.
- **Top-end survey non-response.** Household surveys systematically miss the rich. The correction
  literature (Blanchet, Flores and Morgan) matters enormously for LIS- and SWIID-based cross-country
  comparisons, and most users of those series don't apply it.
- **Inequality of what.** Consumption inequality has risen much less than income inequality in the
  US (Meyer and Sullivan), which is either evidence that income data overstates the trend or that
  consumption data understates it via the same top-end non-response problem. Probably both.
- **The productivity slowdown.** Bergeaud–Cette–Lecat and the Long-Term Productivity Database show
  the post-1970 slowdown is common to essentially all frontier economies with a common timing, which
  is hard to square with country-specific policy explanations. Bloom et al.'s "Are ideas getting
  harder to find?" is the leading supply-side account; Gordon's is the demand-for-innovation account.
  Neither has a falsifier anyone has agreed on, which is why the debate is 15 years old and static.

## Honest summary

Growth data is more reliable than it looks and inequality data is less. If you want one
recommendation: use PWT for anything cross-country and levels-based, use WID and Auten–Splinter
*together* as a bracket rather than choosing, and treat any single-source Gini time series
(especially SWIID's imputed ones) as an indicator with a confidence interval wide enough to contain
most of the claims people make with it.
