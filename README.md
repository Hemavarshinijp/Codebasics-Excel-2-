# Codebasics-Excel-2-

In this Dataset, I did VLOOKUP, INDEXMATCH,and  XLOOKUP to retrieve the data from one table to another table

### VLOOKUP FUNCTION

=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])

VLOOKUP(Movies[@[movie_id]:[movie_id]], Financials, 5, FALSE)

--> The VLOOKUP function is used to look up a value in a table by searching for a corresponding value in the leftmost column of another table.
--> Syntax of the VLOOKUP() function is: 
# VLOOKUP (lookup_value, table_array, col_index_num, [range_lookup])

# Some limitations of VLookup:
--> It searches only the first column of a reference table for a matching value.
--> Adding a new column to the reference table can cause errors by shifting column indexes and changing the referenced columns.

### INDEXMATCH FUNCTION

=INDEX(return_range, MATCH(lookup_value, lookup_range, 0))

   =INDEX(Table, row, column)

INDEX(Financials, MATCH(Movies7[@[movie_id]:[movie_id]], Financials[[movie_id]:[movie_id]],0),MATCH("Currency", Financials[#Headers],0))

INDEX() and MATCH() are two powerful Excel functions that are often used together to search for and retrieve data from a table or range.
The syntax of the INDEX() function is: 
# INDEX(array, row_num, [column_num]).
The syntax of the MATCH() function is:
# MATCH(lookup_value, lookup_array, [match_type]).

### XLOOKUP FUNCTION

=XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found], [match_mode], [search_mode])

XLOOKUP((Movies[@[mobie_id]:[movie_id]], Finance[movie_id]:[movie_id], Finance[Budget], Not Available, 0)

The syntax of the XLOOKUP() function is: 
# XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found], [match_mode])

Unlike VLOOKUP, which only searches in the leftmost column of a table, XLOOKUP is capable of searching in any column.
