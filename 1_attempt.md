Step 1: Initial Attempt (Draft Referee's Note & Metric Selection)
 Commit Snapshot Hash
 Metric Selection Rationale (Teaching Data)
Item A (Stable Staple, e.g., Milk): Report the mean and first-to-last percentage change. The distribution shows no extreme outliers, so the mean accurately reflects typical price levels alongside overall directional growth.
Item B (Skewed/Volatile Item, e.g., Fresh Produce): Report the median. Occasional extreme price spikes skew the mean upward, making the median a much better representation of what a shopper typically pays.
Flagged Value Impact (Week 2 Cleaned File)
With Flagged Outlier: The mean price is pulled noticeably higher than the median, exaggerating perceived inflation.
Without Flagged Outlier: Removing or correcting the flagged outlier brings the mean closely in line with the median, proving that the apparent price jump was driven by a single extreme data anomaly rather than a broad price increase across all dates.
 Draft Referee's Note (Labeled O / E / C)
[O] Across the observed period in our teaching dataset, the mean price of the staple item rose higher than its median price. [O] Specifically, while the median price remained steady across most recorded dates, a small cluster of extreme high-price observations pulled the arithmetic mean upward. [E] One possible explanation for this gap is temporary, localized supply bottlenecks or seasonal stock shortages that caused brief price spikes without altering baseline pricing. [O] When comparing the first and last recorded dates, the overall percentage change shows a moderate net increase. [C] Ultimately, corporate price gouging during peak shopping weeks caused these spikes and permanently reduced household purchasing power.
