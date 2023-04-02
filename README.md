
## SQL HackerRank Challange

Here is the Challange I completed about SQL on HackerRank


## Weather Analysis

There is a tale with daily weather data over the last 6 months of 2020, including the maximum, minimum, and average temperatures.
Write a query that gives month, monthly maximum, monthly minimum, mnthly average temperatures for the six months.

```bash
  SELECT MONTH(record_date), MAX(data_value) AS max, MIN(data_value) AS min,
       round(AVG(CASE WHEN data_type = 'avg' then data_value END)) AS avg
FROM temperature_records
WHERE MONTH(record_date) BETWEEN 7 AND 12
GROUP BY MONTH(record_date)
ORDER BY MONTH(record_date);
```

## Note
Round the average to the nearest integer.





