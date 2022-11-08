# The Negative Impact of Local Public Policy on Pittsburgh Residential Property Values

## Abstract
This analysis is aimed at discovering some potential causes or contributions to disparties in Pittsburgh residential property values, especially those which may be resulting from public policies. Analysis of property taxes and median incomes concluded that there is likely a connection between property tax burden >5%, but further analysis would be needed.  

## Purpose
As with most cities, Pittsburgh has pronounced disparities in residential property values between different neighborhoods. Is local public policy in Pittsburgh driving, even partly, these disparties in value? If so, which ones? 

## Background
In 2016, the Urban Redevelopment Authority, along with the Reinvestment Fund, conducted a Market Value Analysis (MVA) of Pittsburgh. The URA utilizated cluster analysis to create block groups with similar economic properties which were then assigned a letter grade based on the economic viability of the block. The factors that were used in the analysis include median sales price, foreclosure as a percent of sales, density of residential housing units, etc.  Block groups such as many of those in neighborhoods like Squirrel Hill, Shadyside, Washington's Landing, downtown, and the strip have "A" or "B" letter grades assigned to them, whereas block groups in Homewood, parts of the North sdie, and the Hill District have "H" or "I" letter grades assigned to them.

It is in our collective interest to reduce the disparities in property values such as those pointed out in the MVA. Even more so, it is in the interests of those own and live in residential properties with comparitively low values to have those values increase. In oder to properly address property value disparities work must be done to understand the unintended consquences of our policies implemented by our public servants which may be contributing. If indeed local public policies, such as zoning laws, city property ownership, or taxation contribute to these disparities, then Pittsburgh local government should act to reverse these policies insofar as the harm is being done. 

Data in this study has been utilized from the following sources:
1. Western Pennsylvania Regional Data Center (http://www.wprdc.org/)
2. Pennsylvania Spatial Data Access (https://www.pasda.psu.edu/)
3. American Community Survey (https://www.census.gov/programs-surveys/acs)

## Analysis
Initial attention was given to the MVA conducted by the URA with consideration of the variables which the URA utilized to characterize the economic wellbeing of each block. Then median residential sale price data per census block was reviewed. Attention was given to visualizing Pittsburgh's zoning, including understanding of how residential zoning may be impacting residential property values. Consideration was given to how City Owned properties which are deemed condemned affect property values. "Count Points in Polygon" was used to assess distribution of city owned properties per census block.

I focused much analysis on property tax burden. I combined point layers from WPRDC and PASDA to have so the estimated property taxes per property could be determined. Then property taxes were considered in light of median income data obtained from the American Community Survey. I used several table joins, and "Join attributes by location" to combine the median income of the neightborhood for each property to the address point layer so that property tax relative to income could be determined for each point.

## Results and Discussion
### URA's Market Value Analysis
![Pittsburgh Market Value Analysis](pgh_mva.svg)
This reproduction of the URA's MVA data provides some context for the study.

### Median Residential Sales Price
![Median Residential Sales Price](Median_residential_sales_price.svg)
Median residential sales price helps to provide further context for the MVA by focusing on one of the variables that the MVA took into consideration.

![Pittsburgh Property Taxes per Household](pgh_prop_taxes_and_income_2.png)
While rates are consistent, the absolute value of property taxes paid per property vary widely throughout Pittsburgh.

![Property Tax as percentage of median income](prop_tax_percent_median_inc.png)
Property tax is taken into consideration given the median income per census block.

## Conclusions
It is reasonable based on this analysis to ascertain that property tax burdens impact continued residential property disparties. Indeed, in some neighborhoods in Pittsburgh, with median household incomes of about 30,000 or less, some households pay >5% of the median income in property taxes. This burden could potentially stifle both individual and collective efforts to invest in activities that may increase residential property values. 

Local government ought to ease the property tax burden of relatively low income neighborhoods. 

## Limitations
This analysis was limited in part by incomplete datasets. The point layers I combined to get the geocoded points for residential properties in Pittsburgh ended up reducing the dataset to around 65,000 points, trimmed from the original around 100,000 points. Missing data and differently entered data such as addresses contributed to this difficulty.

## Future Research
For future research one would need to consider the differences in residential property type. Likewise, the analysis of incomes should be expanded beyond solely median income.
