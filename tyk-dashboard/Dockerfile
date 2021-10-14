FROM        tykio/tyk-dashboard:latest

MAINTAINER  Zaid Albirawi

COPY        ./confs/tyk_analytics.conf /opt/tyk-dashboard/tyk_analytics.conf

ENTRYPOINT  sleep 60 && /opt/tyk-dashboard/tyk-analytics --conf=/opt/tyk-dashboard/tyk_analytics.conf
