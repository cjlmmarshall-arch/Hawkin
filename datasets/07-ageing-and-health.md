# 07 — Ageing, longevity and health

The domain with the best data and the worst signal-to-noise in public discussion, because it is
where a genuine scientific literature sits directly adjacent to a commercial one.

## The datasets

| Dataset | Coverage | What it is | Access |
|---|---|---|---|
| [Human Mortality Database](https://www.mortality.org) | 41 countries, some from 1751 | Period and cohort life tables, deaths by single year of age | Free (registration) |
| [International Database on Longevity](https://www.supercentenarians.org) | Validated 105+ | Age-validated supercentenarian records | Free |
| [Global Burden of Disease](https://vizhub.healthdata.org/gbd-results/) | 204 countries, 1990– | DALYs, YLLs, risk-factor attribution | Free |
| [UK Biobank](https://www.ukbiobank.ac.uk) | 500k, aged 40–69 at recruitment | Genotypes, imaging, biomarkers, EHR linkage | Application, fee |
| [All of Us](https://allofus.nih.gov) | 400k+ enrolled, diverse by design | US genomics + EHR + surveys | Application |
| [FinnGen](https://www.finngen.fi) | 500k Finns | Genotype + national registry linkage | Application |
| [HRS](https://hrs.isr.umich.edu) / [ELSA](https://www.elsa-project.ac.uk) / [SHARE](https://share-eric.eu) | US / England / Europe, 50+ | Harmonised ageing panels with biomarkers | Free–low barrier |
| [GWAS Catalog](https://www.ebi.ac.uk/gwas/) | All published associations | The central registry | Free |
| [Interventions Testing Program](https://www.nia.nih.gov/research/dab/interventions-testing-program-itp) | Mice, 3 sites | Rigorously replicated lifespan trials | Free results |
| [Dog Aging Project](https://dogagingproject.org) | 50k+ dogs | Companion-animal ageing cohort, rapamycin trial | Free (curated) |

## Headline findings

**Life-expectancy gains have decelerated in the frontier countries.**
[Olshansky et al. (2024, *Nature Aging*)](https://www.nature.com/articles/s43587-024-00702-3) took HMD
data 1990–2019 for the eight longest-lived populations plus Hong Kong and the US, and found the rate
of improvement slowing markedly. Their projection: survival to 100 is unlikely to exceed ~15% for
women and ~5% for men this century absent interventions that target ageing itself. The argument is
structural — the twentieth century's gains came from crushing infant, infectious and then
cardiovascular mortality, and those wins are largely banked. What remains is senescence, and nothing
in current clinical practice slows it.

**This is contested, and the dissent is credible.** A [2025 rebuttal](https://www.biorxiv.org/content/10.1101/2025.05.01.651310.full.pdf)
argues that life expectancies are still rising and that Olshansky's deceleration is partly an
artefact of the 1990–2019 window, which contains the US opioid and obesity stall, the post-2010
UK/US austerity-era plateau, and cohort effects from twentieth-century smoking. Pick 1970–2000 or
1950–2019 and the picture is less pessimistic. Vaupel's long-standing position — that predicted
ceilings have been broken repeatedly, and that record female life expectancy rose almost perfectly
linearly at ~2.5 years per decade for 160 years — is the strongest single counter-argument, and it
has an excellent track record of embarrassing forecasters.

My read: the deceleration in the 1990–2019 window is real, but attributing it to a biological
ceiling rather than to identifiable and reversible causes (smoking cohorts, obesity, opioids, health
system stagnation) is a stronger claim than the data supports. It is a decomposition problem and
the paper does not decompose.

**The late-life mortality plateau is unresolved.** Whether the force of mortality flattens after
~105 (Barbi et al., 2018, on Italian data — a genuine plateau, implying no fixed lifespan limit) or
continues to rise (Gavrilov, Gavrilova) turns almost entirely on **age validation**. Newman's
demonstration that supercentenarian records cluster in jurisdictions with poor birth registration
and correlate with pension-fraud incentives is the most uncomfortable finding in demography, and it
implies that a substantial fraction of the input data to this debate is wrong. IDL exists precisely
to address this and remains small.

**Genetics of ageing: highly polygenic, modestly predictive.** GWAS on parental lifespan and
healthspan find many small effects; the only large-effect common variant is *APOE*. Heritability of
lifespan from twin and pedigree studies is around 25%, and Ruby et al. (2018) argue even that is
inflated by assortative mating — their Ancestry.com pedigree analysis puts it nearer 10%. That is a
substantial downward revision and it means lifespan is overwhelmingly environmental and stochastic.

**The only robust lifespan interventions in mammals are unglamorous.** The ITP — three sites,
blinded, genetically heterogeneous mice, deliberately designed to kill false positives — has
replicated lifespan extension for **rapamycin** (largest and most consistent), acarbose, 17-α-
estradiol (males only), and canagliflozin. It has *failed* to replicate a long list of famous
candidates including resveratrol, nicotinamide riboside, metformin (as monotherapy in healthy mice),
and most of the supplement shelf. The ITP is the single most valuable dataset in this domain
precisely because it is designed to produce negative results, and it produces them at a high rate.

## Reading UK Biobank honestly

UK Biobank is the most productive dataset in human biology and the most misused. Recruitment
achieved a **~5.5% response rate**; participants are healthier, wealthier, less obese, less likely to
smoke, and have ~50% lower all-cause mortality than the general UK population of the same age.

This matters differently by question type:

- **Genetic association**: mostly fine. Selection is largely orthogonal to genotype, so effect
  estimates hold up reasonably.
- **Prevalence and absolute risk**: unusable without reweighting. The cohort is not the population.
- **Exposure–outcome associations**: dangerous. Collider bias induced by selection on health can
  generate associations of the wrong sign, which is a leading suspect in the "moderate drinking is
  protective" literature. Munafò, Tilling, Taylor, Evans and Davey Smith worked this out formally,
  and it is the single most useful methodological paper for anyone reading biobank epidemiology.

Mendelian randomisation partly rescues this by using genotype as an instrument, but it has its own
failure modes — horizontal pleiotropy, population stratification, and the assortative-mating and
dynastic effects that within-sibship GWAS was designed to expose. Within-family MR estimates are
frequently much smaller than population estimates, which tells you how much confounding was in the
original.

## Wider literature

- **Epigenetic clocks.** Horvath and successors (GrimAge, DunedinPACE) predict mortality better than
  chronological age and are the field's leading candidate biomarker. But they are trained to predict
  age or mortality, so their association with mortality is partly circular, and it is unresolved
  whether they measure a *causal* ageing process or a downstream correlate. If it is the latter,
  intervening to change your clock does nothing, and the clinical-trial programme built on them is
  measuring the wrong endpoint. This is the crux question in the field.
- **Hallmarks of ageing.** López-Otín et al. (2013, updated 2023) is the organising framework —
  twelve hallmarks, from genomic instability to altered intercellular communication. It is a superb
  taxonomy and not a theory: it does not specify which hallmark is upstream, which is what an
  intervention programme needs.
- **Caloric restriction does not transfer cleanly.** Robust in rodents, equivocal in primates — the
  NIA and Wisconsin rhesus studies famously disagreed, and the disagreement traced to what the
  *control* monkeys were fed. CALERIE in humans shows metabolic improvements and a slowed DunedinPACE
  clock, but is far too short to say anything about lifespan.
- **Compression of morbidity is not happening.** Fries predicted illness would compress into a shorter
  terminal window. GBD healthy-life-expectancy data shows healthspan gains lagging lifespan gains
  broadly, so the additional years skew toward disability. This is the most policy-relevant fact in
  the whole domain and the least discussed.

## Honest summary

Human lifespan is not obviously bounded by biology at currently observed levels, but the empirical
case for imminent radical extension is weak, and the honest position on the 1990–2019 deceleration is
that we cannot yet distinguish a ceiling from a bad three decades. The interventions with real
replicated mammalian evidence number about four, and none has a human lifespan trial, because such a
trial would take longer than a career — which is exactly why the biomarker question above matters so
much.
