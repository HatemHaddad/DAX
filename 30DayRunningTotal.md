30 Day Running Total = 

CALCULATE( [Total Sales],

    FILTER(  ALL(Dates),
    
        Dates[Date] > MAX( Dates[Date]) - 30 &&
        
        Dates[Date] <= MAX( Dates[Date] )))
