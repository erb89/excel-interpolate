# excel-interpolate
interpolate between a series of spreadsheet values

if you have a column A of values, copy the following into column B to interpolate once, and average between those values
=IF(MOD(ROWS($B$2:B2),2)=0,AVERAGE(B1,B3),OFFSET($A$2,INT((ROWS($B$2:B2)-1)/2),,,))
