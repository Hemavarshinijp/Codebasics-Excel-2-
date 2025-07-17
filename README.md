# Codebasics-Excel-2-

In this Dataset I did VLOOKUP, INDEXMATCH, XLOOKUP to retrieve the data from one table to another table

# VLOOKUP FUNCTION
VLOOKUP(Movies[@[movie_id]:[movie_id]], Financials, 5, FALSE)
# INDEXMATCH FUNCTION
INDEX(Financials, MATCH(Movies7[@[movie_id]:[movie_id]], Financials[[movie_id]:[movie_id]],0),MATCH("Currency", Financials[#Headers],0))
# XLOOKUP FUNCTION
XLOOKUP((Movies[@[mobie_id]:[movie_id]], Finance[movie_id]:[movie_id], Finance[Budget], Not Available, 0)
