At the time of writing this article, a publicly known exploit in log4j with no CVE assigned was doing rounds on the internet. 


**Affected Versions**


```
2.0 <= Apache log4j <= 2.14.1
```

**Patched Versions**


```
log4j-2.15.0-rc1
```

**Patch without updating log4j**

```
set configuration log4j2.formatMsgNoLookups to true
```

**References**

- https://www.lunasec.io/docs/blog/log4j-zero-day/?s=09
- https://twitter.com/P0rZ9/status/1468949890571337731
- https://github.com/apache/logging-log4j2/pull/608
- https://github.com/tangxiaofeng7/apache-log4j-poc


**Detection**

- https://semgrep.dev/s/chegg:log4j2_tainted_argument
