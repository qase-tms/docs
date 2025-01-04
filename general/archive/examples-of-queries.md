# Examples of Queries

{% hint style="info" %}
This page is archived, please find the up to date content [here](../analytics/queries-qql-qase-query-language.md#examples-of-queries).
{% endhint %}

```
entity = "case" and isDeleted is true
```

```
entity = "case" and created >= now("-3d")
```

```
entity = "case" and created <= now("-3d")
```

```
entity = "case" and isDeleted is true and project in ["QTC"]
```

```
project = "QTC" and automation = "Not automated"
```

```
project = "MR" and automation != "Automated"
```

```
project = "QTC" and status in ["Draft", "Actual"]
```

```
entity = "defect" and status !="Open" and severity = "Not set"
```

```
entity = "defect" and status !=1 and severity = 0
```

```
entity = "defect" and status !=1 and severity = 0 and cfv in ["1", "2"]
```

```
entity = "defect" and status !="Open" and severity != "Not set" and milestone is empty
```

```
entity = "defect" and status !="Open" and severity != "Not set" and cf["Defect URL"] is not null
```

```
entity = "case" and author != "CEO" and updated <= now("-1d") and isFlaky is false
```

```
entity = "case" and author != "CEO" and updated <= now("-1d") and project in ('QAS
```
