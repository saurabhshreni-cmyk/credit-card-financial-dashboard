# DAX Measures Reference

All custom DAX measures used in `Credit_Card_Report.pbix` are documented here.
Update this file whenever a new measure is added to the report.

---

## Revenue Measures

```dax
Total Revenue = SUM(credit_card[Revenue])
```

```dax
Total Interest Earned = SUM(credit_card[Interest_Earned])
```

```dax
Total Transaction Amount = SUM(credit_card[Trans_Amount])
```

```dax
WoW Revenue Change % =
VAR CurrentWeek = [Total Revenue]
VAR PreviousWeek =
    CALCULATE(
        [Total Revenue],
        DATEADD('Calendar'[Date], -7, DAY)
    )
RETURN
    DIVIDE(CurrentWeek - PreviousWeek, PreviousWeek, 0)
```

---

## Customer Measures

```dax
Total Customers = DISTINCTCOUNT(customer[Client_Num])
```

```dax
Activation Rate =
DIVIDE(
    CALCULATE(COUNTROWS(customer), customer[Activation_30_Days] = 1),
    COUNTROWS(customer),
    0
)
```

```dax
Delinquent Rate =
DIVIDE(
    CALCULATE(COUNTROWS(customer), customer[Delinquent_Acc] = 1),
    COUNTROWS(customer),
    0
)
```

---

## Gender Segmentation

```dax
Male Revenue =
CALCULATE(
    [Total Revenue],
    customer[Gender] = "M"
)
```

```dax
Female Revenue =
CALCULATE(
    [Total Revenue],
    customer[Gender] = "F"
)
```

---

## Card Tier Measures

```dax
Blue Silver Transaction Share =
DIVIDE(
    CALCULATE(
        [Total Transaction Amount],
        credit_card[Card_Category] IN {"Blue", "Silver"}
    ),
    [Total Transaction Amount],
    0
)
```

---

## Regional Measures

```dax
Top 3 States Revenue Share =
DIVIDE(
    CALCULATE(
        [Total Revenue],
        customer[State_cd] IN {"TX", "NY", "CA"}
    ),
    [Total Revenue],
    0
)
```

---

> Add new DAX measures here as you build the report.
> Format: measure name, DAX code block, and a one-line description.
