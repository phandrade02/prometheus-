# **How Prometheus Works**
# Prometheus collects metrics from monitored targets by scraping metrics HTTP endpoints. The metrics are stored in a time-series database. Prometheus uses PromQL to query the data. Data can be visualized using tools like Grafana. Define alerting rules and send notifications when conditions are met.

# **Creating Custom Prometheus Alerts and Alerting Rules for Kubernetes Monitoring**
Write alerting rules in a YAML configuration file.
Reference the alerting rules file in the Prometheus configuration (prometheus.yml).
Apply changes by reloading the Prometheus configuration.

# **What is the Prometheus query you can use in Granfana to properly show usage trend of an application metric that is a counter?**
metric called http_requests_total, i can use the following Prometheus query in Grafana: rate(http_requests_total[1m])
to Visualize in Grafana: I need to Create a new panel in Grafana dashboard. Set the data source to Prometheus. Enter the PromQL query rate(http_requests_total[1m]). Customize the visualization as needed (e.g., line chart, bar chart).
