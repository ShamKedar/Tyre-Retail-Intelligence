# 📐 Key DAX Measures

Some of the main Power BI measures include:

```DAX
Net Revenue =
SUM(Sales[Revenue])
```

```DAX
Net Units Sold =
SUM(Sales[Units Sold])
```

```DAX
Gross Revenue =
CALCULATE(
    SUM(Sales[Revenue]),
    Sales[Transaction Type] = "Sale"
)
```

```DAX
Units Sold =
CALCULATE(
    SUM(Sales[Units Sold]),
    Sales[Transaction Type] = "Sale"
)
```

```DAX
Units Returned =
ABS(
    CALCULATE(
        SUM(Sales[Units Sold]),
        Sales[Transaction Type] = "Return"
    )
)
```

```DAX
Return Rate =
DIVIDE(
    [Units Returned],
    [Units Sold],
    0
)
```

```DAX
Inventory Value =
SUMX(
    'Current Stock',
    'Current Stock'[Current Stock Quantity]
        * 'Current Stock'[Unit Cost]
)
```

```DAX
Average Daily Demand =
DIVIDE(
    [Units Sold],
    DISTINCTCOUNT(Sales[Date]),
    0
)
```

```DAX
Days of Inventory =
DIVIDE(
    SUM('Current Stock'[Current Stock Quantity]),
    [Average Daily Demand],
    0
)
```

```DAX
Lead-Time Demand =
[Average Daily Demand]
    * AVERAGE(Supplier[Avg Lead Time])
```

```DAX
Stock Surplus Deficit =
SUM('Current Stock'[Current Stock Quantity])
    - [Lead-Time Demand]
```
