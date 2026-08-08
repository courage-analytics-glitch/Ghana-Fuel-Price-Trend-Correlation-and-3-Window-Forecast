# Ghana Fuel Price Analysis: Comprehensive Insights, Risks, and Forecast

**Prepared by Richard Courage Cobbinah**

Sources: National Petroleum Authority pricing windows, Chamber of Bulk Oil Distributors (CBOD) and Chamber of Oil Marketing Companies (COMAC) market outlook reports, EIA/World of Statistics Brent crude data, exchange-rates.org and TheGlobalEconomy.com cedi/USD data. Full source list and pull dates on the dashboard's Sources page.

---

## Dashboard Structure

Six pages, 30+ visuals, built from 12 core datasets: `brent_crude`, `cedi_usd`, `local_pump_price`, `combined_trend`, `correlation_matrix`, `current_momentum`, `forecast` / `forecast_v2`, `taxes_and_levies`, `omc_uppf_margins`, `price_floors`, `levy_margin_share`, `subsidy_events`, plus `price_composition_full`, `product_consumption_share`, and `price_buildup_funnel` added during the deeper build-out.

---

## Page 1: Trend Snapshot

**Charts:** "5-Year Trend: Crude, Currency, and Pump Price" (line), "Correlation Matrix: What Drives What" (matrix), "Year-on-Year % Change by Driver" (clustered column), "Cedi Movement vs. Petrol Price Movement" (scatter), plus 4 cards (Petrol 5Y, Diesel 5Y, Cedi 5Y, Brent 5Y) and a year slicer.

**Deep insight.** 2022 stands alone in this dataset: petrol rose 76.9% and diesel 93.6%, far outpacing the 48.3% cedi depreciation and 40.9% Brent increase that year. This is a compounding effect, when crude and currency move against Ghana simultaneously, local prices don't simply add the two shocks, they compound through the price build-up mechanism. The correlation matrix confirms the structural relationship behind this: petrol and diesel move almost identically to each other (1.00, expected, since both price off the same regulatory formula), and both track Brent (0.80, 0.86) and the cedi (0.79, 0.75) at meaningfully similar strength, no single input dominates.

**Caution.** These are 5 annual data points, not a long time series. The correlation coefficients are directionally reliable, not statistically robust in the way a 20+ year dataset would be.

**Risk.** The 2022 configuration, rising Brent plus a weakening cedi, is present again in 2026 (Brent +11.64% over the past month, cedi weakening over 6 months). The scatter chart makes this relationship visible point by point rather than as a single summary number.

**Opportunity.** Periods of cedi strength (like most of 2025) are the government's best window to build fiscal buffers before the next compounding shock, not a signal to relax fuel-cost policy.

**Recommendation.** Track Brent and the cedi together monthly using the year slicer to isolate specific periods; a simultaneous adverse move in both is the single highest-risk configuration in this dataset.

---

## Page 2: Forecast

**Charts:** "3-Window Forecast: Petrol, Diesel, and Intervention Scenario" (line), "Projected Window-on-Window Growth Rate" (line), "Diesel Savings Under a Repeated Margin Cut" (column), plus 3 cards (Petrol Forecast, Diesel Forecast, Intervention Savings) and a window slicer.

**Deep insight.** Petrol is projected to rise approximately 4.7% per pricing window and diesel 6.1%, reaching roughly GH¢16.67/L and GH¢17.90/L by the third window out. Diesel's higher elasticity to both Brent (1.41 vs. petrol's 1.07) and the cedi (1.09 vs. 0.93) means it consistently overshoots petrol in any rising-cost environment, with broader knock-on effects since diesel powers freight, agriculture, and industrial generation.

**Caution for users and stakeholders.** This is a momentum-and-elasticity projection built on 5 annual data points, not an econometric model. Treat the direction (both products rising, diesel outpacing petrol) as reliable. Treat the exact GH¢ figures as illustrative scenarios, actual pricing-window outcomes depend on policy decisions not fully predictable from historical elasticity.

**Risk.** Without intervention, diesel-dependent sectors face a compounding cost increase exceeding 18% across three pricing windows, roughly six weeks.

**Opportunity.** The intervention-savings chart quantifies exactly what a repeated margin cut is worth (GH¢0.54/L by Window +3), a concrete, defensible number for either side of a policy debate on whether to renew the relief measure.

**Recommendation.** Diesel-heavy operators (logistics, generators, agriculture) should build Window +2 and Window +3 scenarios into short-term cost planning now, using the window slicer to isolate each scenario individually.

---

## Page 3: Price Build-Up

**Charts:** "What Makes Up the GH¢2.90 Tax Component" (bar), "BOST vs. UPPF/OMC Margin Split" (bar), plus cards for Total Taxes, Total Margins, Total Burden, and Petrol/Diesel/LPG Total Price, and a product slicer.

**Deep insight.** The Energy Sector Levy (GH¢1.00/litre, introduced mid-2025) is the single largest named component in the entire tax structure, larger than any other levy and larger than the entire BOST Margin. Across products, the same GH¢2.90 tax and GH¢1.37 margin apply per litre to petrol and diesel; LPG's tax and margin burden, estimated at GH¢0.99 and GH¢0.47 respectively from its share-of-price data, is proportionally lower in absolute terms but a larger share of its lower per-unit price.

