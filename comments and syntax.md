To enter a line - `click Shift + Enter`

To enter a comment -`//`


Florida Sales of Product 1 or 2 = 

CALCULATE( [Total Sales],

    FILTER ( Locations, Locations[State Code] = "FL"),
    
        FILTER(Products, Products[Product Name] = "Product 1" || Products[Product Name] = "Product 2")) // or syntax

// This is a comment


Or 


Florida Sales of Product 1 or 2 = 

VAR FloridaLocation = FILTER ( Locations, Locations[State Code] = "FL")

VAR ProductSelection = FILTER(Products, Products[Product Name] = "Product 1" || Products[Product Name] = "Product 2")

Return
CALCULATE( [Total Sales], 

    FloridaLocation,
    
        ProductSelection) // or syntax

// This is a comment
