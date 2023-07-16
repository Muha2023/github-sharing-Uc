# github-sharing-Uc

### Python For Data Analytics Project 2023 –Unicorn Startup Companies.

Here are the summarize steps involved 

1.The following columns were renamed as 'Date Joined', 'Valuation', 'Select Investors', and 'Funding' to 'Date', 'Valuation ($B)', 'Investors', and 'Funding ($B)' respectively.

2. The 'Investors' column is converted to a string data type using the `astype()` method.

3. The 'Date' column is converted to a datetime data type using the `pd.to_datetime()` function.

4.  The 'Valuation ($B)' column is converted to a string data type, and then the characters ',' (comma), '$' (dollar sign), and 'B' (Billion) are replaced with empty strings using the `str.replace()` method. Finally, the column is converted to a float data type using `astype('float64')`.

5. The 'Funding ($B)' column is converted to a string data type using the `astype()` method.

6. The symbols ',' (comma), '$' (dollar sign), 'B' (billion), and 'M' (million) are removed from the 'Funding ($B)' column using the `str.replace()` method.

7.The 'Unknown' values in the 'Funding ($B)' column are replaced with NaN (missing value) using the `replace()` method.

8.The 'Funding ($B)' column is converted to a float data type using the `astype()` method.

9. The 'Funding ($B)' column is converted to a string data type using the `astype()` method.

10.The 'Funding ($B)' column is checked for values containing 'M' (million) using the `str.contains()` method. If a value contains 'M', it is replaced by removing 'M' and converting the result to a float data type, divided by 1000 using the '//' (floor division) operator. If a value does not contain 'M', 'B' (billion) is removed, and the result is converted to a float data type.

11.  NaN values in the 'Funding ($B)' column are replaced with 0 using the `fillna()` method. Then, the column is converted to an integer data type using `astype('int64')`.
12.I encountered a challenge regarding the conversion of Funding from string to integer as it contain $ sign as well as Millions to Billions.
