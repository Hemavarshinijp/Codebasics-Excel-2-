# Codebasics-Excel-2-

In this Dataset I did VLOOKUP, INDEXMATCH, XLOOKUP to retrieve the data from one table to another table

# VLOOKUP FUNCTION

=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])

VLOOKUP(Movies[@[movie_id]:[movie_id]], Financials, 5, FALSE)

# INDEXMATCH FUNCTION

=INDEX(return_range, MATCH(lookup_value, lookup_range, 0))

   =INDEX(Table, row, column)

INDEX(Financials, MATCH(Movies7[@[movie_id]:[movie_id]], Financials[[movie_id]:[movie_id]],0),MATCH("Currency", Financials[#Headers],0))

# XLOOKUP FUNCTION

=XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found], [match_mode], [search_mode])

XLOOKUP((Movies[@[mobie_id]:[movie_id]], Finance[movie_id]:[movie_id], Finance[Budget], Not Available, 0)
