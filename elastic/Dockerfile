from docker.elastic.co/elasticsearch/elasticsearch:7.10.0
# centos basic
RUN yum install sudo -y && sudo yum update -y && sudo yum install nano -y && sudo yum clean all -y
# opendistro plugins https://opendistro.github.io/for-elasticsearch-docs/docs/install/plugins/#job-scheduler
RUN sudo /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch https://d3g5vo6xdbdb9a.cloudfront.net/downloads/elasticsearch-plugins/opendistro-job-scheduler/opendistro-job-scheduler-1.12.0.0.zip
RUN sudo /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch https://d3g5vo6xdbdb9a.cloudfront.net/downloads/elasticsearch-plugins/opendistro-alerting/opendistro_alerting-1.12.0.2.zip
RUN sudo /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch https://d3g5vo6xdbdb9a.cloudfront.net/downloads/elasticsearch-plugins/opendistro-sql/opendistro_sql-1.12.0.0.zip
RUN sudo /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch https://d3g5vo6xdbdb9a.cloudfront.net/downloads/elasticsearch-plugins/opendistro-reports-scheduler/opendistro-reports-scheduler-1.12.0.0.zip
RUN sudo /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch https://d3g5vo6xdbdb9a.cloudfront.net/downloads/elasticsearch-plugins/opendistro-anomaly-detection/opendistro-anomaly-detection-1.12.0.0.zip
RUN sudo /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch https://d3g5vo6xdbdb9a.cloudfront.net/downloads/elasticsearch-plugins/performance-analyzer/opendistro_performance_analyzer-1.12.0.0.zip