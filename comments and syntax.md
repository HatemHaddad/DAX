To enter a line - `click Shift + Enter`

To enter a comment -`//`


Florida Sales of Product 1 or 2 = 

`CALCULATE( [Total Sales], 

    FILTER ( Locations, Locations[State Code] = "FL"),
    
        FILTER(Products, Products[Product Name] = "Product 1" || Products[Product Name] = "Product 2"))` // or syntax

// This is a comment
