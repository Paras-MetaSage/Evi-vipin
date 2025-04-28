---
title: Category Details
---

# Category: {params.category}

```sql category_orders
select *
from needful_things.orders
where category = '${params.category}'
limit 100
```

<DataTable data={category_orders} /> 