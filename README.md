# Monte Carlo Simulations for Early Stage Venture Portfolios
This is a quick script I wrote to experiment with different portfolio construction theories around early stage venture funds. It's completely non-scientific, loaded with all sorts of generic assumptions, and the code quality is poor. _Yes, I know that my for-loop iterations are wildly inefficient and could be vectorized_. This was my quick hack to look at these.

### Assumptions
The purpose of this experiment was to analyze the size (in quantity of investments) of a portfolio assuming a variety of different outcome distributions. The numbers were taken from the following sources:

- Seth Levine post (by fund size <$100mm and also by check size <$1mm
- Correlation ventures data
- Dave McClure's post on portfolio size

When there was a multiple range assigned to a bin, I picked a multiple right in the middle, except for the final bin... more on that later.


#### Seth Levine - by Fund Size
| Multiple Bin | Distribution | Average Multiple |
| ------------ | ------------ | ---------------- |
| <1x          | 50%          | 0                |
| 1x - 3x      | 23%          | 2                |


### Results
