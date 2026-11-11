# US Health Insurance: Did the ACA Actually Move the Needle?

A Power BI dashboard looking at how the uninsured rate changed across US states after the Affordable Care Act, and whether Medicaid expansion made a real difference.

![Dashboard preview](images/dashboard.png)

## Why I built this

The ACA is one of those topics everyone has an opinion on, but I wanted to see what the state-level numbers say. Some states expanded Medicaid and some didn't, so it works almost like a natural comparison. I wanted to know:

- Which states saw the biggest drop in uninsured residents
- Whether expansion states did better than non-expansion states
- Where Medicaid enrollment grew the most
- How marketplace enrollment lines up with tax credits

## What I found

**The starting point.** In 2010, before the ACA took effect, the average uninsured rate across states was 14.15%. Medicaid enrollment grew by about 16.11M overall, and around 9M people received marketplace tax credits averaging $292.16 a month.

**Expansion helped, but it wasn't the whole story.** About 63% of states expanded Medicaid and 37% didn't. Expansion states cut their uninsured rate by roughly 6 points on average, compared with about 4.7 in non-expansion states. That's a clear gap, but non-expansion states still improved, so the marketplace and tax credits were clearly doing some of the work.

**Texas was the surprise.** It had the biggest drop in uninsured residents by a wide margin (around 1.8M, more than three times the next state), even though it never expanded Medicaid. A lot of that comes down to population size and marketplace sign-ups. It's a good reminder that raw counts favor big states, while rates favor small ones, so you need both to tell the story fairly.

**More enrollees doesn't mean bigger tax credits.** Most states sit between $200 and $400 in average credits no matter how many people enrolled. The few outliers are probably high-premium markets and would be worth a closer look.

## What this suggests

- Medicaid expansion looks like the strongest single lever for cutting the uninsured rate
- Non-expansion states shouldn't be written off, because enrollment help and subsidies clearly work there too
- Outreach in large states gives the biggest return in absolute numbers
- Any scorecard should show rates and headcounts side by side

## How it's built

- **Tool:** Power BI
- **Data prep:** Power Query for cleaning and shaping the state-level data
- **Modeling:** DAX measures for the KPIs (average uninsured rate, tax credits, Medicaid growth) and the expansion vs. non-expansion comparison
- **Visuals:** filled map, ranked bar charts, donut for the expansion split, clustered bars, and a scatter plot of enrollees vs. tax credit

## Data

Source: *add your dataset link here*

State-level figures on uninsured rates, Medicaid enrollment, marketplace enrollment, tax credits, and expansion status.

## Files

```
├── US_Health_Insurance.pbix
├── data/
├── images/
└── README.md
```

## Limitations

This is state-level, observational data. It shows that expansion states improved more, but it can't prove expansion was the only cause. Population size, existing coverage levels, and local insurance markets all play a part.

## About me

I'm Rocket (Sokunbi Victor Oluwaseun), a data analyst working with Power BI, Excel, and Python. This is part of my #PowerBIPortfolioSeries.

Feel free to reach out on [LinkedIn](https://www.linkedin.com/in/victor-sokunbi-26217a22b/).
