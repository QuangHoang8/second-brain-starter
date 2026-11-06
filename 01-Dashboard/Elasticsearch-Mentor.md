## Questions by stage

```dataview
TABLE WITHOUT ID
  key AS "Stage",
  length(rows) AS "Total"
FROM "02-Projects/Elasticsearch-Mentor"
WHERE type = "es-question"
GROUP BY stage
SORT key ASC
```

## Questions requiring verification

```dataview
TABLE id, stage, topic, status, source
FROM "02-Projects/Elasticsearch-Mentor"
WHERE type = "es-question"
AND status != "verified"
SORT created DESC
```

## Recent sessions

```dataview
TABLE stage, date, correct_answers, total_questions, score, accuracy
FROM "02-Projects/Elasticsearch-Mentor"
WHERE type = "es-session"
SORT date DESC
LIMIT 10
```

## Open mistakes

```dataview
TABLE stage, topic, mistake_type, created
FROM "02-Projects/Elasticsearch-Mentor"
WHERE type = "es-mistake"
AND status != "resolved"
SORT created DESC
```

## Recent insights

```dataview
TABLE stage, insight_type, created
FROM "02-Projects/Elasticsearch-Mentor"
WHERE type = "es-insight"
SORT created DESC
LIMIT 10
```

## Benchmarks

```dataview
TABLE stage, goal, change, metric_before, metric_after, verified, date
FROM "02-Projects/Elasticsearch-Mentor"
WHERE type = "es-benchmark"
SORT date DESC
```
