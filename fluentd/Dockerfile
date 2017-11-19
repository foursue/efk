FROM fluent/fluentd
RUN apk add --no-cache --update --virtual .build-deps  build-base ruby-dev \
  && gem install \
	fluent-plugin-elasticsearch --no-document \
  && gem sources --clear-all \
  && apk del --purge .build-deps

