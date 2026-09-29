# Sales-Dashboard
An interactive Excel dashboard that analyses 1,000 coffee orders placed between January 2019 and August 2022 by customers in the United States, United Kingdom and Ireland.

## Files

| File | What it is |
|---|---|
| `coffeeOrdersData.xlsx` | The full workbook: raw data sheets, pivot tables and the dashboard |


## Data

The workbook has three source sheets:

- **orders**: 1,000 order lines (order ID, date, customer ID, product ID, quantity)
- **customers**: 1,000 customer records (name, email, phone, address, country, loyalty card)
- **products**: 48 products (coffee type, roast type, size, unit price, profit)

## What I did

1. **Combined the three sheets** into one order table using `XLOOKUP` (customer name, email, country, loyalty card) and `INDEX-MATCH` (coffee type, roast type, size, unit price).
2. **Calculated sales** as unit price × quantity.
3. **Made codes readable** with nested `IF` formulas, for example turning `Ara` into Arabica and `D` into Dark.
4. **Handled missing customer emails** with an `IF` check so blanks show as empty instead of 0.
5. **Built three pivot tables:** sales by month and coffee type for each year, sales by country, and the top 5 customers.
6. **Built the dashboard** with charts and slicers for size, roast type and loyalty card.

## Key figures

- Total sales across all orders: about $45,134
- United States accounts for most of the sales, at about $35,639, ahead of Ireland (about $6,697) and the United Kingdom (about $2,799)

## Tools

Microsoft Excel: XLOOKUP, INDEX-MATCH, IF, pivot tables, pivot charts, slicers

## Source and credit

I built this by following the YouTube Channel Mo Chen and used the dataset from that tutorial.
