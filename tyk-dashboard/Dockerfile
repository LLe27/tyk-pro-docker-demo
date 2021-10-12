FROM        tykio/tyk-dashboard:latest

MAINTAINER  Zaid Albirawi

COPY        ./scripts/wait-for-it.sh /bin/
COPY        ./confs/tyk_analytics.conf /opt/tyk-dashboard/tyk_analytics.conf
RUN         chmod +x /bin/wait-for-it.sh

ENTRYPOINT  /bin/wait-for-it.sh -t 300 localhost:27017 && \
			/opt/tyk-dashboard/tyk-analytics --conf=/opt/tyk-dashboard/tyk_analytics.conf
