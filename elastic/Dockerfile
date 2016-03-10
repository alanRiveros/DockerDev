FROM java:8

MAINTAINER Alan riveros <alan.gabriel.riveros@gmail.com>

RUN apt-get install -y wget

# Install Elasticsearch.
RUN \
  cd / && \
  wget https://download.elasticsearch.org/elasticsearch/elasticsearch/elasticsearch-1.5.2.tar.gz && \
  tar -xzvf elasticsearch-1.5.2.tar.gz && \
  rm -f elasticsearch-1.5.2.tar.gz && \
  mv /elasticsearch-1.5.2 /elasticsearch

VOLUME ["/data"]

WORKDIR /data

CMD ["/elasticsearch/bin/elasticsearch"]

EXPOSE 9200
EXPOSE 9300
