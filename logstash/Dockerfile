ARG LOGSTASH_VERSION
FROM docker.elastic.co/logstash/logstash-oss:${LOGSTASH_VERSION:-latest}

RUN mkdir /usr/share/logstash/patterns
ADD logstash.conf /usr/share/logstash/pipeline/logstash.conf
ADD logstash.yml /usr/share/logstash/config/logstash.yml
ADD patterns /usr/share/logstash/patterns/custom

WORKDIR /usr/share/logstash/pipeline/
