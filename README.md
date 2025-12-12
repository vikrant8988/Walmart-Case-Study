# Walmart Black Friday Customer Purchase Behavior Analysis 

### Business Problem  
Walmart wanted to deeply understand who spends how much during Black Friday and why — specifically:  
- Are there significant differences in average purchase amount across Gender, Age, Marital Status, and City Category?  
- Which customer segments drive the majority of revenue?  
- How can we use these insights to improve targeting, inventory planning, and promotional strategies?

### What I Did (Tools & Techniques)  
- **Programming Language**: Python  
- **Core Libraries Used**:  
  - pandas → data loading, cleaning, grouping & aggregation  
  - numpy → numerical computations  
  - scipy.stats → two-sample independent t-tests & confidence intervals  
  - matplotlib + seaborn → exploratory visualizations (count plots, box plots, distribution plots)  
- **Statistical Methods Applied**:  
  - Descriptive statistics (mean, median, count by segment)  
  - Hypothesis testing (t-test for Gender difference)  
  - 95% Confidence intervals for average purchase per segment  
  - Segmentation analysis (Age, City Category, Marital Status, Occupation)

### Key Numbers & Impact  
| Segment                  | % of Transactions | Avg Purchase Amount | Total Revenue Contribution (approx.) |
|--------------------------|-------------------|----------------------|---------------------------------------|
| Male                     | 75.3%             | ₹9,437               | ~75–78% of total sales               |
| Female                   | 24.7%             | ₹8,734               | ~22–25% of total sales               |
| Age 26–35                | 39.9%             | ₹9,250               | Highest volume + highest spend       |
| City Category C          | 31.2%             | ₹9,711               | Highest average ticket               |
| City Category B          | 42.3%             | ₹9,152               | Largest volume                       |
| City Category A          | 26.5%             | ₹8,911               | Lowest average ticket                |
| Unmarried customers      | 58%               | ₹9,266               | Slightly higher than married         |

**Statistical Significance**  
- Male vs Female spending difference: t-stat = 44.84, p-value ≈ 0 → **highly significant**  
- 95% CI shows males spend ₹650–₹750 more per transaction on average

### Key Insights  
1. **Men dominate Black Friday** — both in number of shoppers and amount spent per trip.  
2. **26–35 age group is the sweet spot** — highest footfall + highest average spend.  
3. **City Category C customers have the highest purchasing power** despite fewer people than City B.  
4. Product Categories 1, 5 & 8 together account for ~60% of total sales.  
5. Certain occupations (4, 7, 0, 17) consistently spend 15–25% above average.

### Business Recommendations  
1. **Primary Targeting** → Males | 26–35 years | living in City C & B → allocate 60–70% of Black Friday marketing budget here.  
2. **Inventory Strategy** → Over-stock Product Categories 1, 5, 8 in City C & B stores; reduce depth in City A for these categories.  
3. **Grow Female Segment** → Launch exclusive early-bird women-only offers or “Shop with Friends” bundle deals to close the ₹700 gap.  
4. **City A Upside Opportunity** → Run deeper discounts or free delivery thresholds specifically for City A to lift average ticket size.  
5. **Married & Older Customers** → Create family-oriented bundles and senior-citizen morning slots with extra loyalty points.  
6. **Next Step** → Build a customer segmentation RFM + demographic model for personalized offers in the next event.

**Result Expected**: 8–12% overall revenue lift in the next Black Friday with the same traffic, simply by smarter targeting and inventory allocation.