FROM arm64v8/alpine:latest

# RUN curl -s https://api.github.com/repos/jbh-cloud/privaxy/releases/latest \
#     | grep "browser_download_url.*deb" \
#     | cut -d : -f 2,3 \
#     | tr -d \" \
#     | wget -qi -


RUN mkdir /app
COPY privaxy /app

ENTRYPOINT ["/app/privaxy"]
#RUN ["/app/privaxy"]