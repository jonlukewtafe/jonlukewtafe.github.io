# Useful Excel Functions

## Date/Time

## Maths

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
4. `QUARTILE.EXC`
   1. This function splits the selected dataset into two halves by using the medium.
   2. It then calculates the first quartile as the median value in the lower half (first half) and the third quartile as the median value in the upper half.
   3. Keep in mind, that this function *excludes* the median of the initial dataset when calculating the first and third quartiles!
5. `QUARTILE.INC`
   1. This function performs the same function as `QUARTILE.EXC`, but instead includes the median of the initial dataset when calculating the first and third quartiles.
   2. Additionally, the median of the initial dataset is included in both the first and third quartiles when calculating their values.
6.

{% include_relative footer.md %}
