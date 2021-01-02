from docker.elastic.co/kibana/kibana:7.10.0
# centos basic
USER root
RUN yum install sudo -y && sudo yum update -y && sudo yum install nano -y && sudo yum clean all -y
# opendistro kibana plugins https://opendistro.github.io/for-elasticsearch-docs/docs/kibana/plugins/#install
USER kibana
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-alerting/opendistroAlertingKibana-1.12.0.2.zip
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-anomaly-detection/opendistroAnomalyDetectionKibana-1.12.0.0.zip
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-query-workbench/opendistroQueryWorkbenchKibana-1.12.0.0.zip
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-trace-analytics/opendistroTraceAnalyticsKibana-1.12.0.0.zip
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-notebooks/opendistroNotebooksKibana-1.12.0.0.zip
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-reports/linux/x64/opendistroReportsKibana-1.12.0.0.zip
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-gantt-chart/opendistroGanttChartKibana-1.12.0.0.zip
