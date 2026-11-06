## Questions by domain

```dataview
TABLE WITHOUT ID
  key AS "Domain",
  length(rows) AS "Total"
FROM "02-Projects/AWS-Mentor"
WHERE type = "aws-question" AND cert = "SAA-C03"
GROUP BY domain
SORT key ASC
```

## Questions by cert

```dataview
TABLE WITHOUT ID
  key AS "Cert",
  length(rows) AS "Total"
FROM "02-Projects/AWS-Mentor"
WHERE type = "aws-question"
GROUP BY cert
```

## Questions requiring verification

```dataview
TABLE id, cert, domain, status, source
FROM "02-Projects/AWS-Mentor"
WHERE type = "aws-question"
AND status != "verified"
SORT created DESC
```

## Recent sessions

```dataview
TABLE cert, date, correct_answers, total_questions, score, accuracy
FROM "02-Projects/AWS-Mentor"
WHERE type = "aws-session"
SORT date DESC
LIMIT 10
```

## Open mistakes

```dataview
TABLE cert, domain, mistake_type, created
FROM "02-Projects/AWS-Mentor"
WHERE type = "aws-mistake"
AND status != "resolved"
SORT created DESC
```

## Recent insights

```dataview
TABLE cert, domain, insight_type, created
FROM "02-Projects/AWS-Mentor"
WHERE type = "aws-insight"
SORT created DESC
LIMIT 10
```

## Lab log

```dataview
TABLE cert, domain, service, platform, status, estimated_cost_usd
FROM "02-Projects/AWS-Mentor"
WHERE type = "aws-lab-log"
SORT date DESC
```
