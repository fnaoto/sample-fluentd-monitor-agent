FROM ruby:2.5

USER root
RUN gem install fluentd-ui
RUN fluentd-ui setup
CMD fluentd-ui start
