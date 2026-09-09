# Readings

A curated list of readings about data science as a practice — how it actually gets done,
where it goes wrong, and what it does to the people in the data. It is a work in progress.

For practical how-to material (Python, `pandas`, `git`, visualization tutorials, cheat
sheets), see the companion [Resources](https://github.com/COGS108/Resources) repo.

**New here?** Start with [What is the question?](#thinking-carefully-with-data),
[Tidy Data](#data-and-data-organization), and
[Ten simple rules for responsible big data research](#ethics-and-accountability).

**A note on access.** Most entries link to a freely readable copy. Entries tagged
*(UCSD access)* are paywalled — sign in through the [UCSD Library](https://library.ucsd.edu/)
or the campus VPN to read them. Entries tagged *(book)* are worth requesting through the
library if you don't want to buy them.

---

## Contents

**Papers and essays**
- [Foundational](#foundational)
- [How Data Science Actually Gets Done](#how-data-science-actually-gets-done)
- [Data and Data Organization](#data-and-data-organization)
- [Thinking Carefully With Data](#thinking-carefully-with-data)
- [Ethics and Accountability](#ethics-and-accountability)
- [Privacy, Anonymity, and Consent](#privacy-anonymity-and-consent)
- [Computing Practices](#computing-practices)
- [Visualization](#visualization)
- [Communicating Results](#communicating-results)
- [Machine Learning and Generative AI](#machine-learning-and-generative-ai)

**Longer reads and ongoing sources**
- [Books and Course Notes](#books-and-course-notes)
- [Blogs and Newsletters](#blogs-and-newsletters)
- [Journals and Venues](#journals-and-venues)
- [Contributing](#contributing)

---

## Foundational

- **[50 Years of Data Science](https://www.tandfonline.com/doi/full/10.1080/10618600.2017.1384734)** — Donoho (*JCGS*, 2017). Traces where "data science" came from and argues for what the field would look like if it took its own science seriously; the standard starting point for the "is this just statistics?" debate. *(UCSD access)*
- **[Exploratory Data Analysis](https://archive.org/details/exploratorydataa00tuke_0)** — Tukey (1977). The book that made looking hard at your data — before modeling it — a respectable activity; skim the early chapters for the mindset rather than the hand-computation methods. *(book · free to borrow)*
- **[Statistical Modeling: The Two Cultures](https://projecteuclid.org/journals/statistical-science/volume-16/issue-3/Statistical-Modeling--The-Two-Cultures-with-comments-and-a/10.1214/ss/1009213726.full)** — Breiman (*Statistical Science*, 2001). The essay that named the split between modeling data to explain it and modeling it to predict; published with commentary from statisticians who disagreed. *(open access)*

## How Data Science Actually Gets Done

- **[How Data Science Workers Work with Data](https://dl.acm.org/doi/10.1145/3290605.3300356)** — Muller et al. (*CHI*, 2019). Interview study showing that practitioners don't "find" data so much as actively construct it through discovery, capture, curation, and design. *(UCSD access)*
- **["Everyone wants to do the model work, not the data work"](https://dl.acm.org/doi/10.1145/3411764.3445518)** — Sambasivan et al. (*CHI*, 2021). How undervaluing data collection produces "data cascades" — small upstream problems that compound into downstream failures in deployed systems. *([free author PDF](https://www.shivanikapania.com/assets/chi2021paper.pdf))*

## Data and Data Organization

- **[Tidy Data](https://vita.had.co.nz/papers/tidy-data.pdf)** — Wickham (*JSS*, 2014). One variable per column, one observation per row, one table per unit of observation — and why every downstream step gets easier when you do that first. *(open access)*
- **[Data Organization in Spreadsheets](https://www.tandfonline.com/doi/full/10.1080/00031305.2017.1375989)** — Broman & Woo (*The American Statistician*, 2018). Concrete rules for the spreadsheet stage that most data still passes through; the [companion tutorial](https://kbroman.org/dataorg/) is free and equally useful. *(UCSD access)*
- **[Datasheets for Datasets](https://arxiv.org/abs/1803.09010)** — Gebru et al. (*CACM*, 2021). Proposes documenting every dataset's motivation, collection process, and intended uses; a useful checklist for describing your own project data. *(open access)*
- **["Raw Data" Is an Oxymoron](https://direct.mit.edu/books/edited-volume/3992/Raw-Data-Is-an-Oxymoron)** — Gitelman, ed. (MIT Press, 2013). Essay collection on the central point that data is always collected by someone, for some purpose, and never arrives raw; the [introduction](https://direct.mit.edu/books/edited-volume/3992/chapter/166409/Introduction) is freely readable. *(book)*

## Thinking Carefully With Data

- **[What is the question?](https://www.science.org/doi/10.1126/science.aaa6146)** — Leek & Peng (*Science*, 2015). Two pages arguing that the most common error in data analysis is mistaking which of six question types you're actually asking. *(UCSD access)*
- **[Many analysts, one data set](https://journals.sagepub.com/doi/10.1177/2515245917747646)** — Silberzahn et al. (*AMPPS*, 2018). Twenty-nine teams analyzed the same data on referee bias and got a wide spread of effect sizes; the clearest demonstration that analytic choices are results. *(open access)*
- **[The Garden of Forking Paths](https://sites.stat.columbia.edu/gelman/research/unpublished/p_hacking.pdf)** — Gelman & Loken (working paper, 2013). Why a researcher can inflate false-positive rates without ever running multiple tests — the choices you *would have* made on other data are enough. *(open access)*
- **[Why Most Published Research Findings Are False](https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.0020124)** — Ioannidis (*PLOS Medicine*, 2005). The paper that kicked off the replication crisis: how power, bias, and the number of hypotheses tested determine whether a published claim is likely true. *(open access)*
- **[The ASA Statement on p-Values](https://www.tandfonline.com/doi/full/10.1080/00031305.2016.1154108)** — Wasserstein & Lazar (*The American Statistician*, 2016). The American Statistical Association's six principles on what a p-value does and does not tell you. *(open access)*
- **[Measurement and Fairness](https://arxiv.org/abs/1912.05511)** — Jacobs & Wallach (*FAccT*, 2021). Recasts fairness disputes as measurement problems: the gap between the abstract thing you care about and the variable you actually recorded. *(open access)*
- **[Measurement Schmeasurement](https://journals.sagepub.com/doi/10.1177/2515245920952393)** — Flake & Fried (*AMPPS*, 2020). Names the questionable measurement practices that quietly invalidate a study, and the questions to ask to avoid them. *(open access)*
- **[Calling Bullshit](https://www.callingbullshit.org/)** — Bergstrom & West (2020). Book and full course site — syllabus, case studies, and videos — on spotting misleading data claims without needing to re-do the analysis. *(book · free course site)*

## Ethics and Accountability

- **[Ten simple rules for responsible big data research](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005399)** — Zook et al. (*PLOS Comp Bio*, 2017). Ten concrete commitments — data are people, privacy is contextual, guard against reidentification — that translate directly into project decisions. *(open access)*
- **[Dissecting racial bias in an algorithm used to manage the health of populations](https://www.science.org/doi/10.1126/science.aax2342)** — Obermeyer et al. (*Science*, 2019). A widely deployed algorithm used health costs as a proxy for health need, and thereby understated the illness of Black patients; the canonical example of a biased target variable. *(UCSD access)*
- **[Gender Shades](https://proceedings.mlr.press/v81/buolamwini18a.html)** — Buolamwini & Gebru (*FAT\**, 2018). Audit of commercial gender classifiers showing error rates near zero for lighter-skinned men and above 30% for darker-skinned women — aggregate accuracy hides everything. *(open access)*
- **[Model Cards for Model Reporting](https://arxiv.org/abs/1810.03993)** — Mitchell et al. (*FAT\**, 2019). Companion to Datasheets: report model performance disaggregated by group, alongside intended use and known limitations. *(open access)*
- **[Data Feminism](https://data-feminism.mitpress.mit.edu/)** — D'Ignazio & Klein (MIT Press, 2020). How power decides what gets counted, by whom, and for whose benefit; the full text is free online. *(free book)*
- **[Weapons of Math Destruction](https://www.penguinrandomhouse.com/books/241363/weapons-of-math-destruction-by-cathy-oneil/)** — O'Neil (2016). Case studies of opaque scoring systems — teacher evaluation, credit, policing, college rankings — that scale harm while appearing objective. *(book)*
- **[Automating Inequality](https://virginia-eubanks.com/automating-inequality/)** — Eubanks (2018). Ethnographic account of what automated eligibility, prediction, and ranking systems do to poor and working-class people who cannot opt out. *(book)*

## Privacy, Anonymity, and Consent

- **[Robust De-anonymization of Large Sparse Datasets](https://www.cs.cornell.edu/~shmat/shmat_oak08netflix.pdf)** — Narayanan & Shmatikov (*IEEE S&P*, 2008). Re-identified Netflix Prize users from a little outside knowledge; the reason "we removed the names" is not a privacy plan. *(open access)*
- **[Differential Privacy: A Primer for a Non-Technical Audience](https://scholar.harvard.edu/files/salil/files/differential_privacy_primer_nontechnical_audience.pdf)** — Wood et al. (2018). Plain-language explanation of what differential privacy guarantees, what it costs, and what it doesn't do. *(open access)*
- **[Differential Perspectives: Epistemic Disconnects Surrounding the US Census Bureau's Use of Differential Privacy](https://privacytools.seas.harvard.edu/publications/differential-perspectives-epistemic-disconnects-surrounding-us-census)** — boyd & Sarathy (*HDSR*, 2022). Why the 2020 Census privacy fight was not really a technical disagreement — data users and privacy engineers hold incompatible ideas of what census data *is*. *(open access)*

## Computing Practices

- **[Good Enough Practices in Scientific Computing](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510)** — Wilson et al. (*PLOS Comp Bio*, 2017). The realistic baseline: data management, project organization, version control, and collaboration habits any researcher can adopt this week. *(open access)*
- **[Best Practices for Scientific Computing](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745)** — Wilson et al. (*PLOS Biology*, 2014). The more ambitious companion piece: write for people first, automate repetition, test, and don't optimize before you measure. *(open access)*
- **[Software development skills for data scientists](http://treycausey.com/software_dev_skills.html)** — Causey (2015). The five habits — modular code, documentation, version control, testing, logging — that separate analysis scripts from code other people can use. *(blog)*
- **[PEP 8 — Style Guide for Python Code](https://peps.python.org/pep-0008/)** — van Rossum, Warsaw & Coghlan. The conventions that make Python readable to other Python programmers; skim it once, then let a linter enforce it. *(docs)*

## Visualization

- **[The Grammar of Graphics](https://link.springer.com/book/10.1007/0-387-28695-0)** — Wilkinson (2nd ed., 2005). The formal system underneath `ggplot2`, `plotnine`, and most modern plotting APIs: charts as compositions of data, scales, and geometry rather than a menu of chart types. *(book · UCSD access)*
- **[Graphical Perception: Theory, Experimentation, and Application](http://euclid.psych.yorku.ca/www/psy6135/papers/ClevelandMcGill1984.pdf)** — Cleveland & McGill (*JASA*, 1984). The experiments that ranked how accurately people read position, length, angle, and area — the empirical reason to prefer bars over pies. *(open access)*
- **[The Science of Visual Data Communication: What Works](https://journals.sagepub.com/doi/10.1177/15291006211051956)** — Franconeri, Padilla, Shah, Zacks & Hullman (*PSPI*, 2021). Book-length review of what the perception and cognition literature actually supports about chart design. *(UCSD access)*
- **[Same Stats, Different Graphs](https://www.research.autodesk.com/publications/same-stats-different-graphs/)** — Matejka & Fitzmaurice (*CHI*, 2017). The Datasaurus: datasets with identical summary statistics and wildly different shapes. *(open access)*
- **[Fundamentals of Data Visualization](https://clauswilke.com/dataviz/)** — Wilke (2019). Free, figure-heavy book on why some charts work and others mislead. *(free book)*
- **[How Charts Lie](https://wwnorton.com/books/9781324001560)** — Cairo (2019). How to read charts skeptically — misleading scales, dubious aggregation, and the ways a technically accurate figure still deceives. *(book)*

## Communicating Results

- **[Points of View: Storytelling](https://www.nature.com/articles/nmeth.2571)** — Krzywinski & Cairo (*Nature Methods*, 2013). One page on relating your data to the world your reader already knows. *(UCSD access)*
- **[Ten Simple Rules for Better Figures](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003833)** — Rougier, Droettboom & Bourne (*PLOS Comp Bio*, 2014). Practical rules for figures that carry an argument: know your audience, pick colormaps deliberately, don't mislead. *(open access)*

## Machine Learning and Generative AI

- **[Leakage and the reproducibility crisis in ML-based science](https://arxiv.org/abs/2207.07048)** — Kapoor & Narayanan (*Patterns*, 2023). Catalogs eight kinds of leakage found across 329 papers in 17 fields, with model info sheets for catching them before publication. *(open access)*
- **[Depths of learning](https://www.nature.com/articles/s41567-018-0098-8)** — Buchanan (*Nature Physics*, 2018). Short column on adversarial examples: imperceptible changes to an input can flip a network's prediction, and detection schemes keep getting evaded. *(UCSD access)*
- **[On the Dangers of Stochastic Parrots](https://dl.acm.org/doi/10.1145/3442188.3445922)** — Bender, Gebru, McMillan-Major & Mitchell (*FAccT*, 2021). The costs of ever-larger language models — environmental, documentation, and the harms of training on unvetted web text. *(open access)*
- **[What Should Data Science Education Do with Large Language Models?](https://hdsr.mitpress.mit.edu/pub/pqiufdew)** — Tu, Zou, Su & Zhang (*HDSR*, 2024). Argues the data scientist's role shifts toward problem formulation and validation when the code comes cheap, and what that means for how the field is taught. *(open access)*

## Books and Course Notes

Books listed in the topic sections above aren't repeated here.

- **[Data Science from Scratch](https://library.ucsd.edu/news-events/oreilly-for-higher-education/)** — Grus (2nd ed., 2019). Builds the tools from first principles instead of calling a library you don't understand yet; the harder book, and you'll grow a lot working through it. Free through your UCSD login via O'Reilly for Higher Education. *(book · UCSD access)*
- **[Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/)** — VanderPlas (2nd ed., 2023). Short and to the point on NumPy, `pandas`, matplotlib, and scikit-learn; text and [code](https://github.com/jakevdp/PythonDataScienceHandbook) are both free. *(free book)*
- **[Probability and Statistics for Data Science](https://cims.nyu.edu/~cfgranda/pages/stuff/probability_stats_for_DS.pdf)** — Fernandez-Granda (NYU, 2017). Full lecture notes from NYU's Center for Data Science: probability through hypothesis testing and regression, with the math written out. *(free notes)*

## Blogs and Newsletters

- **[Better Explained](https://betterexplained.com)** — Intuition-first explainers for the math that underlies data science. *(blog)*
- **[Simply Statistics](https://simplystatistics.org)** — Irizarry, Leek & Peng on statistics, data science, and how academic research works. *(blog)*
- **[Datawrapper Blog](https://blog.datawrapper.de/)** — Data-visualization writing with great worked examples; the "what to consider when" posts are excellent (and used in lecture). *(blog)*
- **[Statistical Modeling, Causal Inference, and Social Science](https://statmodeling.stat.columbia.edu/)** — Gelman's long-running blog; where statistical claims in the news get taken apart. *(blog)*
- **[Simon Willison's Weblog](https://simonwillison.net/)** — Close, practical tracking of what LLM tooling can and can't do, from someone who builds with it daily. *(blog)*

## Journals and Venues

- **[Harvard Data Science Review](https://hdsr.mitpress.mit.edu/)** — Open-access journal aimed at "everything data science and data science for everyone"; the most readable venue on this list. *(open access)*
- **[Journal of Open Source Software](https://joss.theoj.org/about)** — Publishes short papers about research software, making tool-building citable work. *(open access)*
- **[Scientific Data](https://www.nature.com/sdata/)** — Nature journal for descriptions of reusable datasets; good models for documenting data. *(open access)*
- **[GigaScience](https://academic.oup.com/gigascience)** — Publishes large-scale data, the code that produced it, and the analyses together. *(open access)*
- **[Distill](https://distill.pub/about/)** — Archive of exceptionally clear interactive machine-learning explainers; the journal ran 2016–2021 and is on indefinite hiatus, but the back catalog is still some of the best explanatory writing in the field. *(archive)*

## Contributing

Suggestions welcome — especially from students. If a link is dead, a citation is wrong, or
something you read for this course belongs here, open an issue or a pull request.

When adding an entry, please match the existing format:

```markdown
- **[Title](https://example.com)** — Author(s) (*Venue*, Year). One or two lines on what it
  argues and why someone in COGS 108 should read it. *(tag)*
```

Tags in use: *open access*, *UCSD access*, *book*, *free book*, *free notes*, *blog*,
*docs*, *archive*.
