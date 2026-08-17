# 06 — Culture and values

Culture is the residual that everything unexplained gets attributed to, which makes it both the most
important variable in comparative social science and the least disciplined. The datasets here are
good; the causal inference built on them mostly is not.

## The datasets

| Dataset | Coverage | What it is | Access |
|---|---|---|---|
| [World Values Survey](https://www.worldvaluessurvey.org) | ~120 countries, 7 waves, 1981– | The canonical global values survey | Free |
| [European Values Study](https://europeanvaluesstudy.eu) | Europe, 1981– | WVS's sibling; jointly released | Free |
| [General Social Survey](https://gss.norc.org) | US, 1972– | The deepest single-country attitude series | Free |
| [ISSP](https://issp.org) | 40+ countries, 1985– | Rotating thematic modules | Free |
| [Pew Global Attitudes](https://www.pewresearch.org/global/) | Rotating | High-quality cross-national attitude data | Free |
| [Google Books Ngrams](https://books.google.com/ngrams) | 1500–2019, 8 languages | Word frequency over ~5% of all books printed | Free |
| [Ethnographic Atlas / D-PLACE](https://d-place.org) | 1,400 pre-industrial societies | Murdock's ethnographic codes, cleaned | Free |
| [Hofstede / GLOBE](https://geerthofstede.com/research-and-vsm/dimensions-data-matrix/) | 100ish countries | Cultural dimensions from employee/manager surveys | Free |
| [Moral Machine](https://www.moralmachine.net) | 40m decisions, 233 countries | Global variation in trolley-problem intuitions | Free |

## Headline findings

**Two dimensions organise most cross-national value variation.** Inglehart and Welzel's factor
analysis of WVS items recovers a stable two-dimensional structure: *traditional versus
secular-rational* (deference to religion, parental authority, national pride) and *survival versus
self-expression* (economic and physical security versus tolerance, autonomy, quality of life). The
resulting cultural map clusters countries into recognisable civilisational groups — Protestant
Europe, Catholic Europe, Confucian, Latin American, African-Islamic, English-speaking — and those
clusters have been remarkably stable across seven waves.

**Development moves societies diagonally.** Countries getting richer tend to travel from the
lower-left (poor, traditional, survival-oriented) toward the upper-right. The Inglehart thesis is
that existential security is the driver: people raised without scarcity develop post-materialist
priorities, and because formative values are set young, the change is largely *cohort replacement*
rather than individual updating. This has a strong testable implication — value change should be
slow, ratchet-like, and predictable from age structure — and it broadly holds.

**But path dependence dominates.** The clusters do not converge as they move. Protestant Europe and
Confucian Asia are both high on secular-rational values, and both have got richer, but they have not
converged on each other; the whole map slides without collapsing. Cultural inheritance survives
enormous economic change, which is the single most important finding here and the one that most
resists a simple modernisation story.

## Where the causal claims get weak

The Inglehart mechanism is identified almost entirely off cross-country and cross-cohort
correlation. Development, secularisation and self-expression move together everywhere, so the data
cannot easily separate "development causes value change" from "a common third factor causes both"
from "values cause development" — which is exactly the direction the cultural-economics literature
below argues for. Welzel's *Freedom Rising* pushes the causal claim hardest and is correspondingly
most exposed.

Two further problems specific to WVS:

- **Translation and response style.** Acquiescence bias and extreme-response style vary
  systematically by country, and a meaningful part of the "cultural" variance in Likert items is
  response style rather than content. Anchoring vignettes fix this and are almost never used.
- **The map's dimensions are partly artefacts of item selection.** Change the item battery and the
  factor structure shifts. Two robust dimensions emerging from a battery chosen by researchers who
  expected two dimensions is weaker evidence than it appears.

## Wider literature

- **Cultural economics has found instruments, with mixed success.** Nunn and Wantchekon use historical
  slave-raiding intensity to explain contemporary low trust in Africa; Alesina, Giuliano and Nunn use
  historical plough suitability to explain gender-role attitudes; Giuliano and Nunn use historical
  climate variability to explain the strength of tradition itself. These are ingenious, and they all
  share the same vulnerability: any historical instrument can affect present outcomes through
  channels other than culture (institutions, disease, trade), and the exclusion restriction is
  asserted rather than tested. Kelly's critique — that many of these results are driven by spatial
  autocorrelation, and that the instruments predict outcomes about as well as *randomly generated
  spatial noise* does — is the most serious methodological challenge in the field and has not been
  adequately answered.
- **Epidemiological approach.** The strongest identification comes from comparing second-generation
  immigrants from different origins facing the same institutions (Fernández and Fogli on fertility
  and female labour supply). Origin-country culture predicts behaviour decades after migration. This
  is the cleanest evidence that culture is a real, transmissible, and economically consequential
  variable, and it does not require a historical instrument.
- **WEIRD samples.** Henrich, Heine and Norenzayan (2010) showed the behavioural-science evidence base
  was drawn overwhelmingly from Western, Educated, Industrialised, Rich, Democratic populations, and
  that these populations are outliers on many measured dimensions — fairness in economic games,
  visual illusions, analytic reasoning, moral reasoning. Its most-cited empirical support, the
  cross-cultural ultimatum-game literature, is thinner than the claim, but the core point stands and
  the field has genuinely changed in response.
- **Ngrams needs care.** Corpus composition changes drastically over time — the scientific literature
  balloons after 1900, and OCR quality varies — so raw frequency trends confound "what people wrote"
  with "what got digitised". Pechenick, Danforth and Dodds document this thoroughly. Most viral
  Ngrams charts are composition effects.
- **Secularisation is not universal.** The classic thesis predicted religion would decline with
  development everywhere. Norris and Inglehart's revision — that secularisation is real within
  developed countries but globally offset by differential fertility between religious and secular
  populations — is a rare case of a theory being amended rather than abandoned in response to data,
  and the amendment is holding up.

## Honest summary

WVS is excellent descriptive infrastructure and weak causal infrastructure. Use it to establish that
values differ, cluster, and change slowly along predictable dimensions. Do not use it, or the
historical-instrument literature built on it, to establish that culture caused any particular
economic outcome — for that, the second-generation immigrant designs are the only ones I would put
real weight on.
