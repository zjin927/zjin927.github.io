---
layout: post
title:  "San Francisco 311 Complaints: Citywide Trends and Street Cleaning Focus"
date:   2025-05-13
categories: [San Francisco, 311 Complaints] 
---

## Motivation

San Francisco’s 311 service receives a huge volume of non-emergency complaints from residents each year. In just the last year and a half, over one million issues were reported via 311[^1]. Analyzing this data is important because it helps us understand what problems residents face most often and how the city can respond. Common complaints revolve around cleanliness (trash, illegal dumping) and maintenance (graffiti) – core issues that affect daily quality of life. By examining when, where, and what people complain about, we can identify patterns and opportunities for city agencies to improve services.

Why analyze 311 complaints?
- Identify Key Issues: Determine which complaint categories (e.g. trash, graffiti, noise) are most frequent, indicating where city services are most needed.
- Improve Resource Allocation: Understand temporal trends (by day or season) to deploy crews and resources when and where they’re most required.
- Measure Responsiveness: Track how quickly complaints get resolved, highlighting any service delays or backlogs that need attention.
- Community Insights: Highlight neighborhood problem hotspots, helping officials and residents collaborate on targeted solutions.

Overall, diving into 311 data allows a data-driven approach to cleaner and safer streets. In the sections below, we present an analysis following a “martini glass” narrative: starting with a broad overview of all complaints, then narrowing to an in-depth focus on one prominent issue – Street and Sidewalk Cleaning – to uncover deeper insights.

## Initial Exploration

Our first step is an exploratory overview of the 311 complaints to understand the big picture. We looked at the distribution of cases across different complaint categories, the variation by day of week, and the seasonal trends throughout the year. 

![Group by Categories](/assets/plots/group_by_categories.png)

(Visualization 1: Street & Sidewalk Cleaning tops all other categories, followed by graffiti and parking enforcement.)

**Complaints by Category**: The data covers a wide range of complaint types, but a few categories dominate. As shown in Visualization 1, Street & Sidewalk Cleaning complaints are the most frequent, accounting for a large share of all 311 requests (on the order of about 39.23% of complaints). This category includes reports of trash on streets, sidewalk litter, and illegal dumping, which are persistent challenges in San Francisco. Following that, Graffiti and Parking Enfrocement are also major contributors. Together, these cleanliness-related issues make up a significant portion of complaints, underscoring citywide concerns with cleanliness and maintenance. Other categories such as homeless encampments, abandoned vehicles, and MUNI feedbacks form the remaining share, but individually they occur far less often than the top issues. 

![Group by Categories](/assets/plots/group_by_weekday.png)

(Visualization 2: Reports peak early in the week — especially Mondays — and drop during weekends.)

**Weekly Trend**: Complaints are logged every day of the week, but there is a noticeable weekly rhythm. **We observe in Visualization 2 that weekdays see slightly more reports than weekends**. In fact, Monday tends to be the peak day for 311 requests, whereas Sundays see the fewest reports. This pattern makes intuitive sense: some issues accumulate over the weekend and get reported at the start of the week, and residents may be less inclined to contact services on a Sunday. Overall, the differences are moderate – people report issues consistently through the week – but understanding these peaks can help schedule city response teams effectively (for example, having more staff on duty to handle the Monday-Tuesday influx of complaints). 

![Group by Categories](/assets/plots/group_by_month.png)

(Visualization 3: Street & Sidewalk Cleaning complaints rise in summer and peak during fall.)

**Seasonal Trend**: Visualization 3 shows the monthly distribution of complaints across the top 10 categories. One category stands out: Street and Sidewalk Cleaning, which dominates both in volume and seasonal variation.
- Street and Sidewalk Cleaning shows a clear seasonal pattern, with fewer complaints in winter and early spring, and a steady rise through summer, peaking around August to October. This pattern likely reflects increased street activity, tourism, and post-summer cleanup needs.
- Other categories such as Graffiti, Encampments, and Parking Enforcement remain relatively stable throughout the year, showing minor fluctuations but no strong seasonal trends.
- Categories like Abandoned Vehicles, Tree Maintenance, and Sewer Issues also display mild variation, possibly influenced by weather or public awareness campaigns.