**Caution.** The "Other levies" and "UPPF/OMC margins" aggregate lines represent real money (GH¢0.47/L and GH¢1.25/L) not broken down by individual component in public reporting. The LPG split specifically is derived, not independently published, flagged as such in the source data.

**Risk.** A price build-up this weighted toward fixed levies means pump prices carry a floor that doesn't fall even if crude prices do, taxes alone would represent a growing share of pump price in a genuinely low-crude scenario.

**Opportunity.** The fixed levy structure gives government predictable per-litre tax revenue regardless of crude price swings, a fiscal planning advantage during volatile periods.

**Recommendation.** Track the Energy Sector Levy specifically given its size; it functions as a de facto pricing lever despite being framed as a fixed levy. Use the product slicer to compare the three products' total build-up side by side.

---

## Page 4: Relief Impact

**Charts:** "Tax and Margin Share of Pump Price, Before and After Relief" (column), "Relief Impact by Product" (line), "National Consumption Share: Petrol, Diesel, LPG" (donut), plus cards for Petrol/Diesel/LPG Share Change, and a window slicer.

**Deep insight.** The April 2026 relief measure measurably worked: diesel's combined tax, levy, and margin share of pump price fell from 24.26% to 13.93%, a 10.33 percentage point drop, far larger than petrol's move in the same window. This was a targeted intervention, not a blanket one, consistent with diesel's outsized economic footprint. The donut chart shows petrol dominates national consumption volume (49.35%), diesel follows (36.11%), with LPG a distant third (5.27%), though this measures volume share, not policy priority.

**Caution for stakeholders.** The donut chart mixes measurement units (litres for petrol/diesel, kilograms for LPG) and reflects national average consumption, not cost-weighted household burden. LPG's small volume share doesn't diminish its policy importance for clean cooking and household energy transition goals.

**Risk.** A relief measure this targeted, if not renewed, creates sharp reversal risk, the 10.33pp gain could snap back in a single pricing window once the intervention lapses.

**Opportunity.** Given petrol's dominant consumption share versus diesel's larger relief measure, there's a data-backed case for either a proportionally larger petrol intervention (maximizing consumers reached) or continuing the diesel-first approach (minimizing broader freight/food cost pass-through), a genuine policy tradeoff visible in this data.

**Recommendation.** Any future relief measure should specify and publish its expected duration; the absence of a stated end date undermines the proactive planning recommended on Page 2. Use the window slicer to compare any two windows directly as new pricing data becomes available.

---

## Page 5: Current Prices

**Charts:** "Price Floor by Pricing Window" (column), "Price Floor Trend, Continuous View" (line), "Confirmed Pricing Interventions, 2015-2026" (table), "Petrol Price Build-Up: From Base Cost to Pump Price" (funnel), plus cards for Latest Petrol, Latest Diesel, Diesel Peak to Latest Change, and LPG Total (reused from Page 3), and a window slicer.

**Deep insight.** The funnel chart's internal consistency, base cost (GH¢10.26) plus margins (GH¢1.37) plus taxes (GH¢2.90) landing exactly on the published GH¢14.53 floor, validates the price composition methodology used across the entire dashboard. This is a working accuracy check, not just a visual.

**Caution.** The most recent price floor reflects the active August 2026 diesel-only margin cut, an explicitly one-month measure. Read this figure alongside the subsidy events table, not in isolation, or the temporary relief-driven price could be mistaken for a new baseline.

**Risk.** Absent renewal, diesel could revert toward its pre-intervention level in the next pricing window, a reversal not visible from the price chart alone without the events table beside it.

**Opportunity.** The funnel format is a clearer public communication tool than a single opaque pump price number, showing exactly where a price increase originates: crude, currency, or a specific levy.

**Recommendation.** Pair every published price floor with an explicit note on whether an active relief measure is embedded, and its expected end date. Use the window slicer to isolate any single pricing window and see its full context (floor price, funnel breakdown, and nearby events) together.

---

## Sources Page

A full table of all 12+ datasets with source and pull date, plus the methodology summary covering the key findings, forecast direction, relief-measure pattern, and the primary recommendation, formalizing intervention duration and renewal criteria.

---

## Overall Forecast Summary

Ghana's fuel price trajectory into the next three pricing windows is upward, driven by the same combination, rising Brent plus a weakening cedi, that produced 2022's outsized spike, though currently at a smaller scale. Diesel will consistently outpace petrol given its higher elasticity to both inputs, with broader economic effects through freight, food, and industrial costs. Government has a proven, twice-used tool (targeted margin cuts) that measurably reduces the tax/margin burden without a blanket tax cut, but its ad hoc, undated nature limits its value as a planning input. The single highest-value recommendation across this entire analysis: formalize relief-measure duration and renewal criteria, converting a reactive tool into a predictable one for businesses, consumers, and policymakers alike.

---

This report is for informational purposes only and does not constitute financial, investment, or trading advice.
