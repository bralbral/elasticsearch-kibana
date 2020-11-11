from kibana:7.9.1
# centos basic
USER root
RUN yum install sudo -y && sudo yum update -y && sudo yum install nano -y && sudo yum clean all -y
# opendistro kibana plugins https://opendistro.github.io/for-elasticsearch-docs/docs/kibana/plugins/#install
USER kibana
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-query-workbench/opendistro-query-workbench-1.11.0.0.zip
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-alerting/opendistro-alerting-1.11.0.0.zip
RUN /usr/share/kibana/bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-anomaly-detection/opendistro-anomaly-detection-kibana-1.11.0.0.zip
