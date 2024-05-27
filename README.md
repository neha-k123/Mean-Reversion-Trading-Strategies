# mean_revert_trading_strats
A mini project to test different implementations of mean reversion trading strategy on NYSE stocks. 
Our work was derived from implementations as described on the [Wikipedia page
]([url](https://en.wikipedia.org/wiki/Rescaled_range)) and [this blog post]([url](https://blogs.cfainstitute.org/investor/2013/01/30/rescaled-range-analysis-a-method-for-detecting-persistence-randomness-or-mean-reversion-in-financial-markets/)) by Jason Voss. 

## Usage
- Our script prompts the user to enter the ticker of the instrument as it appears on the NYSE, followed by the start date and end date for the time period of data collection.
- We scrape data from Yahoo Finance and ask the user how many sub-arrays will be created for the purposes of the rescaled range analysis algorith.

## Results:
- We found that, as Lo (1991) concluded, the stock market has no evidence of long term memory. From January 3, 1950 to November 15, 2012, we found H=0.48, which is less than the H = 0.5 threshold of a system that has long memory. Thus, our preliminary findings indicate that the stock market is mean reverting.
  
- We found that NVIDIA (NYSE: NVID), has H = 0.62 from 2020-01-01 to 2024-05-01 with 4 subarrays and MSFT has H = 0.59 with the same parameters. This indicates that the systems are not mean reverting and instead have long memory.

## Next Steps:
- We plan on writing a separate script to perform an algorithm trading strategy for systems that are mean reverting, using the findings from this script.
