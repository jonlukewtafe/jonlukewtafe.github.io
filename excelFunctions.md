# Useful Excel Functions

## Date/Time

## Maths

1. `QUARTILE.EXC`
   1. This function splits the selected dataset into two halves by using the medium.
   2. It then calculates the first quartile as the median value in the lower half (first half) and the third quartile as the median value in the upper half.
   3. Keep in mind, that this function **excludes** the median of the initial dataset when calculating the first and third quartiles!
2. `QUARTILE.INC`
   1. This function performs the same function as `QUARTILE.EXC`, but instead **includes** the median of the initial dataset when calculating the first and third quartiles.
   2. Additionally, the median of the initial dataset is included in both the first and third quartiles when calculating their values.

## Logic

1. `IF`
   1. Allows you to automate decision making in a spreadsheet.
   2. Particularly useful if you need to check whether a cell contains a value or if a cell value is above, below or equal to a particular value.
2. `CONCATENATE`
   1. Allows you to combine the value from multiple cells into one.
   2. For example, if you have a first and last/second name in two seperate cells, you can use the `CONCATENATE` function to combine them into a singular cell, making it easier to read.

## Other

1. `COUNT`
   1. Counts the number of cells within the given range
   2. Useful for if you need to know how many cells are contained within your data set.
2. `COUNTBLANK`
   1. Allows for the counting of any blank/empty cells within a given range.
   2. Useful for if you need to check how row cells within a given table column are empty.
3. `COUNTIF`
   1. Counts the number of cells which match the given condition
   2. Useful for if you want to know the number of cells that match a given condition.
      1. This condition could use other functions.

## To Be Added
1. `VAR.P`
   1. Calculates the variance of the given dataset based on the entire population, ignoring logical values and text in the population.
   2. (Microsoft's Support Page for this function)[https://support.microsoft.com/en-us/office/var-p-function-73d1285c-108c-4843-ba5d-a51f90656f3a]
2. `VAR.S`
   1. Estimates the variance based on a given sample of a dataset, ignoring logical values and text in the sample.
   2. (Microsoft's Support Page for this function)[https://support.microsoft.com/en-us/office/var-s-function-913633de-136b-449d-813e-65a00b2b990b]
3. `STDEV.P`
   1. 
4. `STDEV.S`
5. 

{% include_relative footer.md %}
