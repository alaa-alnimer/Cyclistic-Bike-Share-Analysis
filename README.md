# Cyclistic-Bike-Share-Analysis: Converting Casual Riders to Members
Google Data Analytics Capstone: SQL + Tableau analysis of Cyclistic bike-share ridership.

Google Data Analytics Professional Certificate — Capstone Case Study

Business Task

The goal behind analyzing 12 months of Cyclistic's trip data was to answer the business question of how casual riders and annual members use Cyclistic bikes differently, and how that can inform a marketing strategy to convert casual riders into members. The data reveals that members primarily use the bikes for weekday commuting, while casual riders ride more on weekends and for significantly longer durations (~29 minutes).

Data Source

Source: Divvy trip data, Sept 2025–Aug 2026 (12 months, ~6.1M rows)

Tools used: PostgreSQL, Tableau Public

Data Cleaning (Process)

29 rows had invalid durations (end time before or equal to start time) — removed

5,285 rides exceeded 24 hours — removed

~21–22% of rows had null station names — kept (mostly electric/dockless bikes)

293 anomalous classic-bike rows had null end data — noted, not removed

Final cleaned dataset: 6,110,555 rows

Key Findings

Overall ride duration — casual riders' rides average ~48% longer than members'.

Day of week — members ride most on weekdays; casual riders ride most on weekends.

Duration by bike type — casual riders stand out with an average ride of ~29 minutes on classic bikes.

Hour of day — members show sharp peaks at commuting hours (8am and 5pm); casual riders show one broad afternoon peak.

<img width="527" height="881" alt="Screenshot 2026-09-30 134742" src="https://github.com/user-attachments/assets/b98432b8-91fd-4fee-93b5-21a2b3f111a4" />
<img width="1447" height="867" alt="Screenshot 2026-09-30 132133" src="https://github.com/user-attachments/assets/e466737d-b650-4e7a-a151-dee065d9e88b" />
<img width="850" height="897" alt="Screenshot 2026-09-30 132419" src="https://github.com/user-attachments/assets/4837605e-a856-42a1-99df-27e791abbc60" />
<img width="1230" height="880" alt="Screenshot 2026-09-30 132512" src="https://github.com/user-attachments/assets/581c4b1d-3db2-4aa1-8ac0-d4e1ca2d9c34" />

Visualization

[🔗 View the full interactive dashboard on Tableau Public](https://public.tableau.com/views/Cyclistic_Case_Study_17906912042890/CyclisticBike-ShareMembervsCasualRiderAnalysis?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

Recommendations (Act)
1. Day of Week

Finding: Members ride more frequently on weekdays (Mon–Thu) and least on Sunday. Casual riders show the opposite pattern — riding most on Fri–Sun and least on weekdays.

Insight: This pattern suggests members ride mostly for commuting to work, while casual riders ride more on weekends for leisure and recreational activities.

Recommendation: Offer casual riders discounted or free rides for riding more frequently on weekdays. Riding more could also earn them points redeemable toward a membership subscription.

2. Hour of Day

Finding: Members ride most frequently at 8am and 5pm (commuting hours) and least at midnight. Casual riders ride most between 12pm and 5pm, without the sharp commuting-hour spikes seen in member ridership.

Insight: This suggests members ride more during work commute hours, while casual ridership rises from midday onward — likely reflecting leisure activity rather than a need to commute early.

Recommendation: Offer discounted rides and points to casual riders who ride between 8–11am and 5–7pm, redeemable toward a membership subscription.

3. Ride Duration by Bike Type

Finding: Casual riders average the longest ride duration on classic bikes (~29 minutes) and electric bikes (~14 minutes). Members show less variation — averaging ~14 minutes on classic bikes and ~11 minutes on electric bikes.

Insight: This suggests members ride primarily for commuting (shorter, consistent durations), while casual riders ride more for leisure and sightseeing, reflected in their longer average ride times.

Recommendation: Offer casual riders double points for rides over 20 minutes, since casual riders' classic-bike rides average ~29 minutes. Points are redeemable only with a membership subscription.

Conclusion

The analysis showed that casual riders ride more than members on weekends, while members ride more on weekdays. It also showed that casual riders average longer ride durations — ~29 minutes on classic bikes and ~14 minutes on electric bikes — while members average around 13 minutes across both bike types. Members' ridership peaks at commuting hours (8am and 5pm), while casual riders show a single broad peak in the early afternoon. These patterns informed three recommendations aimed at converting casual riders into annual members.

Data provided by Divvy / Motivate International Inc., under Lyft Bikes and Scooters, LLC's data license agreement.
