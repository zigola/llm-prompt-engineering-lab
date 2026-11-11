# Classification prompt

```text
Classify the input into exactly one of the allowed labels.
Return JSON only with this schema:
{"label":"<allowed label>","confidence":0.0,"reason":"short evidence-based reason"}

Allowed labels: [positive, neutral, negative]
Input: {{text}}
```

Always validate the returned JSON and treat confidence as an estimate, not proof.
