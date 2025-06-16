# Market Basket Analysis – Online Retail

## Project Overview  
Applied Apriori algorithm to retail transaction data to uncover product combinations frequently purchased together, enabling actionable cross-selling strategies.

## Data  
- 541,909 transactions  
- UK-based online retail store data

## Methodology  
- Filtered out invalid/canceled transactions  
- Transformed to one-hot encoded basket table  
- Generated frequent itemsets (support ≥ 2%)  
- Extracted association rules (lift ≥ 1.2)

## Key Findings  
- Top itemsets: [‘tea’, ‘milk’], [‘biscuits’, ‘cookies’], etc.  
- Rule example: **{tea, biscuits} → coffee** (Support: 3%, Confidence: 60%, Lift: 1.3)
  - 📈 Bundle tea, biscuits, and coffee together in promotions.

## Visualizations  
- ![Frequent Itemsets](images/support_count_plot.png)  
- ![Rules Scatter](images/rules_scatter.png)

## Tools Used  
Python, Pandas, mlxtend (Apriori), Matplotlib/Seaborn

## Next Steps  
- Try varying support/confidence thresholds  
- Use FP-Growth for faster processing  
- Integrate results into a Tableau dashboard
