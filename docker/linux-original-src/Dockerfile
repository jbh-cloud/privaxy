FROM ubuntu:22.04

# RUN curl -s https://api.github.com/repos/jbh-cloud/privaxy/releases/latest \
#     | grep "browser_download_url.*deb" \
#     | cut -d : -f 2,3 \
#     | tr -d \" \
#     | wget -qi -

RUN apt-get update && apt-get install -y ca-certificates
RUN update-ca-certificates
RUN mkdir /app
COPY privaxy /app

# Web GUI
EXPOSE 8000
# Proxy
EXPOSE 8100
# Web GUI API
EXPOSE 8200


ENTRYPOINT ["/app/privaxy"]
#RUN ["/app/privaxy"]