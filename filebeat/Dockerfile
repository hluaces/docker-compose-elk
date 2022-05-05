ARG FILEBEAT_VERSION
FROM docker.elastic.co/beats/filebeat-oss:${FILEBEAT_VERSION:-latest}

ADD sample.log /var/log/sample.log
ADD filebeat.yml /usr/share/filebeat/filebeat.yml

USER root
RUN chmod go-w /usr/share/filebeat/filebeat.yml