These patterns suggest that while some services must be maintained consistently year-round, others—particularly cleaning operations—require seasonal scaling. Preparing for higher demand in late summer and early fall can help improve service responsiveness and resident satisfaction. We identified Street and Sidewalk Cleaning as a critical area to explore further. This category stood out as the top issue and one that significantly impacts residents’ quality of life. Next, we dive deeper into what the data reveals about these specific complaints.

## Deep Dive into Street and Sidewalk Cleaning

Street and Sidewalk Cleaning issues include things like overflowing trash cans, loose garbage on streets, illegal dumping of large items, and general litter on public right-of-ways. We chose to focus on this category because it **represents a substantial portion of all 311 complaints** (the single largest category in our data) and shows an interesting seasonal pattern. Clean streets are vital for public health and neighborhood pride, yet San Francisco has struggled with this issue – for example, reports of illegal dumping and loose trash have **skyrocketed in recent years (quadrupling over the past decade)**[^1], indicating a growing challenge.

Focusing our analysis here allows us to uncover specific insights: **How quickly are these cleaning requests addressed? Where in the city are these problems most concentrated?** And can we discover patterns or clusters among different areas of the city in terms of their street cleaning issues? By drilling down on one category, we can provide targeted findings that might help Public Works and other agencies improve street cleanliness.

### Response Time Analysis

One critical aspect of 311 service requests is how long it takes for the city to respond or resolve the issue. For Street & Sidewalk Cleaning complaints, timely response is important – trash left on the street not only looks bad but can attract pests or create hazards. The city’s official goal is to address 95% of street cleaning requests within 48 hours[^2]. In practice, however, performance has been under that target in recent years, likely due to staffing shortages and the sheer volume of reports.

![Group by Categories](/assets/plots/street_monthly_response_time.png)

(Visualization 4: Average monthly response times from 2008 to 2024 (in hours).)

Visualization 4 above shows the monthly average response time (in hours) for Street and Sidewalk Cleaning complaints from 2008 to 2024. From 2008 to 2012, average response times were generally stable, staying below 300 hours. In **2012**, there was a dramatic spike, with average response time exceeding **2,000 hours** (~83 days). This likely reflects a data anomaly, backlog clearance, or system changes. From **2014 onward**, response times **gradually decreased** and became more consistent. And **from 2016 to 2017**, it fluctuated between 250 to 1000 hours, indicating a potential issue with staffing or communication. Since **2020**, performance has **significantly improved**, with average response time often staying below **100 hours** (~4 days), and in recent years, even dropping closer to 24–48 hours.

Longer response times can negatively impact neighborhoods – trash left on sidewalks for extended periods can spread or attract more dumping. The city has acknowledged these challenges, noting that they have been falling short of their **48-hour response target since 2021**. This analysis underlines the need for improved response strategies: perhaps better dispatch of crews, increased staffing or overtime during peak complaint days, or community programs to prevent dumping in the first place. Reducing the average resolution time would directly improve cleanliness on the streets.

### Geographic Distribution

Another key question is where these street cleaning complaints are happening. Are they evenly spread across San Francisco, or are certain neighborhoods disproportionately affected? We analyzed the data by police district (each police district roughly corresponds to a set of neighborhoods) to see the geographic patterns of Street & Sidewalk Cleaning requests. 

![Group by Categories](/assets/plots/street_group_by_pd.png)

(Visualization 5: Complaint totals by police district. Mission leads by a large margin.)

**District Hotspots**: Visualization 5 shows the total number of complaints per district. **Mission** district stands out as the clear hotspot, with over **500,000 complaints**, far exceeding all other areas. Other high-complaint districts include **Northern**, **Central**, and **Bayview** — all densely populated and heavily trafficked zones. **Tenderloin** also appears among the lower half of the chart, but still has a noticeable number of reports, consistent with known sanitation challenges in the area. **Park**, **Taraval**, and **Richmond** — primarily residential neighborhoods in the western part of the city — report significantly fewer complaints. These areas tend to have lower population density and fewer high-traffic commercial corridors, which may contribute to better street conditions or fewer reports. This geographic breakdown highlights how urban density, foot traffic, and land use are closely tied to street cleanliness issues. City services may benefit from area-specific strategies — such as increased cleaning frequency in downtown zones or public awareness efforts in mixed-use neighborhoods.

Visualization 6 below shows a choropleth view of Street & Sidewalk Cleaning complaints by Police District in San Francisco:

