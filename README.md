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
| <1x          | 50%          | 0.0              |
| 1x - 3x      | 23%          | 2.0              |
| 3x - 5x      | 11%          | 4.0              |
| 5x - 10x     | 8%           | 7.5              |
| 10x+         | 8%           | 10.0             |

#### Seth Levine - by Check Size
| Multiple Bin | Distribution | Average Multiple |
| ------------ | ------------ | ---------------- |
| <1x          | 56%          | 0.0              |
| 1x - 3x      | 24%          | 2.0              |
| 3x - 5x      | 7%           | 4.0              |
| 5x - 10x     | 6%           | 7.5              |
| 10x+         | 7%           | 10.0             |

#### Correlation Ventures Data
| Multiple Bin | Distribution | Average Multiple |
| ------------ | ------------ | ---------------- |
| <1x          | 64.8%        | 0.0              |
| 1x - 5x      | 25.3%        | 3.0              |
| 5x - 10x     | 5.9%         | 7.5              |
| 10x - 20x    | 2.5%         | 15.0             |
| 20x - 50x    | 1.1%         | 35.0             |
| 50x+         | 0.4%         | 50.0             |

#### Dave McClure's Post
| Multiple Bin | Distribution | Average Multiple |
| ------------ | ------------ | ---------------- |
| <1x          | 50%          | 0.0              |
| 0.5x         | 25%          | 0.5              |
| 3x           | 18%          | 3.0              |
| 15x          | 5%           | 15.0             |
| 50x          | 2%           | 50.0             |



### Results
