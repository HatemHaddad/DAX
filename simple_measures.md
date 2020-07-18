

`Quantity Sold = SUM(Sales[Quantity])`

`Average Quantity = Average(Sales[Quantity])`



__Iterating Functions - Very Important__




`Total Sales = SUMX( sales, sales[Quantity] * sales[Price])`


`Total Transaction = COUNTROWS( SALES )`

---

Measure Branching - Measures out of measures

In Sales Table we want to RELATE to the Products table to calculate Total Cost

`Total Cost = SUMX(Sales, RELATED(Products[Product Cost]))`

`Total Profits = [Total Sales] - [Total Cost]`

`Profit Margin = DIVIDE([Total Profits],[Total Sales],0)`

---
