## Questions by topic

```dataview
TABLE WITHOUT ID
  key AS "Topic",
  length(rows) AS "Total"
FROM "02-Projects/Millionaire-Mentor/Questions"
WHERE type = "millionaire-question"
GROUP BY topic
SORT key ASC
```

## Questions by difficulty

```dataview
TABLE WITHOUT ID
  key AS "Difficulty",
  length(rows) AS "Total"
FROM "02-Projects/Millionaire-Mentor/Questions"
WHERE type = "millionaire-question"
GROUP BY difficulty
SORT key ASC
```

## Questions requiring verification

```dataview
TABLE id, topic, difficulty, status, source
FROM "02-Projects/Millionaire-Mentor/Questions"
WHERE type = "millionaire-question"
AND status != "verified"
SORT created DESC
```

## Recent sessions

```dataview
TABLE date, correct_answers, total_questions, score, accuracy
FROM "02-Projects/Millionaire-Mentor/Sessions"
WHERE type = "millionaire-session"
SORT date DESC
LIMIT 10
```

## Open mistakes

```dataview
TABLE question, topic, difficulty, mistake_type, created
FROM "02-Projects/Millionaire-Mentor/Mistakes"
WHERE type = "millionaire-mistake"
AND status != "resolved"
SORT created DESC
```

## Recent insights

```dataview
TABLE topic, insight_type, created
FROM "02-Projects/Millionaire-Mentor/Insights"
WHERE type = "millionaire-insight"
SORT created DESC
LIMIT 10
```
