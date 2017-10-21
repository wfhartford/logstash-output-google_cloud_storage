FROM logstash:2.4.1

COPY gcs.p12 /

COPY logstash-output-google_cloud_storage.gem /
RUN /opt/logstash/bin/logstash-plugin install logstash-output-google_cloud_storage.gem

COPY test-config.conf /
COPY input.txt /
