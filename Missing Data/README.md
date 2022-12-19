
## Missing Data

The most frequently used method to handle missing data is known as listwise deletion and refers to the exclusion of rows with NAs. Another popular approach is single imputation which substitutes missing values with the mean, median or mode. The one that fascinates me is multiple imputation (or MICE) which imputes missing values based on the patterns of those that are available. Which of these is best will depend on the data at hand. In real projects where time is of the essence, this is decided on the proportion of missingness in each column. However, there are some general recommendations: <br>

**Listwise Deletion**
- Mssing data are Missing Completely at Random (MCAR)
- Less than (approximately) 5% of the data are missing in the relevant variable(s)
- Prefer to use with large datasets as it affects statistical power

**Single Imputation**
- Mssing data are Missing Completely at Random (MCAR)
- Less than (approximately) 5% of the data are missing in the relevant variable(s)
- Avoid mean imputation 

**Multiple Imputation**
- When more than 5% of data are missing from the variables of interest.
- When less than 40% of data in each variable are missing (Jakobsen et al., 2017)
- Ideally when data are missing at random (i.e., MCAR or MAR).

Listwise deletion and single imputation are quick and easy to figure out so we will not be discussing them any further. A more detailed discussion can be found in [Chapter 1](https://stefvanbuuren.name/fimd/sec-simplesolutions.html#sec:simplesolutions) of Stef Van Buuren's free e-book, [Flexible Imputation of Missing Data](https://stefvanbuuren.name/fimd/).
