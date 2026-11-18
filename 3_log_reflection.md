# Step 3, 4 & 5: Audit Table, Confused Classmate Transcript & Reflection
 Step 3: Interpretation Auditor Table (Colour the Claims)
 AI Interpretation Claim | Colour | How Checked | Decision | Reason / Evidence |
 1. "The mean price exceeds the median price for skewed items in the table." | **Green** | Recomputed directly against `summary_stats` in `2_work.ipynb`. | **Accept** | Verified: arithmetic mean is mathematically higher than the 50th percentile when right-skewed outliers exist. |
 2. "Seasonal demand surges likely account for the upper-tail price spikes." | **Amber** | Checked data dictionary for causal/seasonal variables. | **Reject** | Plausible explanation, but no seasonal or demand variables exist in the dataset to verify it. |
3. "Supplier monopolies forced retail prices up by 15% across the region." | **Red** | Checked dataset columns for supplier/market-share data and recomputed % change. | **Reject** | Unverified causal claim referring to external market structure data not present in our file. |
 4. "Removing the highest outlier reduces the mean while leaving the median nearly unchanged." | **Green** | Recomputed mean and median with and without the flagged outlier in Python. | **Accept** | Verified: the median is resistant to extreme single-point changes, whereas the mean shifts directly. |
 Step 4: Confused Classmate Transcript Excerpt
Confused Classmate: "I don't get it—the mean adds up every single price and divides equally, so isn't the mean *always* the most accurate typical price?"
Our Explanation: "Not when there are extreme outliers. Imagine 9 days where bread costs $2, and 1 glitch or shortage day where it costs $22. The mean is ($18 + $22) / 10 = $4.00, even though nobody ever paid $4.00—and 90% of the time they paid $2.00."
Confused Classmate: "But why shouldn't that $22 day count just as much as the other days?"
Our Explanation: "It *does* count if you want total revenue or total spend, which is what the mean measures. However, if a neighbor asks what a 'typical' trip to the store costs, the middle value (the median, $2.00) reflects reality for 9 out of 10 days, whereas the mean gets dragged away from almost every real transaction by one freak spike."
Confused Classmate: "Oh! So the mean gets pulled by extremes, while the median shows the middle shopper's experience."
 Step 5: Reflection
In our first draft, the final sentence claimed that *"corporate price gouging during peak shopping weeks caused these spikes and permanently reduced household purchasing power."* That went far beyond what the data allowed. Our dataset only contains item names, dates, and unit prices—it contains zero information on corporate profit margins, wholesale costs, peak foot traffic, or household income. By labeling that sentence **C (causal claim)**, we recognized that descriptive price numbers can show *what* happened to prices, but cannot prove *why* sellers raised them or how hard households were hurt.
