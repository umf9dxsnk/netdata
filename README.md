# Example Prometheus configuration for scraping Netdata metrics
global:
  scrape_interval: 5s
  scrape_timeout: 4s

scrape_configs:
  - job_name: 'netdata'
    metrics_path: '/api/v1/allmetrics'
    params:
      format: ['prometheus']
    static_configs:
      - targets: ['localhost:19999']