<div style="width: 100%; overflow: auto;">
  <iframe src="{{ '/assets/maps/street_group_by_pd_map.html' | relative_url }}" width="740" height="370" style="border:none;"></iframe>
</div>

(Visualization 6: Interactive map of street cleaning complaints by police district. The darker the color, the more complaints there are in that district.)

**Complaint Density Map**: Visualization 6 clearly shows that complaint hotspots are concentrated in the central and eastern districts, particularly:
- Mission
- Northern
- Central
- Bayview

These areas are dense, mixed-use, and experience higher levels of foot traffic, commercial activity, and illegal dumping, all of which likely contribute to elevated complaint levels.

In contrast, western and southwestern districts (e.g., Park, Richmond, Taraval) show much lower complaint densities. These are primarily residential zones with lower population density and fewer commercial waste issues.

Visualization 7 below is an interactive visualization of monthly complaint trends for the five districts with the most Street and Sidewalk Cleaning complaints:

<div style="width: 100%; overflow: auto;">
  <iframe src="{{ '/assets/bokeh/street_top_5_pd_by_complaints_trend_bokeh.html' | relative_url }}" width="740" height="370" style="border:none;"></iframe>
</div>

(Visualization 7: Top 5 districts by Street & Sidewalk Cleaning complaints. Mission shows the most rapid and sustained growth.)

**Top 5 Problem Districts**: We can see from Visualization 6 that **Mission District** (in red) consistently shows the **highest volume of complaints** — peaking around 2021 with nearly **7,000 reports in a single month**. **Central**, **Bayview**, and **Northern** follow, each showing significant growth since 2015. **Ingleside** lags slightly behind, but still trends upward, especially after 2020.

The chart highlights a widening gap over time:
- Complaint counts across these top districts have more than quadrupled from 2010 to 2024.
- The Mission District alone far exceeds others, signaling sustained pressure on cleaning services.
- Seasonal peaks and pandemic-related spikes are also visible, suggesting shifting community needs.

These five districts account for a **large share of all street cleaning complaints citywide**. Many are in or near the **urban core**, with dense housing, transit hubs, and in some cases industrial zones — all contributing to greater waste accumulation and reporting activity.

To improve service equity and efficiency, the city may consider:
- Allocating more cleaning resources to top districts during peak seasons.
- Deploying targeted anti-dumping programs (e.g., Bayview industrial areas)
- Investigating root causes such as insufficient public trash bins or enforcement gaps

### Clustering Analysis

To dig deeper into the patterns across districts, we applied a clustering analysis on the Street & Sidewalk Cleaning complaint data. The idea was to group similar districts together and see if distinct profiles emerge – for instance, are there clusters of districts that behave similarly in terms of their street cleaning issues (either in volume or average response time)? We used K-Means clustering to classify the districts based on their complaint patterns (such as the number of complaints per month in each district). To determine a suitable number of clusters, we performed a silhouette analysis. 

![Group by Categories](/assets/plots/silhouette_score.png)

(Visualization 8: Highest silhouette score achieved at k = 5, indicating optimal clustering.)

**Choosing Clusters**: Visualization 8 above shows the silhouette score for different number of clusters (k=2 to 9). The silhouette score measures how similar an object is to its own cluster compared to other clusters (values range from -1 to 1, where higher is better). The **highest score** was achieved at **k = 5**, suggesting that five clusters offer the most meaningful and well-separated grouping. Based on this analysis, we used **k = 5** in our final clustering model.

Using K-Means clustering, we analyzed Street and Sidewalk Cleaning complaints across San Francisco's Police Districts. Five distinct clusters emerged, highlighting patterns in complaint volume and response efficiency.

We then visualized the clusters on a city map (in the project, an interactive map highlights each district’s cluster). 

<div style="width: 100%; overflow: auto;">
  <iframe src="{{ '/assets/maps/street_sfpd_clustering_map.html' | relative_url }}" width="740" height="370" style="border:none;"></iframe>
</div>

(Visualization 9: Each district is colored by cluster label, representing complaint and response patterns.)

So, what do these clusters in Visualization 9 represent? After examining the members of each cluster, we found a logical interpretation:

