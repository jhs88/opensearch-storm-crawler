FROM opensearchproject/opensearch-dashboards:latest
RUN /usr/share/opensearch-dashboards/bin/opensearch-dashboards-plugin remove securityDashboards
COPY --chown=opensearch-dashboards:opensearch-dashboards config/opensearch_dashboards.yml /usr/share/opensearch-dashboards/config/
