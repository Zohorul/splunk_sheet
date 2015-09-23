# splunk_sheet
Cheat sheet for splunk search command line

##API

```
index="api" source="/data/log/api_go/supervisor_log.txt"  "match" | rex field=_raw ".*\| (?<number>\d+\.\d+)s" | search number > 1
```
