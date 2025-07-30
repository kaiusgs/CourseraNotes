# Monitoring and Observability for Development and DevOps  
## Monitoring  
- Types  
    1. System Monitoring  
        ![system_monitoring](./static/14/system_monitoring.png)  
    2. Dependency Monitoring  
        - If your application isn’t working properly, your dependency monitoring tool could tell you where the error originates from, based on the mapped connections to your application  
    3. Integation Monitoring  
        ![integation_monitoring](./static/14/integation_monitoring.png)  
    4. Web Performance Monitoring  
        ![web_performance_monitoring](./static/14/web_performance_monitoring.png)  
    5. Business Activity Monitoring  
        ![business_activity_monitoring](./static/14/business_activity_monitoring.png)  
    6. Application Performance Monitoring  
        - IT environment, Infrastructure, Network data, Fast launch and response  
        ![application_performance_monitoring](./static/14/application_performance_monitoring.png)  
        ![apm_tools_functions](./static/14/apm_tools_functions.png)  
    7. Real User Monitoring  
        ![real_user_monitoring](./static/14/real_user_monitoring.png)
    8. Security Monitoring  
        - tracks anomalies and ensures that potential threats are stopped before they are a problem.  
- Golden Signals (for SRE)  
    ![golden_signals](./static/14/golden_signals.png)  
- Evaluation  
    ![monitoring_evaluation](./static/14/monitoring_evaluation.png)  
- Components  
    ![components](./static/14/components.png)  
- Qualities 
    ![monitoring_system_qualities](./static/14/monitoring_system_qualities.png)  
- Metrics  
    ![host_based_metrics](./static/14/host_based_metrics.png)  
    ![application_metrics](./static/14/application_metrics.png)  
    ![network_&_connectivity_metrics](./static/14/network_&_connectivity_metrics.png)  
    ![server_pool_metrics](./static/14/server_pool_metrics.png)  
    ![external_dependency_metrics](./static/14/external_dependency_metrics.png)  
## Monitoring Systems & Techniques  
- Synthetic Monitoring (Synthetic testing or Proactive monitoring)  
    ![synthetic_monitoring](./static/14/synthetic_monitoring.png)  
    ![synthetic_monitoring1](./static/14/synthetic_monitoring1.png)  
    ![synthetic_monitoring_tools](./static/14/synthetic_monitoring_tools.png)  
    - real user monitoring VS synthetic monitoring  
    ![rum](./static/14/rum.png)  
- Application Monitoring  
    - Telemetry is system data that is automatically gathered and recorded for monitoring.  
    ![telemetry_monitored](./static/14/telemetry_monitored.png)  
    ![app_monitoring_steps](./static/14/app_monitoring_steps.png)  
- Prometheus  
    ![prometheus](./static/14/prometheus.png)  
- Grafana  
    ![grafana](./static/14/grafana.png)  
- Alerting  
    ![alert_types](./static/14/alert_types.png)  
> Web transaction: An interaction between a **client**, commonly a web browser, and one or more **databases** as the backend of a multi-tier engineering.  
## Loging  
- Logging & Tracing  
    - Some things to consider logging are an application's incoming and outgoing messages, services and functions, business cases and user journeys, data operations, system events, performance statistics, and threats and vulnerabilities.  
    ![distributed_trace](./static/14/distributed_trace.png)  
    ![distributed_trace1](./static/14/distributed_trace1.png)  
    ![application_logs_types](./static/14/application_logs_types.png)  
    - Storing log data is required for different reasons, including the reliability of systems, the security posture of environments, improvement in IT systems’ decision-making, and auditing purposes.  
## Observability  
- the ability to understand the internal state of a system based on its external outputs.  
![observability_vs_monitoring](./static/14/observability_vs_monitoring.png)  
- 3 Pillars  
    - Logs capture detailed information about individual events or transactions, giving you a chronological record of what happened.  
    - Metrics are numerical measurements with accompanying attributes that show the health of a particular system component.  
    - Traces are records of the information pathways or workflows that are created to follow a work item, like a transaction.  
    ![observability_3pillars](./static/14/observability_3pillars.png)  
- Cloud-native  
![cloud_observability_pillars](./static/14/cloud_observability_pillars.png)
- Sampling  
    - the practice of collecting only a subset of log events for analysis/storage.  
    ![sampling_strategies](./static/14/sampling_strategies.png)  
- Telemetry
    - Telemetry is the automated process of collecting and transmitting data from remote or inaccessible sources to support monitoring and analysis.  
    - The key benefits of telemetry include remote feedback, real-time monitoring of application performance, user activity and experience, and network analytics and security.  
    ![useful_telemetry_types](./static/14/useful_telemetry_types.png)  
    - Types  
    ![telemetry_types](./static/14/telemetry_types.png)  
    - Steps  
    ![telemetry_steps](./static/14/telemetry_steps.png)  
- Tracing for Container-Based Applications  
    ![implementing_tracing_steps](./static/14/implementing_tracing_steps.png)  
    ![distributed_tracing_working](./static/14/distributed_tracing_working.png)  
> Ingestion: The process where log data is formatted and uploaded from external sources such as applications, hosts, and cloud-based logging services.  