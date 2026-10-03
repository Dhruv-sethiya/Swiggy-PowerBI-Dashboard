# DAX Measures

This document contains the DAX measures used in the Swiggy Power BI Executive Dashboard. The formulas below were verified against the Power BI report.

## 1. Total Orders

Counts the number of rows in the dataset.

```DAX
Total Orders =
COUNTROWS('Swiggy_Order_Dataset')
```

## 2. Total Revenue

Calculates the sum of all order amounts.

```DAX
Total Revenue =
SUM('Swiggy_Order_Dataset'[Total_Order_Amount])
```

## 3. Average Order Value

Calculates the average order amount using the `AVERAGE` function.

```DAX
Average Order Value =
AVERAGE('Swiggy_Order_Dataset'[Total_Order_Amount])
```

## 4. Average Delivery Time

Calculates the average delivery duration in minutes.

```DAX
Average Delivery Time =
AVERAGE('Swiggy_Order_Dataset'[Delivery_Time])
```

## 5. Average Customer Rating

Calculates the average customer rating.

```DAX
Average Customer Rating =
AVERAGE('Swiggy_Order_Dataset'[Customer_Rating])
```

## 6. Total Customers

Counts the number of distinct customers.

```DAX
Total Customers =
DISTINCTCOUNT('Swiggy_Order_Dataset'[Customer_ID])
```

## Measure Summary

| Measure | DAX Function | Purpose |
|---|---|---|
| Total Orders | `COUNTROWS` | Counts dataset rows |
| Total Revenue | `SUM` | Calculates total order revenue |
| Average Order Value | `AVERAGE` | Calculates the mean order amount |
| Average Delivery Time | `AVERAGE` | Calculates average delivery duration |
| Average Customer Rating | `AVERAGE` | Calculates average customer rating |
| Total Customers | `DISTINCTCOUNT` | Counts unique customers |

## Notes

- All formulas use the table name `Swiggy_Order_Dataset`.
- Average Order Value is calculated directly using `AVERAGE`, not by dividing Total Revenue by Total Orders.
- Total Orders counts rows. This is equivalent to counting unique order IDs for this dataset because no duplicate order IDs were found during validation.
- These measures respond to the report's filter context, including the dashboard slicers.