| Cluster  | Description | Districts | Complaints | Response Time |
| **0** | High volume, moderate response | Northern, Central, Bayview, Ingleside | High | Moderate (~120 hrs)|
| **1** | Moderate volume, quick response | Richmond, Taraval, Park | Medium | Fast (~100 hrs)|
| **2** | Extreme hotspot | Mission | Very High | Moderate (~124 hrs)|
| **3** | Low volume, slow response | Tenderloin | Low | Slow (~152 hrs)|
| **4** | Severe delays | Southern | Medium | Very Slow (~187 hrs)
|

This spatial clustering reveals patterns not just in how many complaints districts receive, but in how quickly they are addressed:
- Cluster 2 (Mission) is a major hotspot with extreme complaint volume, requiring targeted support and scalable response strategies.
- Cluster 4 (Southern) has an average complaint load but the worst delays, suggesting possible resource shortages or inefficiencies.
- Cluster 1 (Richmond, Taraval, Park) performs best — with lower complaint levels and quicker resolution — a potential model for other areas.
- Tenderloin stands out in Cluster 3, where even with fewer reports, response times are significantly slower. This may reflect deeper service access or execution issues.

## Conclusion

In this project, we analyzed San Francisco’s 311 complaints to uncover both broad trends and focused insights on street cleanliness issues:
- Citywide Patterns: We saw that a few categories (especially Street & Sidewalk Cleaning) account for a large portion of complaints. Issues like trash, illegal dumping, and graffiti are at the forefront of residents’ concerns. Complaint volumes aren’t static; they vary by time – spiking on early weekdays. This knowledge can help city agencies anticipate when demand for services will be highest.
- Street Cleaning Focus: By zooming in on Street and Sidewalk Cleaning requests, we highlighted a crucial city service challenge. These complaints are not being resolved as fast as the city aims for (often taking longer than the 48-hour goal on average), pointing to possible resource constraints or process inefficiencies. Geographically, the problem is concentrated: downtown and surrounding districts bear the brunt of dirty streets and sidewalks, while outer neighborhoods see relatively few complaints. This suggests targeted interventions – more cleaning crews and anti-dumping enforcement in hotspots like the Mission, Tenderloin, and Southern could make a big difference.
- Clustering Insights: Using clustering, we discovered that districts naturally fall into groups. This reinforces the idea that a targeted, cluster-specific approach is appropriate – the city might prioritize cluster 3 and 4 areas for intensive cleaning programs, while maintaining cluster 0, 1 with routine services. It also helps in benchmarking: cluster 1 districts set a standard that others could strive for, whereas high-complaint districts could be paired with similar ones to share best practices or resources.

What could be improved or explored further? This analysis opens up several avenues for future work:
- Integrate Population & Foot Traffic: Adjust complaint rates by neighborhood population or daily visitors to understand if high complaints are simply due to more people or if certain areas truly have disproportionately more issues.
- Predictive Analysis: Use time-series forecasting or machine learning to predict spikes in 311 complaints (e.g., before events or weather changes) so that the city can preemptively deploy resources.
- Broader Category Deep-Dives: We focused on street cleaning, but a similar deep dive into other prevalent issues (like graffiti or homeless encampment reports) could yield insights specific to those domains. Each category might have its own patterns and challenges.
- Response Outcome Analysis: Examine how many complaints actually get resolved within the target time and identify bottlenecks. For instance, are certain districts consistently missing the 48-hour goal? Understanding why (staffing, access issues, etc.) could help improve service levels.
- Community Engagement: Overlay 311 data with community factors – for example, do areas with active neighborhood associations have different reporting patterns or faster cleanups? Engaging local communities in the worst-hit areas (through awareness campaigns or volunteer cleanups) could complement city efforts.

In summary, analyzing 311 complaints provides valuable insights for urban management. By following the data from a high-level overview down to a focused story on street cleaning, we found clear evidence of where the city is doing well and where it needs to “clean up” its act. The hope is that these findings can guide smarter allocation of city services, making San Francisco’s streets cleaner and its government more responsive to the people it serves.

## References
[^1]: [S.F. 311 received more than a million calls since start of 2022. Here are the most common complaints](https://www.sfchronicle.com/bayarea/article/311-service-hotline-complaints-18166457.php)
[^2]: [Cleaner sidewalks and streets in the Tenderloin](https://www.sf.gov/data--cleaner-sidewalks-and-streets-tenderloin)