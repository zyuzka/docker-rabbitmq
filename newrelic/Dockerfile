FROM newrelic/infrastructure-bundle:2.7
COPY ./entrypoint.sh entrypoint.sh
RUN chmod +x entrypoint.sh
ENTRYPOINT ["./entrypoint.sh"]
CMD ["/usr/bin/newrelic-infra-service"]
