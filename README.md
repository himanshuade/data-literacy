# Data Literacy

Coursework from **Data Literacy (MATHS 7105)**, part of my Master of Data Science at the University of Adelaide (Trimester 1, 2024).

The course is about the judgement side of data work: how data is collected, how the same numbers can be framed to tell opposite stories, and how to spot charts that mislead. These three assignments are written reports rather than code.

| # | Topic | What I did |
|---|-------|------------|
| 1 | [Survey design and research ethics](assignment-1-survey-design) | Critiqued a flawed experiment and redesigned it using sampling principles |
| 2 | [Data storytelling and spin](assignment-2-data-storytelling) | Built a deliberately one-sided analysis for a political party, then took it apart with honest charts |
| 3 | [Media critique](assignment-3-media-critique) | Identified what two real Fox News charts get right and wrong |

**Skills:** survey and sampling design, research ethics (APA code), data visualisation, chart critique, communicating findings, Excel

---

## Assignment 1: Survey design and research ethics

**Brief:** analyse the "ESP experiment" scene from *Ghostbusters* as if it were a real study of *the effect of negative reinforcement on ESP ability*.

I identified three problems:

- **Credibility of the data.** The interviewer misreports answers, telling one participant he's wrong when he's right and praising the other when she's wrong, so the recorded data is biased at the source.
- **Selective discrimination.** Only one participant is ever penalised, which breaches the APA ethics code and makes the two conditions incomparable.
- **No informed consent.** Participants weren't told the purpose of the study, the penalties involved, or that they could withdraw.

I then proposed a redesigned study built on the elements of the sampling problem (Scheaffer, Mendenhall & Ott): clear objectives and consent, a defined target population and sampling frame, a fixed sample design, identical and unbiased measurement for every participant, and trained field workers.

📄 [`a1_survey_design.pdf`](assignment-1-survey-design/a1_survey_design.pdf)

## Assignment 2: Data storytelling and spin

**Brief:** acting as an analyst for the opposition (Party B), use a fictional country's economic data to argue against the governing Party A. Then show the honest version of the same data.

**Part 1, the spin.** I chose three pairs of indicators and framed each to make Party A look bad, with headlines to match:

- GDP growth vs. happiness: *"GDP soars while citizens' happiness plummets"*
- Education spending vs. unemployment: *"A failed investment in lowering unemployment"*
- Population vs. budget surplus: *"Population growth strains surplus"*

**Part 2, the reality.** I re-plotted the same indicators without manipulation and compared both parties' terms. The honest charts largely reverse the story:

- GDP growth and happiness are positively related.
- Unemployment fell as Party A's education spending rose. Party B spent more than twice as much on education with weaker employment results.
- Party A managed the budget surplus more effectively.

I closed with data-driven recommendations for Party B, covering economic policy, tracking performance against spending, and transparent budgeting.

📄 [`a2_party_b_data_analysis.pdf`](assignment-2-data-storytelling/a2_party_b_data_analysis.pdf) · 📊 [`data/gdp_vs_happiness.xlsx`](assignment-2-data-storytelling/data/gdp_vs_happiness.xlsx)

## Assignment 3: Media critique

I critiqued two Fox News graphics featured on [FlowingData](https://flowingdata.com), listing what each does well and what misleads.

**Unemployment line chart**
- ✅ Labelled data points, a cited source, and labelled axes
- ❌ The y-axis starts at 8% instead of 0, which exaggerates small changes
- ❌ The plotted points are out of proportion: 8.8 appears lower than 8.6
- ❌ Clashing saturated reds and blues, and a loaded title

**2012 GOP candidates pie chart**
- ✅ Labelled segments with percentages, and a title
- ❌ The slices add up to **193%**, so a pie chart is the wrong form
- ❌ The 3D effect makes the 60% slice look bigger than the 70% slice
- ❌ A red/green/blue palette that's hard for colour-blind viewers to read
- ❌ The source is just "Opinions", with no sample size

📄 [`a3_critique_fox_news_line_chart.pdf`](assignment-3-media-critique/a3_critique_fox_news_line_chart.pdf) · 📄 [`a3_critique_fox_news_pie_chart.pdf`](assignment-3-media-critique/a3_critique_fox_news_pie_chart.pdf)

---

## Repository structure

```
data-literacy/
├── assignment-1-survey-design/
│   └── a1_survey_design.pdf
├── assignment-2-data-storytelling/
│   ├── a2_party_b_data_analysis.pdf
│   └── data/gdp_vs_happiness.xlsx
└── assignment-3-media-critique/
    ├── a3_critique_fox_news_line_chart.pdf
    └── a3_critique_fox_news_pie_chart.pdf
```

The Assignment 2 data comes from a fictional country supplied with the course. The charts in Assignment 3 belong to their original publishers and are reproduced here for critique.
