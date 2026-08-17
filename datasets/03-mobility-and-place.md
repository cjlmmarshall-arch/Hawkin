# 03 — Mobility and place

The domain that has benefited most from the shift from surveys to administrative data. Sample sizes
went from thousands to tens of millions, which converted a literature about national averages into a
literature about geography — and geography turns out to be where the variation is.

## The datasets

| Dataset | Coverage | What it is | Access |
|---|---|---|---|
| [Opportunity Atlas](https://www.opportunityatlas.org) | US, ~20m children | Adult outcomes by census tract of childhood | Free (aggregated) |
| [Social Capital Atlas](https://socialcapital.org) | US, 21bn friendships | Facebook-derived connectedness by ZIP/school/college | Free |
| [Opportunity Insights data library](https://opportunityinsights.org/data/) | US | Mobility, college, neighbourhood, COVID economic tracker | Free |
| [PSID](https://psidonline.isr.umich.edu) | US, 1968– , multigenerational | The original income panel | Free |
| [NLSY79 / NLSY97](https://www.bls.gov/nls/) | US cohorts | Labour, education, AFQT | Free |
| [Understanding Society](https://www.understandingsociety.ac.uk) | UK, 40k households | UK household panel, successor to BHPS | Free (UKDS) |
| [Moving to Opportunity](https://www.nber.org/programs-projects/projects-and-centers/moving-opportunity) | 4,600 families, randomised | The housing-voucher RCT | Restricted |
| [Global Database on Intergenerational Mobility](https://www.worldbank.org/en/topic/poverty/brief/what-is-the-global-database-on-intergenerational-mobility-gdim) | 150+ countries | Education/income mobility, cross-country | Free |
| [Statistics Denmark / Nordic registers](https://www.dst.dk/en/TilSalg/forskningsservice) | Full population, multigenerational | The gold standard | Restricted, on-site |

## Headline findings

**Mobility is local.** Chetty, Hendren, Kline and Saez (2014) linked ~40 million US tax records
across generations and found absolute upward mobility varies by a factor of two or more across
commuting zones — a child at the 25th percentile in Salt Lake City reaches roughly the 46th
percentile in adulthood; in Charlotte, roughly the 36th. The national number that the literature had
spent thirty years arguing about turned out to be an average over a distribution nobody had seen.

**And it is causal, at least partly.** The obvious objection is selection: better places have better
parents. Chetty and Hendren (2018) exploit families who move at different child ages and find a
dose-response relationship — each year of childhood spent in a better area contributes
proportionally, which is very hard to generate from pure sorting. The Moving to Opportunity
reanalysis (Chetty, Hendren and Katz, 2016) confirms it experimentally: children who moved before
age 13 had substantially higher adult earnings; those who moved as teenagers did not, or did worse.
Age at exposure is the identifying variation, and it is a genuinely elegant design.

**Economic connectedness beats every other measure of social capital.**
[Chetty et al. (2022, *Nature*)](https://www.nature.com/articles/s41586-022-04996-4) used 21 billion
Facebook friendships covering 84% of US adults aged 25–44 to build three distinct social-capital
measures. Only one predicts mobility: **economic connectedness**, the share of a low-SES person's
friends who are high-SES. Social cohesion (clustering, tight-knittedness) and civic engagement
(volunteering) are essentially unrelated to mobility. The counterfactual: if low-SES children grew
up in counties with the connectedness of the average high-SES child, their adult incomes would be
about **20% higher**.

This is a serious blow to the Putnam-style "bowling alone" reading of social capital, in which what
matters is the density of community ties. The *density* of ties does nothing. The *cross-class
composition* of ties does a great deal. The companion paper decomposes this into exposure (are there
high-SES people around?) and friending bias (do you befriend them when there are?), and finds both
matter roughly equally — which means integration alone is insufficient, because large schools and
neighbourhoods with high exposure often have high friending bias too.

**American mobility is not falling, but it was never high.** Chetty et al. (2017) find absolute
mobility — the share of children out-earning their parents — fell from ~90% for the 1940 cohort to
~50% for the 1980 cohort, driven mostly by slower growth rather than by changing distribution.
Meanwhile *relative* mobility (rank-rank correlations) has been roughly flat since the 1970s. These
two facts are often confused. The US is not becoming less mobile; it is becoming less able to make
everyone richer than their parents by growth alone.

## What I would push back on

The Opportunity Insights programme measures adult income rank conditional on childhood location.
Places that produce high-earning adults score well. Places whose children stay put, near family, in
lower-cost and lower-wage areas score badly — even if those children are doing fine. There is a real
sense in which the Atlas partly measures **out-migration to expensive labour markets**. The
age-at-move design handles the selection objection well; it handles this measurement objection less
well, because moving to a high-wage city is one of the mechanisms.

Second: the social capital results are cross-sectional. The 20% counterfactual is an observational
contrast dressed in causal language, and the paper is more careful about this than its coverage was.
There is no experiment in which anyone's friendship network was randomised.

## Wider literature

- **Nordic registers** show much higher mobility than the US at every margin, with intergenerational
  income elasticities roughly half the US level. But Landersø and Heckman (2017) make the awkward
  point that Denmark's educational mobility is no better than the US — Danish mobility is
  substantially a *tax-and-transfer* achievement compressing the income distribution, not a
  human-capital one. The Great Gatsby Curve (Corak) is consistent with this: mobility correlates
  with inequality across countries, but partly mechanically.
- **Multigenerational persistence is higher than two-generation estimates imply.** Clark's surname
  studies (*The Son Also Rises*) find status persistence across many generations at a rate far above
  what iterating a one-generation elasticity would predict, and remarkably similar across societies
  and eras. The methodology has real problems — surnames are a selected, group-level instrument, and
  the "universal constant" claim is much stronger than the evidence — but the core observation that
  measurement error in single-generation data biases persistence downward is correct and important.
- **Behavioural genetics complicates all of this.** Parent–child correlations in income confound
  transmitted environment with transmitted genotype. Within-family designs and adoption studies
  (Sacerdote; Björklund, Lindahl and Plug) suggest both matter and neither dominates. The polygenic
  score literature (§07) is starting to let people include genetic controls directly, which is
  either the future of mobility research or an enormous new source of confounded regressions,
  depending on how carefully it is done.

## Honest summary

The single most robust finding is the age-at-exposure result: childhood environment causally affects
adult outcomes, roughly linearly in years of exposure. That is as close to settled as this field
gets. The connectedness result is more novel and less identified — I would treat it as an
outstanding descriptive fact in search of an experiment, not as a policy instruction.
