Project Notes
Data Scope & Limitations

This project uses proxy datasets and seasonal estimates to analyze the economic impact of Detty December.

The data is designed for high-level policy analysis, not for precise financial accounting or operational forecasting.

Revenue and visitor figures represent estimated magnitudes and patterns, rather than audited totals.

Modeling Decisions

A star schema was used to support scalable, time-based analysis:

Fact tables: economic impact and visitor flow

Dimension tables: time and sector

Surrogate keys (time_id, sector_id) were created to ensure consistent aggregation and avoid reliance on text-based joins.

Time attributes (month, year, season) were centralized in the time dimension to prevent duplication and ambiguity.

Data Transformation Approach

Data cleaning and key derivation were performed in Power Query, reflecting common BI workflows.

SQL was used primarily for:

Row-count validation

Join integrity checks

Aggregation verification

Relationships and measures were implemented in Power BI to support interactive analysis.

Interpretation Guidance

Findings should be interpreted as directional insights highlighting seasonal patterns, concentration effects, and relative sector contributions.

Results are intended to inform strategic planning and risk awareness, not to assign fault or evaluate agency performance.

Policy Context

The analysis explicitly considers transport safety and emergency response implications associated with seasonal visitor surges.

Insights are framed to support proactive, data-driven planning, recognizing Detty December as a predictable, recurring event.

Reproducibility

The project structure and documented assumptions allow the analysis to be:

Extended with official transport, health, or emergency response data

Adapted to other cities or seasonal tourism events

Measures and visuals can be updated as more granular or real-time data becomes available.

Author’s Note

This project is intended to demonstrate applied data modeling, analytical reasoning, and policy-oriented insight generation rather than dashboard aesthetics alone.