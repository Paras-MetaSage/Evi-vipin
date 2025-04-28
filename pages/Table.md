```sql orders
select
  state,
  sales,
  address,
  channel,
  category,
  '/category/' || category as category_link
from needful_things.orders
limit 100
```

<DataTable data={orders} link=category_link />

