# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:7.9.1

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
COPY ./config/logstash.yml /usr/share/logstash/config/
COPY ./pipeline/logstash.conf /usr/share/logstash/pipeline/
