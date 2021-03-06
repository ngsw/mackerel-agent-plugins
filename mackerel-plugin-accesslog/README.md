mackerel-plugin-accesslog
=====================

accesslog custom metrics plugin for mackerel.io agent.

Apache log format (common and combined) and LTSV log format are supported.

## Synopsis

```shell
mackerel-plugin-accesslog /path/to/access.log
```

## Example of mackerel-agent.conf

```
[plugin.metrics.accesslog]
command = "/path/to/mackerel-plugin-accesslog /path/to/access.log"
```

## Screenshot

![graphs-screenshot](https://user-images.githubusercontent.com/177122/27474076-22f7defc-583c-11e7-84ee-1679e5164358.png)

## Graphs and Metrics

### accesslog.access_num

- accesslog.access_num.total_count
- accesslog.access_num.2xx_count
- accesslog.access_num.3xx_count
- accesslog.access_num.4xx_count
- accesslog.access_num.5xx_count

### accesslog.access_rate

- accesslog.access_rate.2xx_percentage
- accesslog.access_rate.3xx_percentage
- accesslog.access_rate.4xx_percentage
- accesslog.access_rate.5xx_percentage

## accesslog.latency

Latency (Available only with LTSV format)

- accesslog.average
- accesslog.90_percentile
- accesslog.95_percentile
- accesslog.99_percentile
