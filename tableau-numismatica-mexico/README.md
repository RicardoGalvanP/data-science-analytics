# Numismática México: Sales Analysis and Data Storytelling (Tableau)

## Version

- Interactive story on Tableau Public: [Equipo13_Reto_Etapa4-4](https://public.tableau.com/app/profile/ricardo.galvan.paez/viz/Equipo13_Reto_Etapa4-4/Stories)
- Static copy: [`story.pdf`](story.pdf)

## Problem Statement

Numismática México sells numismatic products (coins, banknotes and collector folders) through marketplace channels. Year-end events bring its largest revenue, so the marketing director needs a data-backed commercial strategy for November and December: which days and products matter most, where the sales come from, how delivery times behave, and what role advertising plays.

This is a team project (Team 13) from the Data Visualization course of the M.Sc. in Applied Artificial Intelligence. It had four stages: understand the case and the data, build visualizations, design a dashboard, and define a strategy supported by data storytelling. This repository covers the last stage, the story.

My contribution: My contribution: I built several of the visualizations and wrote the data story: the captions and key findings, plus additional charts created specifically to support each point of the narrative.

Team: Team 13.

## Dataset

Provided by the course as part of the case: an Excel file with a sales table (transaction ID, listing title, sales channel, carrier, advertising flag, destination postal code, state and municipality, sale / shipping / delivery dates, units, unit price, marketplace fee and shipping cost) and a product catalog. The data covers September 2021 to September 2022.

The measure used in the story is net sales: product income minus the marketplace fee and taxes. It is not profit, because there is no cost or advertising-spend data. The data is not included in this repository.

## Tech Stack

Tableau Public (calculated fields, filter actions, map, trend lines, Stories).

## Methodology

- Explored the sales and product tables and defined the business questions: seasonality, top products, geography, advertising effect.
- Built a monthly view that highlights November and December against the rest of the period.
- Ranked products by net sales and measured how concentrated the revenue is (Pareto).
- Mapped sales by state, and linked the product chart to the map and trend charts with filter actions so each product can be inspected.
- Compared sales with and without advertising over time, with linear trend lines.
- Wrote a captioned story that goes from seasonality to concentration, geography and advertising.

## Key Findings

- **Seasonality.** November and December 2021 brought about $106K of roughly $388K in net sales (27%) over the 13 months in the data. Evenly spread, two months would be 15%.
- **Concentration.** Five products (out of 2,350+ in the catalog) generate about 80% of net sales ($310K). The leader, a folder of commemorative 5, 10 and 40 peso coins and banknotes, sells about $128K.
- **Geography.** Estado de México ($55.8K), Distrito Federal ($44.9K) and Jalisco ($31.7K) lead the Top 5's sales.
- **Advertising.** Ad-attributed sales rose from about $10K in April to $21K in August 2022, while non-ad sales moved between $6K and $13K. For one product (Carpeta Escudo Nacional) total monthly sales stayed near $4.5K from May to August while the ad-attributed share grew, which is also consistent with ads capturing sales that would have happened anyway.

## Limitations

- Only one holiday season is observed (Nov-Dec 2021), so seasonality cannot be separated from growth or from advertising campaigns.
- Net sales are not profit, and there is no advertising spend, so the return on ads cannot be computed. The ad-versus-organic comparison shows association, not cause.
- Geographic totals are not adjusted for population, so the weight of the central states may partly reflect where more people live.
- Maps filtered to a single product with the advertising flag show only that part of the sales, not the product's total demand.
- The Top 5 is computed over the whole period, while the brief asked to focus on November and December.

## What I Learned

- Every caption in a story must be traceable to what the chart shows in that exact filter state; filter actions change a chart's content, and the title should say so.
- Define the metric precisely (net sales, not profit) and name it that way in every chart.
- A concentration finding (80% of revenue from five products) is both a strength and a risk, and it should lead to concrete actions, such as protecting stock and advertising for those products.
- A rising line for ad-attributed sales does not prove that advertising works; the total, the spend and an organic baseline are needed to tell.
- One season of data supports a hypothesis about seasonality, not a conclusion.

## About

Ricardo Galván Páez, Mechatronics Engineer and Software Support Engineer (WMS/OMS, SQL), studying the M.Sc. in Applied Artificial Intelligence at Tecnológico de Monterrey. This project was built as part of that program.

[GitHub](https://github.com/RicardoGalvanP) · [LinkedIn](https://www.linkedin.com/in/ricardo-galvan-paez)
