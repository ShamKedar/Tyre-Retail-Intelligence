# 🧮 Key Business Metrics

## Net Revenue

Revenue after accounting for returns.

```text
Net Revenue = Sales Revenue + Return Revenue
```

Returns have negative revenue, so they automatically reduce net revenue.

---

## Return Rate

The percentage of sold units that were subsequently returned.

```text
Return Rate =
Returned Units / Sold Units × 100
```

---

## Average Daily Demand

The average number of tyres sold per day.

```text
Average Daily Demand =
Total Units Sold / Number of Sales Days
```

---

## Days of Inventory

An estimate of how many days the current inventory could support based on the calculated demand rate.

```text
Days of Inventory =
Current Stock / Average Daily Demand
```

---

## Lead Time

The amount of time required by a supplier to deliver an order.

For example:

```text
Order placed → 1 August
Order received → 7 August

Lead Time = 6 days
```

---

## Lead-Time Variability

Lead-time variability describes how much the supplier's delivery time changes from one delivery to another.

A supplier with:

```text
Average Lead Time = 7 days
Standard Deviation = 1 day
```

has relatively predictable delivery times.

A supplier with:

```text
Average Lead Time = 7 days
Standard Deviation = 5 days
```

has considerably more variation in delivery times.

The dataset provides `Lead Time Std Dev` as a measure of this variability.

---

## Lead-Time Demand

The expected number of tyres that will be sold while waiting for a supplier replenishment.

```text
Lead-Time Demand =
Average Daily Demand × Average Lead Time
```

For example:

```text
Average Daily Demand = 10 tyres
Average Lead Time = 7 days

Lead-Time Demand = 10 × 7
                 = 70 tyres
```

If current stock is only 50 tyres, the product may face a stockout before the replenishment arrives.

---

## Stock Surplus / Deficit

A simple comparison between current stock and expected demand during supplier lead time.

```text
Stock Surplus / Deficit =
Current Stock - Lead-Time Demand
```

Example:

```text
Current Stock = 50
Lead-Time Demand = 70

Stock Deficit = 50 - 70
              = -20
```

A negative value indicates potential inventory shortage.

---

Lead time = how long it takes for an order to arrive after placing it.

Lead-Time Variability = how much delivery times vary around the average.

Lead-Time Demand = expected demand during supplier lead time.

Stock Surplus/Deficit = Stock more than demand trend / Stock less than demand trend.

Stock Surplus = business holds stock that exceeds current customer demand and safety requirements.

Stock Deficit = business holds lower stock than current customer demand and safety requirements.

SKU = unique alphanumeric code assigned by a business to a product for internal inventory tracking.
