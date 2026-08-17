# 05 — Politics and institutions

The measurement problem in this domain is unusually severe: the outcome variable is a construct
assembled by human coders from qualitative material, and the coders live in the world they are
coding. When V-Dem reports that democracy is declining, it is reporting that expert coders think
democracy is declining, which is a different proposition and correlated with the first in ways
nobody has cleanly identified.

## The datasets

| Dataset | Coverage | What it is | Access |
|---|---|---|---|
| [V-Dem](https://www.v-dem.net) | 202 countries, 1789– , 31m+ data points | ~500 indicators, multiple expert coders per item, IRT-aggregated | Free |
| [Polity5](https://www.systemicpeace.org/inscrdata.html) | 1800– | The older autocracy–democracy scale | Free |
| [Freedom House](https://freedomhouse.org/reports) | 1973– | Political rights and civil liberties scores | Free |
| [CSES](https://cses.org) | 60+ countries, 5 modules | Harmonised post-election surveys | Free |
| [ANES](https://electionstudies.org) | US, 1948– | The American National Election Studies | Free |
| [British Election Study](https://www.britishelectionstudy.com) | UK, 1964– , plus internet panel | Face-to-face + 20+ wave panel | Free |
| [Manifesto Project](https://manifesto-project.wzb.eu) | 1,000+ parties, 1945– | Hand-coded party platform positions | Free |
| [ParlGov](https://www.parlgov.org) | 37 democracies | Parties, elections, cabinets | Free |
| [Chapel Hill Expert Survey](https://www.chesdata.eu) | Europe | Expert placement of parties on policy dimensions | Free |
| [Correlates of War](https://correlatesofwar.org) | 1816– | Interstate conflict, alliances, capabilities | Free |
| [UCDP](https://ucdp.uu.se) | 1946– | Armed conflict and battle deaths | Free |
| [QoG Institute](https://www.gu.se/en/quality-government) | Merged | Aggregator of governance datasets | Free |

## Headline findings

**The third wave of autocratisation.** V-Dem's
[Democracy Report 2025](https://www.v-dem.net/documents/60/V-dem-dr__2025_lowres.pdf) reports that
autocracies now outnumber democracies for the first time in over twenty years — 91 autocracies (56
electoral, 35 closed) against 88 democracies (29 liberal, 59 electoral) — with roughly 72% of the
world's population living under autocracy. The level of democracy for the average world citizen is
back to about 1985. Forty-five countries are in autocratisation episodes against 19 democratising.
Freedom of expression is deteriorating in nearly a quarter of countries, a record over the last 25
years.

**The mechanism changed.** The classic route out of democracy was the coup: fast, visible,
externally punishable. The modern route is incremental and legalistic — executive aggrandisement,
court-packing, media capture, electoral-commission capture — each step individually defensible and
collectively decisive. This is the substantive contribution of Bermeo's "On democratic backsliding"
and of the Levitsky–Ziblatt literature, and V-Dem's disaggregated indicators are what made it
measurable, because a single 0–10 democracy score cannot show you which component moved first.

**Democratisation waves are real but the mechanism is contested.** Modernisation theory (Lipset)
predicts development causes democracy. Przeworski and Limongi's rejoinder — that development does
not cause transitions to democracy but does prevent democracies from dying — is one of the cleanest
"same correlation, different mechanism" results in political science, and it still roughly holds
under V-Dem data.

## Where I would apply pressure

**Expert coding drifts.** V-Dem's methodology is genuinely serious — multiple coders per
country-year-indicator, an item-response model that estimates and corrects for coder thresholds and
reliability, bridge and lateral coders to anchor across countries. It is the best-engineered
solution anyone has to this problem. But the fundamental issue survives good engineering: if the
concept of "free and fair" tightens over time in the minds of the academics doing the coding, the
series declines with no change in the world. Little, Meng and others have argued that
objective indicators — incumbent vote shares, turnover rates, incumbent defeat frequency — show much
less backsliding than subjective ones over the same period. The counter-argument (Knutsen et al.) is
that objective indicators are lagging by construction: an incumbent who has captured the courts
still loses elections until suddenly they don't.

I do not think this dispute is resolved, and I would treat the *magnitude* of measured global
decline as uncertain while treating the *specific country cases* — Hungary, Turkey, India, El
Salvador — as well-evidenced, because those show up on objective indicators too.

**Population-weighting does a lot of work.** "72% of humanity lives under autocracy" is heavily
driven by India's reclassification and China's constancy. Country-weighted and person-weighted
narratives about global democracy diverge substantially, and outlets pick whichever is more
dramatic.

## Wider literature

- **Electoral systems and vote efficiency.** Duverger's law survives as a tendency, not a law. The
  more decision-relevant finding is that under FPTP, seat outcomes depend on the *geographic
  efficiency* of a party's vote — its distribution, not its total. The BES and ParlGov data make this
  computable, and it has direct implications for campaign resource allocation that most campaigns
  ignore in favour of maximising raw vote share. UK 2024 is the extreme case in the modern record: a
  landslide majority on a low vote share, achieved almost entirely through efficiency.
- **Polarisation is asymmetric and mostly affective.** ANES data shows US ideological polarisation on
  policy positions has moved much less than *affective* polarisation — feeling-thermometer ratings of
  the out-party have collapsed. Boxell, Gentzkow and Shapiro's cross-country comparison finds the US
  is an outlier in trend, which cuts against explanations (social media, the internet) that should
  apply everywhere. That is a genuinely underrated result: the most popular explanation for
  polarisation fails a simple placebo test.
- **Manifesto Project coding error.** Mikhaylov, Laver and Benoit showed the hand-coded left–right
  scale carries substantial non-classical measurement error, which attenuates and sometimes reverses
  downstream regressions. Enormous numbers of published results use RILE uncorrected.
- **Democracy and growth.** Acemoglu, Naidu, Restrepo and Robinson (2019) find democratisation raises
  GDP per capita by around 20% over 25 years, using a dichotomous measure and flexible controls for
  dynamics. It is the best-identified estimate available and still rests on 122 transitions, which is
  not many.

## Honest summary

The V-Dem infrastructure is the most impressive measurement project in political science and should
be the default source. Use the disaggregated component indicators rather than the headline indices —
they are where the actual information is, they are less exposed to conceptual drift, and they let you
see *which* institution moved rather than being told that a latent variable declined.
