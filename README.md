---Date Table Short With Dax
Code: Date Table = CALENDAR (DATE(2010,1,1), DATE(2010,12,31))

--- Long Date Table with DAX

LongDateTable = 
ADDCOULUMNS(
  CALDENDER(DATE,(2010,1,1), DATE(2010,12,31)),
  "day", DAY([DATE]),
  "month", MONTH([DATE]),
  "year", YEAR([DATE])
)
