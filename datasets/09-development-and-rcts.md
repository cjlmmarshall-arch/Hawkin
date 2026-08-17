# 09 — Development, household surveys and RCTs

The field that won a Nobel for solving internal validity and then spent a decade discovering that
external validity is the harder problem.

## The datasets

| Dataset | Coverage | What it is | Access |
|---|---|---|---|
| [DHS Program](https://dhsprogram.com) | 90+ countries, 400+ surveys, 1984– | Health, fertility, nutrition, anthropometrics, GPS clusters | Free (registration) |
| [World Bank LSMS](https://www.worldbank.org/en/programs/lsms) | 40+ countries | Detailed consumption and income modules | Free |
| [MICS](https://mics.unicef.org) | 118 countries | UNICEF's child-focused counterpart to DHS | Free |
| [Afrobarometer](https://www.afrobarometer.org) / [Latinobarómetro](https://www.latinobarometro.org) | Regional | Attitudes, governance, service delivery | Free |
| [PovcalNet / PIP](https://pip.worldbank.org) | Global | The $2.15/day poverty line machinery | Free |
| [AEA RCT Registry](https://www.socialscienceregistry.org) | 8,000+ trials | Pre-registration and pre-analysis plans | Free |
| [J-PAL evaluations](https://www.povertyactionlab.org/evaluations) | 1,000+ RCTs | Searchable trial database with replication data | Free |
| [3ie Development Evidence Portal](https://developmentevidence.3ieimpact.org) | 10,000+ studies | Impact evaluations and systematic reviews | Free |
| [Enterprise Surveys](https://www.enterprisesurveys.org) | 150+ countries | Firm-level constraints and performance | Free |
| [Demographic and health GPS + satellite](https://www.nature.com/articles/sdata201866) | Africa-wide | Nightlights and imagery for local economic activity | Free |

## Headline findings

**Extreme poverty fell by roughly a billion people, and then stopped falling.** PIP puts the share
below the international line at ~38% in 1990 and under 10% by the late 2010s — the largest and
fastest reduction in material deprivation in recorded history, concentrated in China and then South
and Southeast Asia. Progress stalled around 2019 and reversed during COVID; the remaining poor are
increasingly concentrated in sub-Saharan Africa and in conflict states, where growth-based
approaches work worst.

Worth noting what this measure is and is not. It is consumption from household surveys, converted at
PPP, at a line calibrated to the national poverty lines of the poorest countries. It is sensitive to
PPP revisions in ways that have moved the global count by hundreds of millions overnight, and
Deaton's critique of the survey-to-national-accounts discrepancy — household surveys capture a
shrinking fraction of national-accounts consumption — has never been resolved.

**Cash works, and works better than most alternatives.** The evidence on unconditional cash transfers
is now large and consistent: GiveDirectly's RCTs, Egger et al. (2022) on general-equilibrium spillovers
finding a local fiscal multiplier around 2.5, and Banerjee et al.'s multi-country review finding no
evidence that transfers increase spending on alcohol or tobacco. The 12-year Kenya follow-up work
and the "big push" graduation programmes (Banerjee et al., 2015, six countries) show persistent
effects on assets and consumption. Cash has become the benchmark against which other interventions
must justify their cost — a genuine methodological achievement, because it converted a moral argument
into a cost-effectiveness comparison.

**Deworming is the field's most instructive fight.** Miguel and Kremer (2004) found large school
attendance effects from mass deworming; the Cochrane reviews found little effect on the health
outcomes they prioritised; the reanalysis by Aiken, Davey et al. and the ensuing "worm wars" turned
on coding errors, spillover specification, and — most importantly — which *outcome* counts. Hicks,
Kremer and Miguel's long-run follow-ups find labour-market effects a decade later. Nothing about the
underlying biology was in dispute; the entire fight was about outcome selection and inference. It is
the single best case study in why "the evidence says" is usually an incomplete sentence.

**Micro-credit does much less than promised.** Six RCTs published together in 2015 (*AEJ: Applied*)
found modest business investment effects and essentially no effects on consumption, health,
education or women's empowerment. This is the field working as intended: a large, well-funded,
ideologically popular intervention was tested and substantially deflated.

## The external validity problem

The RCT revolution buys internal validity — within the study, the estimate is unbiased. It buys
nothing about transportability. Deaton and Cartwright's critique is the sharpest statement: a
randomised estimate is a *sample average treatment effect for one population, one implementation,
one context*, and there is no statistical machinery that carries it elsewhere. Pritchett and
Sandefur showed the practical bite — for several standard questions, using a well-identified RCT
estimate from a *different* country gives worse predictions than using a poorly-identified
observational estimate from the *same* country. Rigour and relevance trade off, and the field's
implicit assumption that rigour dominates is not supported.

Related and underappreciated: **site selection is not random**. Allcott's work on scaling shows that
early trial sites are systematically unrepresentative — programmes are first tested where
implementers are enthusiastic and capable — so measured effects shrink on scale-up for reasons that
have nothing to do with the intervention. Vivalt's meta-analysis across hundreds of impact
evaluations finds substantial heterogeneity and a consistent pattern of government-implemented
programmes underperforming NGO-implemented ones.

**Publication bias is present but has been partly addressed.** The AEA registry and pre-analysis
plans have materially improved things — pre-registered trials report smaller and more null effects
than unregistered ones, which is what you would expect if the reform is working. Brodeur et al.'s
z-curve work still shows clear bunching just above conventional significance thresholds across
economics, though less so in RCTs than in IV and DiD papers.

## Wider literature

- **Institutions versus geography versus culture.** Acemoglu, Johnson and Robinson's settler-mortality
  instrument is the most-cited identification strategy in development. Albouy's critique — that the
  mortality data is sparse, inconsistently constructed, and that the result is sensitive to
  reasonable coding choices — is serious and never fully answered. Treat the institutions result as a
  compelling narrative with contested identification, not as settled.
- **Nightlights and satellites.** Henderson, Storeygard and Weil established nightlight luminosity as a
  proxy for local economic activity, which enables subnational analysis where no statistical system
  exists. It has known non-linearities (saturation in cities, blooming, sensor changes across
  satellite generations) that a lot of downstream work ignores.
- **Statistical capacity is itself a variable.** Jerven's *Poor Numbers* documents how thin the
  underlying national-accounts machinery is in much of Africa — Ghana's 2010 rebasing raised measured
  GDP by 60% overnight, Nigeria's 2014 rebasing by 89%. Cross-country growth regressions using these
  series are estimating something, but it is partly the evolution of statistical offices.
- **Migration is the largest measured intervention.** Clemens' "place premium" estimates find wage
  gaps for identical workers across borders that dwarf the effect of any development intervention
  ever trialled — factors of 3 to 10. The New Zealand seasonal-worker lottery (McKenzie and Gibson)
  is a rare randomised estimate and confirms the magnitude. That the field spends vastly more effort
  on interventions with effect sizes two orders of magnitude smaller is a fact about political
  feasibility, not about evidence.

## Honest summary

The RCT movement genuinely raised the evidentiary standard and killed several popular but ineffective
programmes, which is more than most methodological revolutions achieve. Its blind spot is that it
optimised the one form of validity that generalises least. When reading any development claim, the
questions worth asking are: what was the comparison condition, who implemented it, and what is the
argument — not the assumption — that it transports.
